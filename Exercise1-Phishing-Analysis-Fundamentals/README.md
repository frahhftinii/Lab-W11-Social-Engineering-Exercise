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

This task introduced the Phishing Analysis Fundamentals room and the basic purpose of phishing email investigation.

<img width="932" height="712" alt="1" src="https://github.com/user-attachments/assets/a26445ec-9bf2-425c-a3da-d80292e02a45" />

<img width="947" height="777" alt="2" src="https://github.com/user-attachments/assets/86497e44-0479-44fd-8de7-d90a67181bfb" />

---

# Task 2 – The Email Address

This task explained the structure of an email address and how to identify the domain from an email.

## Answer
```text
tryhatme.com
```

<img width="930" height="832" alt="3" src="https://github.com/user-attachments/assets/555c6586-8458-4246-a71c-61f1b9e2fccb" />

<img width="928" height="655" alt="4" src="https://github.com/user-attachments/assets/56cfbe3b-8e55-4011-b026-93c54f3c53e3" />

---

# Task 3 – Email Delivery

This task explained how emails are sent and received using different protocols and services.

## Answer
```text
SMTP
DNS
IMAP
```

### Findings

- SMTP is used to send emails from a client to a mail server.
- DNS is used to look up the recipient domain's mail server.
- IMAP allows users to access emails from multiple devices.

<img width="943" height="842" alt="5" src="https://github.com/user-attachments/assets/9e47c9e6-bcd9-4b63-9627-84d19f958032" />

<img width="932" height="822" alt="6" src="https://github.com/user-attachments/assets/ccba1bb9-8bf4-429a-9308-a1a25e03c7b0" />

<img width="927" height="613" alt="7" src="https://github.com/user-attachments/assets/e2b8969f-02c0-4a8a-82b2-e48b7d8f2066" />

---

# Task 4 – Email Headers

In this task, the raw source of email1.eml was inspected using Thunderbird. Email headers were analyzed to identify important metadata such as the subject line and originating IP address.

## Answers
```text
Help protect your budget by protecting your home
43.255.56.161
```

### Findings

- The full subject line was identified from the email.
- The X-Originating-IP was found in the raw email header.
- Email headers can reveal useful forensic information about the sender and message origin.

<img width="936" height="830" alt="13" src="https://github.com/user-attachments/assets/d611719d-5762-46e5-9126-0840a87ca250" />

<img width="927" height="762" alt="14" src="https://github.com/user-attachments/assets/18c77be1-6902-45d4-9460-317d19ac86e1" />

<img width="937" height="560" alt="15" src="https://github.com/user-attachments/assets/af9dceab-14fa-4f64-a212-3adda39e6dd8" />

<img width="912" height="538" alt="10" src="https://github.com/user-attachments/assets/14c274d7-9529-432f-a476-886becee9cee" />

<img width="955" height="160" alt="12" src="https://github.com/user-attachments/assets/63a0aaaa-0aef-443c-a90a-42c0a9842236" />

---

# Task 5 – Email Body

In this task, email2.txt was analyzed. The email body contained an attachment encoded in Base64 format. CyberChef was used to decode the Base64 content and recover the PDF attachment.

## Answers
```text
application/pdf
zmqpalgh.pdf
THM{BENIGN_PDF_ATTACHMENT}
```

## Steps Performed
1. Opened email2.txt.
2. Identified the attachment content type as application/pdf.
3. Identified the attachment filename as zmqpalgh.pdf.
4. Copied the Base64 encoded attachment content.
5. Used CyberChef to decode the Base64 data.
6. Recovered the PDF attachment.
7. Opened the PDF and found the flag.

<img width="916" height="861" alt="20" src="https://github.com/user-attachments/assets/238907be-0944-4a35-b4dc-499b0329197b" />

<img width="940" height="830" alt="21" src="https://github.com/user-attachments/assets/004bc637-5ac4-4d1e-ae84-561af0d063ef" />

<img width="928" height="662" alt="22" src="https://github.com/user-attachments/assets/e84eabf6-7eb5-4b39-9dd0-286ab1071c22" />

<img width="957" height="226" alt="17" src="https://github.com/user-attachments/assets/e98cf96b-2453-4b70-97ec-9ed37d0e3467" />

<img width="1920" height="877" alt="18" src="https://github.com/user-attachments/assets/2a9f9b0d-7634-45e7-97f5-4186cd13a2d1" />

<img width="405" height="102" alt="19" src="https://github.com/user-attachments/assets/269e74c7-b7c2-4d05-b9e3-ccae3376e069" />

---

# Task 6 – Types of Phishing

This task introduced different types of phishing attacks and included an investigation of email3.eml.

## Answers
```text
Home Depot
support@teckbe.com
103[.]234[.]236[.]83
atlas102.free.mail.gq1.yahoo.com
```

### Findings

| Item | Result |
|--------|---------|
| Spoofed Organization | Home Depot |
| Sender Email | support@teckbe.com |
| Defanged X-Originating-IP | 103[.]234[.]236[.]83 |
| Authentication Server | atlas102.free.mail.gq1.yahoo.com |

<img width="928" height="861" alt="26" src="https://github.com/user-attachments/assets/2e5cf69e-d5b1-417a-939d-6b4dcebcfc2f" />

<img width="942" height="843" alt="27" src="https://github.com/user-attachments/assets/4976fbe4-5dbf-4426-8c1e-28f61fe3df64" />

<img width="932" height="851" alt="28" src="https://github.com/user-attachments/assets/41c2efad-c854-40e3-bf7e-d1dd8d7d4a7d" />

<img width="862" height="483" alt="24" src="https://github.com/user-attachments/assets/9fd19871-86f7-4bed-b3b8-fc39a043fbea" />

<img width="965" height="326" alt="25" src="https://github.com/user-attachments/assets/f5559474-d5b0-441c-b0ae-d480a72c81d2" />

---

# Task 7 – Conclusion

This task introduced Business Email Compromise (BEC), which is a phishing attack where attackers use a compromised email account to trick employees into fraud.

## Answer

```text
Business Email Compromise
```

### Screenshot

<img width="931" height="753" alt="29" src="https://github.com/user-attachments/assets/aaecd026-34c4-4bbc-9329-148862cb5628" />

---

# Key Lessons Learned
- Email addresses should be checked carefully to identify suspicious domains.
- Email delivery involves SMTP, DNS, and IMAP.
- Email headers contain important metadata such as X-Originating-IP and Authentication-Results.
- Email bodies may contain suspicious links or encoded attachments.
- Base64 encoding can be used to hide attachment content.
- CyberChef can be used to decode encoded email content.
- Phishing attacks can impersonate trusted organizations such as Home Depot.
- Business Email Compromise is a serious phishing technique used for fraud.

---

# Conclusion

This lab provided hands-on experience in phishing analysis fundamentals. By analyzing email addresses, delivery protocols, headers, email bodies, attachments, and phishing types, I gained a better understanding of how phishing emails are investigated. The exercise also showed the importance of examining metadata, suspicious attachments, and sender information before trusting any email.

# Completion Evidence

```bash
Room Status : COMPLETED
Tasks Completed : 7
Points Earned :112
```

<img width="742" height="457" alt="30" src="https://github.com/user-attachments/assets/fe181b35-ff5b-442c-816c-d53a2d954e43" />
