# 🛡️ Verbose Login Email Enumerator

This Python script automates the process of enumerating valid email addresses by interacting with a **verbose login endpoint** that leaks error messages, commonly found in Capture The Flag (CTF) labs or vulnerable web applications.

---

## 📌 Purpose

In some login forms, servers return different messages depending on whether an email/username exists or not. This script takes advantage of that to distinguish between **valid** and **invalid** email addresses.

---

## 🔧 How It Works

- Sends a POST request to the login endpoint with a target email and dummy password.
- Parses the JSON response.
- Based on the error message, determines whether the email exists.
- Useful for:
  - CTF challenges (like TryHackMe or Hack The Box)
  - Security testing labs with verbose login messages

---

## 🚀 Usage

```bash
python3 verboseLogin.py <email_list_file>
