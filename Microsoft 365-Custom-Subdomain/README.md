# Microsoft 365 Custom Subdomain Configuration

## Project Overview

This project documents the end-to-end process of purchasing a domain from **QServers**, 
creating a custom subdomain, and integrating it with a Microsoft 365 tenant. 
The project demonstrates practical experience with domain management, DNS configuration, domain verification, and Microsoft 365 administration.

---

## Objective

The goal of this project was to:

- Purchase a domain
- Create a custom subdomain.
- Add the subdomain to a Microsoft 365 tenant.
- Verify domain ownership using DNS records.
- Configure the required DNS records.
- Successfully connect the subdomain for use within Microsoft 365.

---

## Technologies Used

- Microsoft 365 Admin Center
- Microsoft Entra ID
- QServers Domain Manager
- DNS Management
- Custom Domain Configuration

---

## Prerequisites

Before starting this project, the following were required:

- A Microsoft 365 tenant
- A registered domain purchased from QServers
- Global Administrator permissions in Microsoft 365
- Access to the QServers DNS Management Portal

---

## Project Steps

### Step 1: Purchase a Domain

Purchased a custom domain from **QServers**.

Example:

![]()
```

---

### Step 2: Create a Custom Subdomain

Created a custom subdomain that would be integrated with the Microsoft 365 tenant.

Example:

```text
lab.example.com
```

---

### Step 3: Add the Subdomain to Microsoft 365

1. Signed in to the **Microsoft 365 Admin Center**.
2. Navigated to **Settings > Domains**.
3. Selected **Add domain**.
4. Entered the custom subdomain.
5. Continued to the verification stage.

---

### Step 4: Verify Domain Ownership

Microsoft 365 generated a **TXT record** for domain verification.

The TXT record was added to the DNS zone in the QServers Domain Manager.

After DNS propagation, Microsoft successfully verified ownership of the subdomain.

---

### Step 5: Configure DNS Records

Configured the required DNS records provided by Microsoft 365, including:

- TXT Record
- MX Record
- CNAME Record
- Autodiscover Record
- SPF Record

These records enabled Microsoft 365 services such as authentication, email delivery, and service discovery.

---

### Step 6: Verify Configuration

After the DNS records propagated:

- The subdomain was successfully verified.
- Microsoft 365 recognized the custom subdomain.
- The subdomain became available for user accounts and Microsoft 365 services.

---

## Result

The project was successfully completed.

The custom subdomain was fully integrated into the Microsoft 365 tenant and was available for organizational use.

---

## Skills Demonstrated

- Microsoft 365 Administration
- Microsoft Entra ID Administration
- DNS Management
- Domain Verification
- Custom Domain Configuration
- Cloud Identity Management
- DNS Troubleshooting

---

## Lessons Learned

This project provided hands-on experience with:

- Purchasing and managing domains using QServers.
- Understanding DNS records and their functions.
- Verifying domain ownership in Microsoft 365.
- Configuring Microsoft 365 custom domains.
- Troubleshooting DNS propagation delays.
- Integrating third-party domain providers with Microsoft 365.

---


---

## Conclusion

This project demonstrates the practical implementation of integrating a custom subdomain from QServers into a Microsoft 365 tenant. It showcases essential Microsoft 365 administration skills, including DNS configuration, domain verification, and cloud identity management, while reinforcing best practices for managing custom domains in enterprise environments.
