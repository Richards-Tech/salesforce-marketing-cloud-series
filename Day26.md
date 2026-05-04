# 📅 Day 26 – SFMC Learning Series | Learn With Me

## 🎯 Email Personalization Strategies

From **basic personalization → real-time, behavior-driven experiences** in Salesforce Marketing Cloud.  

---

### 🚀 Why This Topic Matters
Most beginners stop at:  
👉 “Hi %%FirstName%%” ❌  

But real-world personalization is:  
✔ Context-aware  
✔ Behavior-driven  
✔ Dynamic at send-time  

---

### 📌 1. AMPscript vs Personalization Strings

#### 🔹 Personalization Strings (Basic Layer)
- Simple merge fields  
- Easy to use  

**Example:**  
`Hi %%FirstName%%,`  

👉 **Use When:**  
- Static data  
- No logic needed  

---

#### 🔹 AMPscript (Advanced Layer)
- Server-side scripting  
- Enables logic + conditions + lookups  

**Example:**  
```ampscript
%%[
IF [LoyaltyTier] == "Gold" THEN
  SET @msg = "Exclusive Gold Offer!"
ELSE
  SET @msg = "Check our latest deals!"
ENDIF
]%%
%%=v(@msg)=%%
```

👉 **Use When:**  
- Conditional logic  
- Data Extensions lookup  
- Real-time personalization  

---

### 📌 2. Dynamic Content Rules
👉 Show different content blocks based on rules  

**Example:**  
- If City = Mumbai → Show Mumbai offer  
- If City = Pune → Show Pune banner  

👉 Built using: **Rule Builder (UI-based)**  
No coding required  

---

### 📌 3. Conditional Content (More Control)
👉 Similar to dynamic content but more flexible via AMPscript  

**Example:**  
```ampscript
%%[ 
IF [PointsBalance] > 5000 THEN 
]%%
  🎁 Premium Rewards Available
%%[ ELSE ]%%
  👉 Earn more points to unlock rewards!
%%[ ENDIF ]%%
```

👉 **Use When:**  
- Complex segmentation  
- Multiple conditions  

---

### 📌 4. Behavior-Based Personalization (Advanced)
👉 Personalization based on **user actions**  

🔥 **Examples:**  
- Last purchase category  
- Email engagement (`_Open`, `_Click` data views)  
- Website activity (via tracking)  

👉 **Real Use Cases:**  
- Show “Continue Shopping” if cart abandoned  
- Recommend products based on last purchase  
- Send re-engagement offers to inactive users  

---

### 🎯 Real Scenario
Case: Show different banners based on **Loyalty Tier**  

**Logic:**  
- Gold → Premium Offer Banner  
- Silver → Mid-tier Discount  
- Basic → Entry-level Offer  

**AMPscript Example:**  
```ampscript
%%[
IF [LoyaltyTier] == "Gold" THEN
]%%
  <img src="gold_offer.jpg">
%%[ ELSEIF [LoyaltyTier] == "Silver" THEN ]%%
  <img src="silver_offer.jpg">
%%[ ELSE ]%%
  <img src="basic_offer.jpg">
%%[ ENDIF ]%%
```

👉 This is **real personalization** used in production  

---

### 🧠 Pro Strategy
✔ Combine **Data + Behavior + Context**  
✔ Avoid over-personalization (can feel creepy)  
✔ Always have fallback content  
✔ Test every condition path  
✔ Use **Data Views** for smarter targeting  

---

### 🚨 Common Mistakes
❌ Only using First Name personalization  
❌ Missing fallback values (NULL issues)  
❌ Hardcoding instead of dynamic logic  
❌ Ignoring testing scenarios  

---

### 💬 Question
👉 What happens if **LoyaltyTier** is NULL in your AMPscript logic?  
How will you handle fallback?  

---

### 🚀 Final Insight
👉 **Basic personalization = Data insertion**  
👉 **Advanced personalization = Decision engine**  

---

📌 Follow along as I simplify SFMC step by step 👇

<img width="1024" height="1536" alt="DAY EMAIL PERSONALIZATION" src="https://github.com/user-attachments/assets/25adb8ed-c0c6-4383-a948-99e05964bc7a" />
