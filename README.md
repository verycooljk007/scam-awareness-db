# 🛡️ Scam Awareness Database

**A repository dedicated to documenting, analyzing, and exposing common digital scams.**

The goal of this project is to create a "Hall of Shame" for phishing attempts, spam texts, and social engineering attacks. By deconstructing real-world examples, we help users identify red flags and avoid becoming victims.

---

## ⚠️ Safety & Disclaimer
**PLEASE READ BEFORE BROWSING**

1.  **Educational Purpose:** This repository is for educational and research purposes only.
2.  **Do Not Click:** Never visit the URLs listed in this repository. They are malicious sites designed to steal credentials or install malware.
3.  **Defanged Links:** All malicious links in this repo have been "defanged" (e.g., `https` becomes `hxxps`) to prevent accidental clicking.
4.  **Privacy:** All personal phone numbers (sender and receiver) and personal names are redacted to protect privacy, as scammers often use spoofed numbers belonging to innocent people.

---

## 📂 Repository Structure

We organize scams by the **medium** used to deliver them:

* **[`/sms-scams`](./sms-scams)** - "Smishing" attacks sent via text message (e.g., Delivery fees, Bank alerts).
* **[`/email-scams`](./email-scams)** - Phishing emails (e.g., Job offers, Invoice fraud).
* **[`/social-media`](./social-media)** - Scams found on WhatsApp, Telegram, Instagram, etc.

---

## 🚩 How to Spot a Scam (The "Red Flags")

Every entry in this repository analyzes the scam based on these criteria:

* **Urgency:** Does the message demand immediate action? ("Account suspended", "Final Notice")
* **The Link:** Does the URL match the official company domain? (e.g., `netflix-account-verify.com` vs `netflix.com`)
* **The Sender:** Is a "Bank" texting you from a personal mobile number?
* **Generic Greetings:** Does it say "Dear Customer" instead of your name?

---

## 🤝 How to Contribute

We welcome community submissions! If you receive a scam message, please help us document it.

### Submission Rules
1.  **Redact Everything:** You MUST black out your phone number, the sender's phone number (unless it's a confirmed shortcode), and your name/address.
2.  **Defang URLs:** Replace `https://` with `hxxps://` and put brackets around the dot `[.]`.
    * *Bad:* `https://evil-site.com`
    * *Good:* `hxxps://evil-site[.]com`
3.  **No Executables:** Do not upload malware samples or executable files. Only text and screenshots.

### Steps to Submit
1.  Take a screenshot and redact sensitive info.
2.  Create a **New Issue** using the "Scam Report" template.
3.  OR fork this repo and submit a Pull Request adding a markdown file to the appropriate folder.

---

## 📝 Example Entry

Here is how we format our entries:

### [UPS Delivery Fee Scam]

**Type:** SMS
**The Hook:** Claims a package is on hold due to unpaid fees ($2.99).
**Red Flags:**
* Link is `ups-package-handling.com` (Fake domain).
* Sent from a personal +1 (647) area code number.
* Grammar error: "kindly pay the fees."

**Raw Text (Defanged):**
> UPS: We have attempted to deliver your parcel. Unpaid fees: $2.99. Pay here: hxxps://ups-package-handling[.]com

---

## 📜 License
[MIT License](LICENSE)
