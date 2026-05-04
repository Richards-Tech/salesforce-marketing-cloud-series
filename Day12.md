# 📅 Day 12 – SFMC Learning Series | Learn with Me

## 📨 Complete Email Send Flow in SFMC

👉 One thing while learning SFMC:  
Many people know how to click **Send**  
But don’t understand what happens in the backend before an email reaches the subscriber  

---

### 🔹 Why Understanding Send Flow is Important?
Because if one component is wrong:  
❌ Email may fail  
❌ Subscriber may not receive message  
❌ Tracking may break  

👉 To debug issues, you must know the full flow.  

---

### 🔹 Step 1: Data Extension / Audience Selection
Every email send starts with selecting an audience.  
Usually from:  
- Sendable Data Extension  
- List  
- Filtered Data Extension  

📌 This contains:  
- Subscriber Key  
- Email Address  
- Personalization Data  

👉 Think of this as **“Who will receive the email?”**  

---

### 🔹 Step 2: Email Asset Selection
After audience selection, choose the email/content to send from:  
- Content Builder  
- Email Studio Template  

📌 Email may include:  
- Subject Line  
- Body Content  
- Personalization Strings  
- Dynamic Content  

👉 Think of this as **“What will be sent?”**  

---

### 🔹 Step 3: Send Classification
Defines the sending behavior.  
Includes:  
- Sender Profile  
- Delivery Profile  
- CAN-SPAM Classification  

📌 Controls:  
- From Name  
- From Email Address  
- Reply Mail Management  

👉 Think of this as **“How the email is sent”**  

---

### 🔹 Step 4: Publication List Check
Before sending, SFMC checks Publication List / Subscription Status.  

**Purpose:**  
- Ensure subscriber is opted-in  
- Validate communication preference  

📌 Example:  
Subscriber wants:  
✔ Promotions  
❌ Newsletter  
👉 Only eligible publication emails are sent.  

---

### 🔹 Step 5: Unsubscribe Validation
SFMC checks:  
- Has subscriber unsubscribed?  
- Is subscriber in All Subscribers as Unsubscribed/Held?  

📌 If YES:  
❌ Email blocked automatically  
👉 Protects compliance rules.  

---

### 🔹 Step 6: Send Processing / Personalization
Before final send, SFMC processes:  
- AMPscript  
- Personalization Strings  
- Dynamic Content Rules  

📌 Example:  
“Hi %%FirstName%%” → System replaces placeholder with actual data.  

---

### 🔹 Step 7: Delivery to Subscriber Inbox
After validations, email is delivered to subscriber mailbox.  

📌 Final delivery depends on:  
- ISP filters  
- Spam score  
- Domain reputation  

---

### 🔹 Step 8: Tracking & Reporting
Once email is sent, SFMC tracks:  
- Opens  
- Clicks  
- Bounces  
- Unsubscribes  

👉 Used in Analytics Builder / Tracking Reports  

---

### 🔄 Complete Flow Summary
**DE → Email Asset → Send Classification → Publication Check → Unsubscribe Validation → Processing → Delivery → Tracking**  

---

### 💡 Key Takeaway
SFMC Email Send is not just **“Click Send”**  

👉 It follows a complete backend validation process before delivery.  

Understanding this helps in:  
✔ Better Debugging  
✔ Better Configuration  
✔ Better Interview Knowledge  

---

📌 Follow along as I simplify SFMC step by step 👇

<img width="1216" height="1294" alt="12" src="https://github.com/user-attachments/assets/a64b20ed-567a-4703-b638-ac92bc9d749e" />
