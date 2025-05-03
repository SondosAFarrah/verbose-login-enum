# 🛡️ Verbose Login Email Enumerator  

A Python script to automate email enumeration by exploiting verbose login endpoints that leak error messages. Ideal for CTF challenges and security testing.  

---

## 📌 Purpose  

Some login systems return different error messages for **valid** vs. **invalid** emails. This script exploits this behavior to:  
✔ Identify registered email addresses.  
✔ Test for insecure login forms in web apps or CTF labs (e.g., TryHackMe, Hack The Box).  

---

## 🔧 How It Works  

1. **Sends a POST request** to the target login endpoint with:  
   - A test email (from your wordlist).  
   - A dummy password.  
2. **Analyzes the response**:  
   - Checks for differences in error messages (e.g., "Invalid password" vs. "User not found").  
   - Flags valid emails based on the server’s feedback.  

---

## 📚 Wordlist Suggestions

You can use pre-made username/email lists from the following GitHub repository:

🔗 **nyxgeek/username-lists**  
https://github.com/nyxgeek/username-lists/tree/master/usernames-top100

---
