# 📊 Survey Feedback Response Bot – Power Automate

This project automates the detection of negative customer feedback using **Power Automate**, and alerts the Customer Success team in real time while logging responses for tracking.

🔍 Use Case

Collect feedback via Microsoft Forms
Automatically detect negative responses (rating ≤ 2)
Send real-time alerts to CS
Log feedback in Excel or SharePoint
(Optional) Send apology emails to customers

🧰 Tools & Technologies
Microsoft Forms
Power Automate
Outlook (Email connector)
Excel Online / SharePoint
(Optional) JavaScript Expressions for condition logic


⚙️ Workflow Steps

**Trigger**: When new survey response is submitted
**Condition**: Check if rating ≤ 2
**If Yes**:
Send alert email to CS
Log response in Excel / SharePoint
(Optional) Send apology/follow-up email to customer
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
