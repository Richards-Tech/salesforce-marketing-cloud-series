# 📅 Day 17 – SFMC Learning Series | Learn with Me

## 🚀 Send Classification in Salesforce Marketing Cloud

---

### 🎯 What is Send Classification?
Send Classification in Salesforce Marketing Cloud defines how your email is sent — especially in terms of:  
📩 **Email Type** (Commercial vs Transactional)  
🧾 **Sender Profile** (From Name & Email)  
🔐 **Delivery Profile** (IP, Domain, Header/Footer Rules)  

👉 Think of it as a **control layer** that ensures compliance, branding, and deliverability for every email send.  

---

### 🧩 Components of Send Classification

#### 1️⃣ Sender Profile
Defines **who is sending the email**  
- From Name (e.g., *Company Support*)  
- From Email Address (e.g., *support@company.com*)  

📌 Ensures consistent branding and trust  

---

#### 2️⃣ Delivery Profile
Defines **how the email is technically sent**  
- Sending Domain  
- IP Address (Dedicated/Shared)  
- Header/Footer settings  

📌 Critical for email deliverability & reputation  

---

#### 3️⃣ Send Classification Type
There are 2 main types:  

📢 **Commercial Sends**  
- Used for: Marketing emails, newsletters, promotions  
- Requires:  
  ✅ Unsubscribe link  
  ✅ Compliance with anti-spam laws  
📌 Example: Discount offer, product launch  

⚡ **Transactional Sends**  
- Used for: System-triggered emails  
- No unsubscribe required  
📌 Example:  
  - Order confirmation  
  - Password reset  
  - OTP emails  

---

### 🔄 How It Works in Real Flow
👉 When you send an email:  
**Email → Send Classification → Applies Sender + Delivery Rules → Email Sent**  

📌 Without proper Send Classification, your send may fail or violate compliance rules  

---

### ⚠️ Key Points to Remember
- You must select Send Classification before sending emails  
- It directly impacts:  
  📬 Inbox placement  
  📊 Deliverability  
  ⚖️ Legal compliance (like CAN-SPAM, GDPR)  

---

### 💡 Pro Tips (Real Project Insight)
✔ Use different Send Classifications for:  
- Marketing campaigns  
- Transactional journeys  

✔ Always verify:  
- Sender email domain is authenticated  
- Proper unsubscribe handling for commercial sends  

🧠 **Example:**  
👉 What happens if you send a promotional email using a Transactional Send Classification?  
💬 **Answer:**  
It may bypass unsubscribe requirements — leading to compliance issues and potential legal risk.  

---

### 📊 Final Thought
Send Classification is not just a setting — it’s the **foundation of responsible email sending** in SFMC.  

---

📌 Follow along as I simplify SFMC step by step 👇

<img width="1024" height="1024" alt="Learn with Me" src="https://github.com/user-attachments/assets/b087fd21-b25b-4e36-b3fc-899379ff348c" />
