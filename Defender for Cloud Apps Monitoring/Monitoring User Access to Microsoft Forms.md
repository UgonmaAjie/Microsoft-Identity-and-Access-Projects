# Monitoring User Access to Microsoft Forms Using Microsoft Defender for Cloud Apps and Microsoft Entra ID

## Project Overview

This project demonstrates how to monitor a user's access to Microsoft Forms by integrating Microsoft Entra ID Conditional Access with Microsoft Defender for Cloud Apps (MDCA).

In this scenario, a user named **Pedro** is required to use Microsoft Forms to access sensitive organizational forms. Rather than restricting his access, the security team wants to gain visibility into his activities by monitoring his sessions and generating alerts whenever he accesses Microsoft Forms.

To achieve this, Conditional Access App Control was configured in **Monitor only** mode, allowing administrators to observe Pedro's activity without interrupting his workflow.

---

## Project Scenario

A security administrator has been asked to monitor a specific employee's access to Microsoft Forms.

The objective is to:

- Monitor Pedro's Microsoft Forms sessions.
- Generate security alerts whenever Pedro accesses Microsoft Forms.
- Gain visibility into Pedro's activities.
- Allow uninterrupted access while monitoring user behavior.

This implementation enables administrators to evaluate user activity before enforcing stricter security controls if necessary.

---

## Technologies Used

- Microsoft Entra ID
- Microsoft Defender for Cloud Apps (MDCA)
- Microsoft Forms
- Conditional Access
- Conditional Access App Control
- Activity Policies

---

## Architecture

```
Pedro
   │
   ▼
Microsoft Entra ID
   │
Conditional Access Policy
   │
Use Conditional Access App Control
(Monitor only)
   │
   ▼
Microsoft Defender for Cloud Apps
   │
Activity Policy
   │
Alerts & Activity Logs
```

---

## Implementation

### Step 1: Configure Conditional Access

A Conditional Access policy was created in Microsoft Entra ID with the following configuration:

- **User:** Pedro
- **Target Resource:** Microsoft Forms
- **Session Control:** Use Conditional Access App Control
- **Mode:** Monitor only

This configuration redirects Pedro's Microsoft Forms session through Microsoft Defender for Cloud Apps, enabling session monitoring without blocking access.

---

### Step 2: Configure Microsoft Defender for Cloud Apps

After enabling Conditional Access App Control, an Activity Policy was created in Microsoft Defender for Cloud Apps.

The policy was configured to:

- Monitor Pedro's activity.
- Detect access to Microsoft Forms.
- Generate alerts whenever Pedro accessed the application.
- Record activity for investigation and auditing purposes.

---

### Step 3: Test the Configuration

The policy was validated by signing in as Pedro and accessing Microsoft Forms.

During testing:

- Pedro successfully accessed Microsoft Forms.
- A session notification appeared informing the user that the session was being monitored.
- Microsoft Defender for Cloud Apps recorded the activity.
- Alerts were generated according to the configured Activity Policy.

---

## Expected Outcome

After completing the implementation:

- Pedro can continue accessing Microsoft Forms normally.
- Every monitored session is routed through Microsoft Defender for Cloud Apps.
- Administrators receive alerts whenever Pedro accesses Microsoft Forms.
- User activities are recorded for auditing and investigation.
- No access is blocked because the policy operates in **Monitor only** mode.

---

## Security Benefits

- Provides visibility into user activity.
- Enables real-time monitoring of cloud application sessions.
- Generates security alerts for monitored users.
- Supports auditing and compliance requirements.
- Allows organizations to evaluate user behavior before enforcing stricter controls.

---

## Skills Demonstrated

- Microsoft Entra ID Administration
- Conditional Access Policy Configuration
- Conditional Access App Control
- Microsoft Defender for Cloud Apps
- Activity Policy Configuration
- Cloud Application Security
- Session Monitoring
- Security Monitoring and Alerting

---


## Key Takeaways

This project demonstrates how Microsoft Entra ID and Microsoft Defender for Cloud Apps work together to provide visibility into cloud application usage.

By using **Conditional Access App Control** in **Monitor only** mode, organizations can observe user behavior, generate alerts, and collect valuable security insights without disrupting productivity.

This approach is especially useful when evaluating security policies before transitioning to stricter access controls such as blocking downloads, preventing uploads, or enforcing session restrictions.
