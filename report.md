# Phishing Email Analysis Report
**Analyst:** Jakka Jayaram  
**Date:** August 6, 2025  
**Subject:** Suspicious USPS Delivery Email  

---

## 1. Overview

I received an email that appeared to be from USPS, claiming a package was ready to be delivered within 60 minutes. At first glance, it looked legitimate — it had the USPS logo, some tracking details, and a "Download details" button. But after digging deeper, it became clear this was a phishing attempt.

---

## 2. Email Header Findings

- **Sender:** USPostalService `<wainani@soclar.net>`  
- **Return Path:** `<wainani@soclar.net>`  
- **Sender IP:** 35.196.193.120  
- **SPF/DKIM/DMARC:** All failed  
- **Authentication Result:** compauth=fail, spf=fail

**What this tells us:**  
The domain `soclar.net` isn't affiliated with USPS, and the email completely fails standard authentication checks (SPF, DKIM, DMARC). This strongly suggests that the sender info was spoofed — a common tactic used in phishing.

---

## 3. Suspicious Link Breakdown

- **Text in email:** USPS.com  
- **Actual link:** `http://lbbyqrluzu.cracknight.ru/dHJw183la23jm?q=9250194086`

**Red flag:**  
While the email *says* it links to USPS, hovering over the button shows it actually redirects to a suspicious Russian domain — a common trick to make malicious links look trustworthy.

---

## 4. Things That Stood Out

Here are the clear signs this email was malicious:

| Indicator | Explanation |
|----------|-------------|
| **Spoofed Sender** | The sender's email looks official, but it’s from a random domain (`soclar.net`). |
| **Authentication Failures** | Fails SPF, DKIM, and DMARC — meaning it wasn’t sent from a trusted source. |
| **Phishing Link** | The "Download details" button links to a shady external domain. |
| **Urgency** | Saying the package is arriving in 60 minutes is designed to pressure the reader into acting quickly. |
| **Generic Greeting** | The email doesn’t include any personal info — just a generic “Hello.” |
| **Deceptive Branding** | The USPS logo is used to make the email look legitimate. |

---

## 5. Final Thoughts

Everything about this email points to a phishing attempt. The spoofed sender, mismatched link, urgency, and failed security checks all suggest it's trying to trick the recipient into clicking a malicious link or downloading malware.

---

## 6. What To Do

If you receive a similar email:

- **Don’t click any links or download anything.**
- **Report the email** to your IT/security team or email provider.
- **Mark it as phishing** in your inbox.
- **Delete it immediately.**
- Let your colleagues know, so
