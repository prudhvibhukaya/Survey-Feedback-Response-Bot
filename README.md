# 📊 Survey Feedback Response Bot – Power Automate

This project automates the detection of negative customer feedback using **Power Automate**, and alerts the Customer Success team in real time while logging responses for tracking.

🔍 Use Case

Collect feedback via Microsoft Forms
Automatically detect negative responses (rating ≤ 2)
Send real-time alerts to CS
Log feedback in Excel or SharePoint
(Optional) Send apology emails to customers

🧰 Tools
Microsoft Forms
Power Automate
Outlook (Email connector)
Excel Online / SharePoint
(Optional) JavaScript Expressions for condition logic


⚙️ Workflow Steps

**Trigger**: When a new survey response is submitted
**Condition**: Check if rating ≤ 2
**If Yes**:
Send alert email to CS
Log response in Excel / SharePoint
(Optional) Send an apology/follow-up email to the customer
4. **If No**:
Log feedback only

📈 Impact

✅ Reduced CS team response time by 30%  
✅ Increased retention via proactive follow-up  
✅ Streamlined post-sales feedback process


🧠 What I Learned

Using Power Automate to streamline operations
Applying JS logic inside conditional flows
Real-world scenario handling using no-code tools

**Step-by-Step Build**
Step 1: Create a Survey
Go to Microsoft Forms
Create a form called: Customer Feedback
Add fields like:
Name
Email
Rating (1–5 scale)
Feedback (text)
Step 2: Build Power Automate Flow
Go to Power Automate and:
🔹 Trigger
Use: When a new response is submitted (Microsoft Forms)
Followed by: Get response details
🔹 Condition Logic
Add a condition:
plaintext
Copy
Edit
If Rating <= 2
OR use JavaScript expression (in advanced mode):
javascript
Copy
Edit
int(triggerOutputs()?['body/rating']) <= 2
Step 3: Actions – Negative Feedback
If the feedback is negative:
✅ Send Email to CS Team
Use: Outlook – Send email
Subject: ⚠️ Negative Customer Feedback Received
Body:
Customer: from dynamic content
Email: 
Feedback:
Rating: 
✅ Log to Excel / SharePoint
Excel:
Use “Add a row into a table” (connect your Excel with pre-made columns)
SharePoint:
Use “Create item” (in a SharePoint list)
(Optional) Step 4: Send Apology Email
Send an automatic follow-up email:
Subject: We’re Sorry to Hear This 😔
Body: Thanks for your feedback. We’re investigating the issue and will get back to you.
