Project 5 — Lead Collection System
Week: 2 — Day 12

Date: 2026-06-12

Tools: Zapier, Google Forms, Google Sheets, Gmail

Status: ✅ Completed

Time to build: 33 minutes

What This Project Does
This automation creates a complete lead collection system for any small business. When a potential customer submits their name, email, and problem through a Google Form — Zapier instantly saves their information to a Google Sheet and sends them a personalized professional welcome email through Gmail. The entire process happens automatically within seconds of form submission with zero manual work required.
This is one of the most practical and sellable automation services a freelancer can offer to small businesses.

Real World Use Case
Every small business has the same problem. Potential customers fill out a contact form on their website. The business owner checks it manually every few hours. By the time they respond the lead has already contacted a competitor.
With this lead collection system:

Every lead is captured instantly in a Google Sheet
Every lead receives a professional welcome email within seconds
The business owner has a complete organized database of all leads
Response time drops from hours to seconds
Zero leads are ever missed or forgotten

This system is used by:

Small business owners collecting customer inquiries
Freelancers managing client requests
Coaches collecting consultation requests
Real estate agents collecting property inquiries
Clinics collecting patient appointment requests

Every single one of these is a potential client who will pay for this service in Month 3.

Tools Used
ToolPurposeGoogle FormsCollects lead information — Name, Email, ProblemZapierAutomation engine connecting all apps togetherGoogle SheetsStores all lead data in organized databaseGmailSends personalized welcome email to each lead

How It Works — The Logic
Lead submits Google Form with Name, Email, Problem
                    ↓
Zapier detects new form response instantly
                    ↓
Action 1: Adds lead data as new row in Google Sheets
                    ↓
Action 2: Sends personalized welcome email via Gmail
This follows three step automation logic:

Trigger → Data Storage → Automated Communication

Step by Step Build Process
Step 1 — Create the Google Form

Created Google Form with three fields:

Full Name — Short answer
Email Address — Short answer with email validation enabled
Describe your problem or need — Paragraph answer



Important lesson about email validation:

Originally added email as a simple short answer field. Discovered that without validation someone could type random text instead of a real email address. This would cause Zapier to fail when trying to send the welcome email.
Fixed by:

Clicking the email question
Clicking three dots menu at bottom right
Selecting Response Validation
Selecting Text → Email address
This forces Google Forms to only accept valid email format

This step wasted some time during the build but taught an important lesson — always validate data at the input stage before it enters your automation. Bad input breaks good automations.
Step 2 — Create New Zap

Opened Zapier → clicked "Create Zap"
Named the Zap: Lead Collection System

Step 3 — Set Up Trigger

Searched: Google Forms
Selected: "New Response in Spreadsheet"
Connected Google account
Selected the Lead Collection form
Clicked "Test Trigger"
Confirmed all three fields detected correctly — Name, Email, Problem
Clicked "Continue"

Step 4 — Add Google Sheets Action

Clicked "+" to add first action
Searched: Google Sheets
Selected: "Create Spreadsheet Row"
Created new spreadsheet named "Lead Collection"
Added headers in Row 1:

Column A — Name
Column B — Email
Column C — Problem
Column D — Date


Mapped fields:

Column A → Full Name from Google Form
Column B → Email Address from Google Form
Column C → Problem from Google Form
Column D → Timestamp from form submission


Clicked "Test Action"
Row appeared in Google Sheet with all four columns filled correctly

Step 5 — Add Gmail Action

Clicked "+" to add second action
Searched: Gmail
Selected: "Send Email"
Connected Gmail account
Configured email fields:

To: clicked "+" → selected Email Address field from Google Form — makes every email go to the actual lead's email address dynamically
Subject: Thank you for reaching out — we received your message
Body: personalized welcome message using lead's name and problem from form



Welcome email body written:
Hi (Name from form),

Thank you for contacting us. We have received your 
message and will get back to you within 24 hours.

Here is a summary of what you submitted:
Problem: (Problem field from form)

We look forward to helping you.

Best regards,
Safdar

Clicked "Test Action"
Welcome email arrived in Gmail inbox within seconds
Lead's name and problem appeared correctly in the email body

Step 6 — Publish and Live Test

Clicked "Publish Zap"
Submitted Google Form twice with different test leads:

Test Lead 1:

Name: Safdar Ali
Problem: Want to automate customer inquiry system for small business

Test Lead 2:

Name: Ahmed Khan
Problem: Spending 2 hours daily sending manual confirmation emails to customers

Results for both tests:

✅ Row added to Google Sheet instantly
✅ Personalized welcome email received within seconds
✅ Zero errors on both live tests
✅ Automation confirmed working perfectly


Challenges Faced and How I Solved Them
Challenge — Email Validation Setup

When first creating the Google Form I added email as a simple short answer field without any validation. Realized this was a problem because anyone could type invalid text instead of a real email address causing the automation to break.
Spent time figuring out how to add email validation inside Google Forms. Solution was: three dots menu on the email question → Response Validation → Text → Email address. This forces the form to only accept properly formatted email addresses before submission.
Lesson learned: Always validate data at the input stage. A small extra step during form creation saves the entire automation from breaking later.

What I Learned
Technical lessons:

How to build a complete three step automation — Form → Database → Email
How to add email validation in Google Forms to ensure data quality
How to use dynamic field mapping so every lead receives a personalized email
How to create and organize a lead database in Google Sheets
How to write professional automated welcome emails that feel personal

Business lessons:

This exact system is what small businesses desperately need
Most small businesses lose leads because of slow manual response times
An automated lead collection system solves a real painful problem
This is a service I can sell to restaurants, clinics, coaches, and ecommerce stores starting Month 3
Pricing for this service in the freelance market ranges from $100 to $500 depending on complexity

Progress comparison:

Project 1 — needed full step by step guidance
Project 3 — 30 minutes, zero errors
Project 4 — 53 minutes, solved errors independently
Project 5 — 33 minutes, solved email validation independently
Speed and confidence are both increasing with every project


Key Concepts Demonstrated
Lead Generation Automation — automatically capturing and storing potential customer information without manual work
Dynamic Email Personalization — using form field mapping to insert the lead's actual name and problem into every email automatically
Data Validation — ensuring only correctly formatted data enters the automation system
Multi-step Zap — connecting three apps in one automation workflow with one trigger and two actions
Real Business Value — this automation directly solves the problem of slow lead response time which costs businesses real money every day

Screenshot
(See screenshot files in this folder)

Next Project
Project 6 — Automated Task Reminder

Google Sheet with tasks and due dates → Zapier checks daily → sends Gmail reminders automatically.

This project is part of my AI Skills Journey — a 30-day structured learning plan building real automation skills from zero.
GitHub: github.com/safdar1234k/AI-Skills-Journey
