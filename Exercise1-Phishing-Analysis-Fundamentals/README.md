# Phishing Emails in Action - TryHackMe Lab

---

# Introduction

Phishing is one of the most common cyber attacks used by threat actors to deceive victims into revealing sensitive information such as usernames, passwords, banking credentials, and personal data.

This lab demonstrates various phishing techniques used by attackers including:

- Email spoofing
- URL manipulation
- Tracking pixels
- Credential harvesting
- Brand impersonation
- Malicious attachments
- Social engineering

The objective of this exercise is to identify phishing indicators and understand how attackers trick users into interacting with malicious content.

---

# Objectives

- Identify phishing emails.
- Analyze suspicious email headers.
- Detect spoofed sender addresses.
- Examine malicious links and attachments.
- Understand credential harvesting attacks.
- Recognize common social engineering techniques.

---

# Lab Environment

```bash
Platform : TryHackMe
Room     : Phishing Emails in Action
Category : Phishing Analysis
Difficulty : Easy
```

---

# Task 1 - Introduction

## Description

Introduction to phishing attacks and common phishing indicators.

## Findings

- Learned how attackers impersonate trusted organizations.
- Learned the importance of inspecting sender addresses.
- Understood how phishing emails create urgency.

## Evidence

<img width="1625" height="798" alt="2" src="https://github.com/user-attachments/assets/18400f85-fd01-4a12-8219-92743c800e63" />

---

# Task 2 - Cancel Your Order

## Phishing Indicators

- Fake order cancellation notification.
- Suspicious sender email.
- Social engineering tactics.

## Findings

- Email attempts to create panic.
- Encourages user to click malicious links.

## Question Answered

```bash
Listed as the Merchant:
Amazing Stuff
```

## Evidence

<img width="1330" height="767" alt="3" src="https://github.com/user-attachments/assets/103a3007-e5b5-4219-8b58-75c1c51e941c" />

<img width="1326" height="786" alt="4" src="https://github.com/user-attachments/assets/d481e268-c146-4f1f-a047-586bb7b2dd23" />

<img width="1348" height="747" alt="5" src="https://github.com/user-attachments/assets/d5b39946-4a36-48cc-b768-d9355805031e" />

<img width="1383" height="777" alt="6" src="https://github.com/user-attachments/assets/c3599cc0-56a9-4b88-9369-c729dd352e3b" />

---

# Task 3 - Track Your Package

## Phishing Techniques Used

- Spoofed sender address
- Hyperlink manipulation
- Tracking pixel

## Findings

The email pretends to be a shipping notification.

Observed indicators:

- Fake tracking number.
- Sender domain mismatch.
- Hidden hyperlink destination.
- Tracking pixel embedded within email.

## Question Answered

```bash
Root Domain:
devret.xyz
```

## Evidence

<img width="1346" height="803" alt="7" src="https://github.com/user-attachments/assets/baf9bcdf-5e60-4b12-be9f-fee8f260f1de" />

<img width="1337" height="832" alt="8" src="https://github.com/user-attachments/assets/85fc7992-5289-4e6c-96e6-afb8cc04663d" />

---

# Task 4 - Download Document Here

## Phishing Techniques Used

- Brand impersonation
- URL redirection
- Credential harvesting

## Findings

The email redirects victims through multiple websites before reaching a fake login portal.

Observed indicators:

- Fake OneDrive page.
- Fake Adobe login portal.
- Suspicious URL structure.
- Request for credentials.

## Question Answered

```bash
Attack Type:
Credential Harvesting
```

## Evidence

<img width="1348" height="855" alt="9" src="https://github.com/user-attachments/assets/76ea6b60-0dda-43b9-95f0-84d74f455225" />

<img width="1332" height="867" alt="10" src="https://github.com/user-attachments/assets/6974e58f-a48d-4926-8d10-4897ef473b48" />

<img width="1340" height="860" alt="11" src="https://github.com/user-attachments/assets/0cb377b6-4201-41cd-b85a-0ce42c747fba" />

---

# Task 5 - Your Account Is On Hold

## Phishing Techniques Used

- Netflix impersonation
- Email spoofing
- Malicious attachment

## Findings

The attacker impersonates Netflix and claims the account has been suspended.

Observed indicators:

- Misspelled sender details.
- Fake payment update request.
- Suspicious attachment.

## Question Answered

```bash
Sender Email:
z99@musacombi.online
```

## Evidence

<img width="1337" height="835" alt="12" src="https://github.com/user-attachments/assets/a9e6e761-b4ea-42dd-90ae-1ab482411c24" />

<img width="1322" height="853" alt="13" src="https://github.com/user-attachments/assets/19488774-c46e-4dc8-a43b-e1ec1e0ea078" />

---

# Task 6 - Your Recent Purchase

## Phishing Techniques Used

- Apple impersonation
- BCC abuse
- Malicious attachment

## Findings

The email claims that a recent purchase was made using the victim's account.

Observed indicators:

- BCC recipient.
- Suspicious attachment.
- Fake urgency.
- Blank email body.

## Questions Answered

```bash
BCC = Blind Carbon Copy

Attachment Extension = .dot
```

## Evidence

<img width="1336" height="852" alt="14" src="https://github.com/user-attachments/assets/898bd7f8-d15b-48be-8489-f2bb78629ab4" />

<img width="1323" height="856" alt="15" src="https://github.com/user-attachments/assets/06677ecc-a1a6-456c-b781-fc2ca2b704f3" />

---

# Task 7 - Scheduled Shipment

## Phishing Techniques Used

- DHL impersonation
- Malicious Excel attachment
- Malware execution

## Findings

The attacker disguises the email as a DHL shipment notification.

Observed indicators:

- XLSX attachment.
- Hyperlink hidden inside spreadsheet.
- Attempts to execute malware.

Potential Impact:

- Credential theft
- Persistence
- Ransomware deployment
- Data exfiltration

## Question Answered

```bash
Executable Name:
regasms.exe
```

## Evidence

<img width="1325" height="852" alt="16" src="https://github.com/user-attachments/assets/c140282b-20f8-41fc-8c21-7f8c3c4fc4c3" />

<img width="1333" height="866" alt="17" src="https://github.com/user-attachments/assets/bb8741a5-036e-494e-9327-cdf37771512e" />

<img width="1327" height="847" alt="18" src="https://github.com/user-attachments/assets/ffc6c6a4-48c7-4aad-9357-7373bb0d0841" />

---

# Common Phishing Indicators Identified

| Indicator | Found |
|------------|--------|
| Spoofed Sender | ✓ |
| Fake Domain | ✓ |
| URL Manipulation | ✓ |
| Tracking Pixel | ✓ |
| Credential Harvesting | ✓ |
| Brand Impersonation | ✓ |
| Malicious Attachment | ✓ |
| Malware Execution | ✓ |
| Social Engineering | ✓ |
| Sense of Urgency | ✓ |

---

# Lessons Learned

Through this lab, I learned how attackers use phishing emails to deceive users into revealing sensitive information.

I learned how to:

- Verify sender addresses.
- Inspect URLs before clicking.
- Detect suspicious attachments.
- Recognize credential harvesting attempts.
- Identify social engineering tactics.
- Analyze phishing indicators effectively.

These skills are important for protecting users and organizations from phishing attacks.

---

# Conclusion

The Phishing Emails in Action room successfully demonstrated how cybercriminals use email-based attacks to compromise victims.

By analyzing sender information, links, attachments, and email content, phishing attempts can be detected before damage occurs.

This exercise improved my understanding of phishing analysis and strengthened my cybersecurity awareness.

---

# Completion Evidence

```bash
Room Status : COMPLETED
Tasks Completed : 8
Points Earned : 56
```

## Final Screenshot

<img width="722" height="428" alt="20" src="https://github.com/user-attachments/assets/c912e1e5-e325-4985-980e-174c8d05889a" />
