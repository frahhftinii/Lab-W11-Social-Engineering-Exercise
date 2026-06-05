# Phishing Analysis Fundamentals

## Objective

The objective of this lab s to understand the fundamentals of phishing analysis by examining email address, email delivery methods, email headers, email bodies, attachment, and different types of phishing attacks.

---

## Tools and Techniques Used
## Tools
- Mozilla Thunderbird
- CyberChef
- TryHackMe

## Techniques
- Email Header Analysis
- Email Metadata Analysis
- Email Body Analysis
- Attachment Analysis
- Base64 Decoding
- Phishing Investigation

---

# Task 1 – Introduction

his task introduced the Phishing Analysis Fundamentals room and the basic purpose of phishing email investigation.

<img width="932" height="712" alt="1" src="https://github.com/user-attachments/assets/a26445ec-9bf2-425c-a3da-d80292e02a45" />

<img width="947" height="777" alt="2" src="https://github.com/user-attachments/assets/86497e44-0479-44fd-8de7-d90a67181bfb" />

---

# Task 2 – The Email Address

This task explained the structure of an email address and how to identify the domain from an email.

### Answer

### Activities Performed

- Examined Return-Path
- Checked Received headers
- Identified sender information
- Reviewed authentication records

### Screenshot

<img width="930" height="832" alt="3" src="https://github.com/user-attachments/assets/555c6586-8458-4246-a71c-61f1b9e2fccb" />

<img width="928" height="655" alt="4" src="https://github.com/user-attachments/assets/56cfbe3b-8e55-4011-b026-93c54f3c53e3" />

---

# Task 3 – Email Delivery

The raw email source was inspected to understand how email messages are structured.

### Findings

- Header information can reveal sender details.
- Authentication results help verify legitimacy.
- Source code contains metadata useful for investigations.

### Screenshot

<img width="943" height="842" alt="5" src="https://github.com/user-attachments/assets/9e47c9e6-bcd9-4b63-9627-84d19f958032" />

<img width="932" height="822" alt="6" src="https://github.com/user-attachments/assets/ccba1bb9-8bf4-429a-9308-a1a25e03c7b0" />

<img width="927" height="613" alt="7" src="https://github.com/user-attachments/assets/e2b8969f-02c0-4a8a-82b2-e48b7d8f2066" />

---

# Task 4 – Email Headers

A suspicious attachment encoded in Base64 format was analyzed.

### Steps Performed

1. Opened the email source.
2. Located the attachment section.
3. Identified Base64 encoded data.
4. Copied the encoded content.
5. Decoded it using CyberChef.
6. Recovered the attached PDF file.

### Flag Obtained

```text
THM{BENIGN_PDF_ATTACHMENT}
```

### Screenshot

<img width="957" height="226" alt="17" src="https://github.com/user-attachments/assets/b670f5f2-c629-4509-b32b-1e45388dfe49" />

<img width="1920" height="877" alt="18" src="https://github.com/user-attachments/assets/7e39a339-09b1-4ff5-ab43-0ead5ad8f763" />

<img width="405" height="102" alt="19" src="https://github.com/user-attachments/assets/c08c84fe-092a-4c5a-94b1-0bb464b8d383" />

---

# Task 5 – Email Body

The email body was reviewed to identify common phishing indicators.

### Indicators Observed

- Urgent language
- Social engineering techniques
- Suspicious links
- Potential impersonation attempts

### Screenshot

<img width="916" height="861" alt="20" src="https://github.com/user-attachments/assets/78e2f8fa-3377-4506-bfd4-2217d33dfe8f" />

<img width="940" height="830" alt="21" src="https://github.com/user-attachments/assets/594f324a-c02c-4e10-b7de-798668667477" />

<img width="928" height="662" alt="22" src="https://github.com/user-attachments/assets/3080a644-a666-4ba1-8ea4-3067b53ab458" />

---

# Task 6 – Types of Phishing

The file **email13.eml** was analyzed to identify the phishing attempt.

### Findings

| Item | Result |
|--------|---------|
| Spoofed Organization | Home Depot |
| Sender Email | support@teckbe.com |
| X-Originating-IP | 103.234.236.83 |
| Authentication Server | atlas102.free.mail.gq1.yahoo.com |

### Screenshot

<img width="862" height="483" alt="24" src="https://github.com/user-attachments/assets/d0bc7c27-86a0-47ce-8023-240958f2d660" />

<img width="965" height="326" alt="25" src="https://github.com/user-attachments/assets/c543b110-03e8-4403-9a51-f3bc27379f38" />

---

# Task 7 – Conclusion

This task introduced Business Email Compromise (BEC), a phishing technique where attackers use compromised email accounts to deceive employees into performing fraudulent actions.

### Answer

```text
Business Email Compromise
```

### Screenshot

<img width="931" height="753" alt="29" src="https://github.com/user-attachments/assets/aaecd026-34c4-4bbc-9329-148862cb5628" />

---

# Key Lessons Learned

- Email headers provide valuable forensic information.
- Attachments should always be treated with caution.
- Base64 encoded content can conceal malicious files.
- Authentication results help verify sender legitimacy.
- Phishing attacks frequently use social engineering techniques.

---

# Conclusion

This lab provided practical experience in phishing email analysis. Through examining email headers, email sources, attachments, and authentication mechanisms, phishing indicators were successfully identified. The exercise demonstrated the importance of email analysis in cybersecurity investigations and phishing detection.
