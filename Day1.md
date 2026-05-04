# 📅 Day 1 – SFMC Learning Series | Learn with Me

## 📊 Understanding Data Extensions vs Lists vs Subscribers in SFMC

If you're starting with Salesforce Marketing Cloud, one of the first confusions is:

👉 **What is the difference between Data Extensions, Lists, and Subscribers?**

---

### 🔹 1. Subscribers
- A Subscriber is a unique person/contact in SFMC (who opted in to receive email).
- Identified by: **Subscriber Key / Contact Key**
- Can exist across multiple channels (Email, SMS, etc.)
- 👉 Think of it as: **One identity in the system**

---

### 🔹 2. Lists (Old Model – Limited Use)
- Lists are a basic way to store subscribers (legacy approach).
- Fixed structure
- Limited flexibility
- Mainly used for simple email sends
- 👉 Not recommended for complex use cases

---

### 🔹 3. Data Extensions (Most Important 🔥)
- Data Extensions are custom data tables in SFMC.
- Flexible structure (custom fields)
- Supports relationships (1:1, 1:N)
- Used in **Journey Builder** & **Automation Studio**
- 👉 This is what most real-world projects use

---

### 🔄 How They Connect
- **Subscriber Key** acts as the common link between:
  - Data Extensions
  - Contact Builder
  - Journey Builder

---

### 💡 Key Takeaway
If you understand **Data Extensions + Subscriber Key** properly,  
👉 SFMC becomes much easier to work with.

---

📌 Follow along as I break down SFMC concepts step by step.
