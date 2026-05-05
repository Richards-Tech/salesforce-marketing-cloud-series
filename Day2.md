# 📅 Day 2 – SFMC Learning Series | Learn with Me

## 🧩 Understanding Data Extension Types in SFMC (Sendable vs Non-Sendable)

When I started working on Salesforce Marketing Cloud, this was one of the most confusing concepts for me — but it’s actually very important in real projects 👇

---

### 🔹 1. Sendable Data Extension (📩 Used for Email Sends)
A Sendable Data Extension is a data table that is configured to send emails (or messages) to contacts.  
It must be linked to a subscriber record using a unique identifier.  
A Sendable Data Extension is required when you want to send emails or trigger journeys.

✔ **Must include:**
- Subscriber Key / Contact Key  
- Channel address (Email Address for email sends)  
- Mapping to the All Subscribers list  

✔ **Why it matters:**
SFMC needs to know:  
👉 Who is the user?  
👉 Where should the email be sent?  

💼 **Real Example:**
In one of my projects, I used a Sendable DE like:  
- CustomerID  
- EmailAddress  
- FirstName  
- BookingStatus  

This was used in Journey Builder to send:  
- Booking confirmation emails  
- Reminder emails  

---

### 🔹 2. Non-Sendable Data Extension (📊 Data Storage Only)
A Non-Sendable Data Extension is a data table used only for storing data, and cannot be used directly for sending messages.  
This type is used only to store data, not to send emails directly.

✔ **Characteristics:**
- No need for Email Address  
- Can store large structured data  

💼 **Real Example:**
- Flight_Bookings  
- Purchase_History  
- Website_Activity  

These DEs store data like:  
- Booking IDs  
- Travel dates  
- User actions  

---

### 🔄 How They Work Together
👉 Non-Sendable DE stores raw data  
👉 Sendable DE is prepared using SQL / filtering  

---

### 💡 Key Takeaway
✔ **Sendable DE** = Required for sending emails  
✔ **Non-Sendable DE** = Used for backend data storage  
✔ **Best practice** = Use both together for scalable design  

---

### 💬 My Learning
Initially I tried using only one DE for everything, but in real scenarios, separating data and audience makes the system clean, scalable, and easy to manage.

---

📌 Follow along as I break down SFMC concepts in a simple, practical way 👇

<img width="1536" height="1024" alt="Copilot_20260505_095435" src="https://github.com/user-attachments/assets/e529df28-4a6e-4391-ae17-e661fb5f521c" />

