🦷 Dental Files — Dental Patient Records Management System

A bilingual web application designed to help dental clinics organize patient records, access medical history, and manage patient information efficiently.

🔗 Live Demo: "Dental Files" (https://dentalpatient.lovable.app)
💻 GitHub Repository: "Dental Files Repository" (https://github.com/baraa-abuwatfa/dentalfiles.git)

---

📌 1. Project Overview

❗ Problem

Dental clinics need an organized way to manage patient records and access medical information efficiently. Manual record management can make it difficult to find patient details and review previous visits.

👥 Target Users

- Dentists
- Dental clinic staff

💡 Solution

Dental Files is a bilingual web application that helps dental clinics organize patient records, manage patient information, and access medical and dental history more easily.

---

✨ 2. Main Features

- 🗂️ Patient Records Management — Organize and manage patient information.
- 🩺 Medical & Dental History — Access patient health information and dental history.
- 🔎 Patient Search — Find patient records more efficiently.
- 📦 Patient Archiving & Restoration — Archive patient records and restore them when needed.
- 🔐 User Authentication — Support authenticated access to the application.
- 📄 PDF Reports — Generate patient reports in PDF format.
- 🌐 Bilingual Interface — Support for Arabic and English.
- 📱 Responsive Design — Designed for desktop, tablet, and mobile screens.

---

🛠️ 3. Tech Stack

Technology| Purpose
Lovable| AI-assisted web application development
Supabase| Database and authentication services
GitHub| Source code management and version control

---

🧪 4. Testing

The application was tested using positive, negative, edge-case, and data/access testing scenarios.

✅ Test 1 — Positive Testing

- Scenario: Test the main application functions using valid information and existing patient records.
- Expected Result: The application processes valid information correctly and displays the appropriate results.
- Actual Result: The tested functionality worked as expected.
- Status: ✅ Pass

❌ Test 2 — Negative Testing

- Scenario: Test the application's behavior when invalid information is entered or a requested record cannot be found.
- Expected Result: The application handles invalid input appropriately and displays a clear response.
- Actual Result: The tested scenarios behaved as expected.
- Status: ✅ Pass

⚠️ Test 3 — Edge Case Testing

- Scenario: Test authentication behavior when multiple attempts are made within a short period.
- Expected Result: The application handles repeated attempts appropriately and provides clear feedback when an authentication limit is reached.
- Actual Result: An authentication limit message appeared during testing. The issue was investigated and addressed.
- Status: ✅ Pass after the fix was verified

🔒 Test 4 — Data & Access Testing

- Scenario: Verify the tested database-related functionality and access to patient records.
- Expected Result: The application handles patient data correctly and follows the configured access rules.
- Actual Result: The tested scenarios passed.
- Status: ✅ Pass

---

🐞 5. Bugs Found

Bug 1 — Authentication Attempt Limit

Error Message:

Too many attempts — please wait a few minutes and try again.

Description:

During testing, an authentication limit was triggered after repeated attempts. This temporarily prevented further authentication attempts and interrupted the testing process.

Impact:

- Temporary difficulty signing in.
- Interrupted authentication testing.
- Reduced usability during repeated attempts.

---

🔧 6. Fixes & Retesting

Fix 1 — Authentication Limit Issue

Actions Taken:

- Investigated the authentication limit and relevant Supabase configuration.
- Addressed the identified authentication issue.
- Retested the affected authentication flow.
- Verified the relevant test scenarios after the fix.

Status: ✅ Resolved and retested

---

📸 7. Testing Evidence

Screenshots can be added here to document the application and testing process.

Evidence| Description
🖥️ Dashboard| Main dashboard and patient records
🩺 Patient Details| Patient information and medical history
🔐 Authentication| Login and authentication interface
🐞 Bug Evidence| Authentication limit error message
🔧 Retesting| Authentication behavior after the fix
🧪 Test Results| Screenshots showing test execution and results

<!-- Add your screenshots below using Markdown image syntax:
![Dashboard](screenshots/dashboard.png)
![Authentication Error](screenshots/auth-error.png)
-->---

🔗 8. Project Links

- 🌐 Live Application: https://dentalpatient.lovable.app
- 💻 GitHub Repository: https://github.com/baraa-abuwatfa/dentalfiles.git

---

👩‍💻 9. Project Focus

This project demonstrates practical experience in:

- AI-assisted web application development.
- Database integration using Supabase.
- Software testing and test scenario design.
- Bug identification, documentation, and retesting.
- Authentication testing and issue resolution.
- Responsive and bilingual application design.

---

Dental Files — Organizing patient records for a more efficient dental care experience.
