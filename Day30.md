# 📅 Day 30 – SFMC Learning Series | Learn With Me

## 🛫 End-to-End SFMC Project

👉 From learning → to building a **real-world system**  
After 30 days, here’s a complete Salesforce Marketing Cloud project built like a real enterprise implementation 🚀  

---

### 🧩 Business Case: Airline Customer Engagement System ✈️
A complete marketing system for an airline brand:  
👉 Booking confirmation  
👉 Pre-travel reminders  
👉 Upsell (seat, baggage, meals)  
👉 Post-travel feedback  
👉 Inactive customer re-engagement  

---

### 🗂️ Data Model (Contact Builder Design)
**Core Data Extensions:**  
- **Customer Master DE**  
  - CustomerID (PK)  
  - Email, Phone  
  - LoyaltyTier, Points  

- **Booking DE**  
  - BookingID (PK)  
  - CustomerID (FK)  
  - Flight Details  

- **Engagement DE**  
  - Opens, Clicks, Last Activity  

💡 **Relationship:**  
👉 1 Customer → Multiple Bookings  

---

### ⚙️ Automation Flow (Automation Studio)
📥 **FTP → File Transfer → Import → SQL → Extract**  

**Process:**  
- Import daily booking data  
- Transform using SQL (join customer + booking)  
- Segment:  
  - Upcoming travelers  
  - Frequent flyers  
  - Inactive users  
- Push to Journey Entry DE  

💡 Includes:  
✔ Error handling  
✔ Data validation  
✔ Scheduled automation  

---

### 🔁 Journey Flow (Journey Builder)

**Journey 1: Booking Lifecycle**  
Entry → Email (Confirmation) → Wait → Upsell Email → Wait → Reminder Email → Exit  

**Journey 2: Re-engagement**  
Entry (Inactive Users) → Email 1 → Wait → Email 2 → Decision Split → Exit / Suppress  

---

### 📩 Email Strategy (What Makes It Powerful)
👉 Personalization using **AMPscript**  
👉 Dynamic content based on:  
- Loyalty Tier  
- Travel Class  

**Examples:**  
- “Upgrade to Business Class” for premium users  
- Discount offers for inactive users  

💡 Triggered emails for **real-time communication**  

---

### 🧠 What This Project Demonstrates
✔ End-to-end SFMC architecture  
✔ Data modeling & segmentation  
✔ Automation + Journey integration  
✔ Real-world use cases  

---

### 🚀 Why This Matters
This is not just a project — it’s a **complete portfolio asset**.  

👉 Use it for:  
- Interviews (explain full flow)  
- Resume projects section  
- LinkedIn Featured section  

---

### 💬 Final Thought
From basics to advanced — this **30-day journey built real skills**.  
Now it’s time to **apply, build, and grow 💼**  

🔁 If you followed this series, comment **“DONE”**  
💡 Let’s connect and grow together  

<img width="1024" height="1536" alt="Day 30 - End-to-End SFMC Project (Showcase)" src="https://github.com/user-attachments/assets/df3bf71e-d68e-4edc-aed1-4c27a9851b1b" />
