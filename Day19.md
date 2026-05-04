# 📅 Day 19 – SFMC Learning Series | Learn with Me

## ⚠️ Common Automation Failures & How to Fix Them

Automation Studio is powerful — but in real projects, failures are very common.  
The key skill is not just building automation, but **debugging it efficiently**.  

---

### 🚨 1. File Not Found Error (File Drop / Import)
🔍 **Cause:**  
- File not available on FTP  
- Incorrect file name or pattern  
- File not placed in correct folder (Import folder)  

✅ **Fix:**  
- Verify file path: `/Import/filename.csv`  
- Check naming convention (case-sensitive)  
- Ensure file is uploaded before automation runs  

---

### 🚨 2. Import Activity Failed
🔍 **Cause:**  
- Column mismatch between file & Data Extension  
- Data type issues (Text vs Number)  
- Required field missing  

✅ **Fix:**  
- Match column names exactly  
- Validate data types in DE  
- Use Header Row option correctly  

---

### 🚨 3. SQL Query Activity Error
🔍 **Cause:**  
- Ambiguous column names (e.g., `PatientID`)  
- Missing required fields in Target DE  
- Syntax errors in query  

✅ **Fix:**  
- Use alias: `p.PatientID`  
- Ensure all required fields are selected  
- Test query in Query Studio before automation  

---

### 🚨 4. Automation Not Starting
🔍 **Cause:**  
- Start date/time is in past  
- Automation is inactive  
- Schedule not configured properly  

✅ **Fix:**  
- Set future start date/time  
- Activate automation manually  
- Recheck schedule settings (Recurring / File Drop)  

---

### 🚨 5. Email Send Failure
🔍 **Cause:**  
- Missing Send Classification  
- Suppression list blocking audience  
- Invalid email addresses  

✅ **Fix:**  
- Assign correct Send Classification  
- Check suppression/exclusion lists  
- Validate email field format  

---

### 🚨 6. Data Not Updating in Target DE
🔍 **Cause:**  
- Wrong update type (Append vs Overwrite)  
- Primary Key conflict  
- Automation step failed earlier  

✅ **Fix:**  
- Choose correct action:  
  - **Overwrite** → Fresh data  
  - **Append** → Add new records  
  - **Update** → Modify existing  
- Check primary key setup  
- Validate previous activity success  

---

### 🧠 Pro Tips
✔ Always check **Activity Log** first  
✔ Use **Error Email Notifications** in automation  
✔ Test each activity individually before full workflow  
✔ Keep naming conventions clean (DE, File, Automation)  
✔ Maintain backup DEs for safety  

---

### 💡 Key Takeaway
Automation Studio = **Data + Workflow + Reliability**  
👉 Building is easy, but **debugging failures makes you project-ready**.  

---

📌 Follow along as I simplify SFMC step by step 👇

<img width="1024" height="1536" alt=" File Not Found Error" src="https://github.com/user-attachments/assets/0d3d9e0f-5dba-466b-beaf-19164d521bd1" />

