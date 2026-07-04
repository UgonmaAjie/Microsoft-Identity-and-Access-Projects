# Monitoring User Access to Microsoft Forms Using Microsoft Defender for Cloud Apps and Microsoft Entra ID

## Overview

This project demonstrates how I used Microsoft Entra ID Conditional Access and Microsoft Defender for Cloud Apps (MDCA) to monitor a user's access to Microsoft Forms.

The objective was to provide visibility into a specific user's cloud application activity without interrupting normal business operations. To achieve this, I configured Conditional Access App Control in **Monitor only** mode and created an Activity Policy in Microsoft Defender for Cloud Apps to generate alerts whenever the monitored user accessed Microsoft Forms.

This project demonstrates how organizations can monitor user sessions, improve visibility into cloud application usage, and collect security insights before enforcing stricter access controls.

---

## Business Scenario

An organization wanted to monitor the Microsoft Forms activity of a user named **Pedro** because the application contained sensitive business forms.

Instead of blocking access, the security team wanted to:

- Monitor Pedro's access to Microsoft Forms.
- Generate alerts whenever he accessed the application.
- Record his activities for auditing and investigation.
- Evaluate user behavior before implementing stricter security controls.

As the Microsoft 365 Security Administrator, I implemented a monitoring solution using Microsoft Entra ID and Microsoft Defender for Cloud Apps.

---

## Objectives

For this project, I aimed to:

- Configure a Conditional Access policy for a specific user.
- Enable Conditional Access App Control in **Monitor only** mode.
- Integrate Microsoft Entra ID with Microsoft Defender for Cloud Apps.
- Create an Activity Policy to monitor Microsoft Forms access.
- Generate alerts whenever the monitored user accessed Microsoft Forms.
- Validate that user activities were successfully captured.

---

## Environment

| Component | Configuration |
|-----------|---------------|
| Identity Platform | Microsoft Entra ID |
| Cloud Security Solution | Microsoft Defender for Cloud Apps |
| Cloud Application | Microsoft Forms |
| Monitored User | Pedro |
| Session Control | Conditional Access App Control |
| Enforcement Mode | Monitor only |

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
# Monitoring User Access to Microsoft Forms Using Microsoft Defender for Cloud Apps and Microsoft Entra ID

## Overview

This project demonstrates how I used Microsoft Entra ID Conditional Access and Microsoft Defender for Cloud Apps (MDCA) to monitor a user's access to Microsoft Forms.

The objective was to provide visibility into a specific user's cloud application activity without interrupting normal business operations. To achieve this, I configured Conditional Access App Control in **Monitor only** mode and created an Activity Policy in Microsoft Defender for Cloud Apps to generate alerts whenever the monitored user accessed Microsoft Forms.

This project demonstrates how organizations can monitor user sessions, improve visibility into cloud application usage, and collect security insights before enforcing stricter access controls.

---

## Business Scenario

An organization wanted to monitor the Microsoft Forms activity of a user named **Pedro** because the application contained sensitive business forms.

Instead of blocking access, the security team wanted to:

- Monitor Pedro's access to Microsoft Forms.
- Generate alerts whenever he accessed the application.
- Record his activities for auditing and investigation.
- Evaluate user behavior before implementing stricter security controls.

As the Microsoft 365 Security Administrator, I implemented a monitoring solution using Microsoft Entra ID and Microsoft Defender for Cloud Apps.

---

## Objectives

For this project, I aimed to:

- Configure a Conditional Access policy for a specific user.
- Enable Conditional Access App Control in **Monitor only** mode.
- Integrate Microsoft Entra ID with Microsoft Defender for Cloud Apps.
- Create an Activity Policy to monitor Microsoft Forms access.
- Generate alerts whenever the monitored user accessed Microsoft Forms.
- Validate that user activities were successfully captured.

---

## Environment

| Component | Configuration |
|-----------|---------------|
| Identity Platform | Microsoft Entra ID |
| Cloud Security Solution | Microsoft Defender for Cloud Apps |
| Cloud Application | Microsoft Forms |
| Monitored User | Pedro |
| Session Control | Conditional Access App Control |
| Enforcement Mode | Monitor only |

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

### Step 1 – Configure the Conditional Access Policy

I created a Conditional Access policy targeting the user **Pedro**.

The policy targeted Microsoft Forms and enabled **Conditional Access App Control** using **Monitor only** mode. This configuration redirected Pedro's session through Microsoft Defender for Cloud Apps without restricting his access.

> **Screenshot:** Conditional Access Policy

---

### Step 2 – Configure an Activity Policy

Next, I navigated to Microsoft Defender for Cloud Apps and created an **Activity Policy**.

The policy was configured to monitor Pedro's activity whenever he accessed Microsoft Forms and to generate alerts for security monitoring purposes.

> **Screenshot:** Activity Policy

---

### Step 3 – Validate the Configuration

To validate the implementation, I signed in as Pedro and accessed Microsoft Forms.

The session displayed a monitoring notification indicating that the session was being monitored through Microsoft Defender for Cloud Apps.

I then confirmed that:

- The activity was recorded.
- An alert was generated.
- The activity appeared in the Defender for Cloud Apps activity log.

> **Screenshot:** Monitoring Notification

> **Screenshot:** Activity Log

> **Screenshot:** Alert Generated

---

## Results

The implementation was successful.

The monitored user was able to continue using Microsoft Forms without interruption while Microsoft Defender for Cloud Apps monitored the session in real time.

The solution provided:

- Visibility into user activity.
- Automated alert generation.
- Activity logging for auditing.
- A non-intrusive monitoring solution using **Monitor only** mode.

---

## Skills Demonstrated

- Microsoft Entra ID
- Conditional Access
- Conditional Access App Control
- Microsoft Defender for Cloud Apps
- Activity Policies
- Cloud Application Security
- Security Monitoring
- Microsoft 365 Security Administration

---

## Conclusion

This project demonstrates my ability to implement Microsoft Entra ID Conditional Access together with Microsoft Defender for Cloud Apps to monitor cloud application usage.

By using **Conditional Access App Control** in **Monitor only** mode, I was able to provide visibility into user sessions, generate security alerts, and record activities without disrupting the user's workflow. This approach enables organizations to assess user behavior and validate security policies before applying more restrictive controls.
## Implementation

### Step 1 – Configure the Conditional Access Policy

I created a Conditional Access policy targeting the user **Pedro**.

The policy targeted Microsoft Forms and enabled **Conditional Access App Control** using **Monitor only** mode. This configuration redirected Pedro's session through Microsoft Defender for Cloud Apps without restricting his access.

> **Screenshot:** Conditional Access Policy

---

### Step 2 – Configure an Activity Policy

Next, I navigated to Microsoft Defender for Cloud Apps and created an **Activity Policy**.

The policy was configured to monitor Pedro's activity whenever he accessed Microsoft Forms and to generate alerts for security monitoring purposes.

> **Screenshot:** Activity Policy

---

### Step 3 – Validate the Configuration

To validate the implementation, I signed in as Pedro and accessed Microsoft Forms.

The session displayed a monitoring notification indicating that the session was being monitored through Microsoft Defender for Cloud Apps.

I then confirmed that:

- The activity was recorded.
- An alert was generated.
- The activity appeared in the Defender for Cloud Apps activity log.

> **Screenshot:** Monitoring Notification

> **Screenshot:** Activity Log

> **Screenshot:** Alert Generated

---

## Results

The implementation was successful.

The monitored user was able to continue using Microsoft Forms without interruption while Microsoft Defender for Cloud Apps monitored the session in real time.

The solution provided:

- Visibility into user activity.
- Automated alert generation.
- Activity logging for auditing.
- A non-intrusive monitoring solution using **Monitor only** mode.

---

## Skills Demonstrated

- Microsoft Entra ID
- Conditional Access
- Conditional Access App Control
- Microsoft Defender for Cloud Apps
- Activity Policies
- Cloud Application Security
- Security Monitoring
- Microsoft 365 Security Administration

---

## Conclusion

This project demonstrates my ability to implement Microsoft Entra ID Conditional Access together with Microsoft Defender for Cloud Apps to monitor cloud application usage.

By using **Conditional Access App Control** in **Monitor only** mode, I was able to provide visibility into user sessions, generate security alerts, and record activities without disrupting the user's workflow. This approach enables organizations to assess user behavior and validate security policies before applying more restrictive controls.
