SkillBridge: Find Your Perfect Internship
SkillBridge is an internship discovery platform designed to bridge the gap between student aspirations and real opportunities across India. It offers personalized internship recommendations and a clean, mobile-responsive user interface.

🌟 Key Features
Personalized Internship Recommendations: Matches opportunities to a user's skills and preferences.

Multi-language Support: Includes translations for English, Hindi (hi), and Tamil (ta), and Bengali (bn) for broad accessibility across India.

Phone Authentication Flow: Implements a sign-in/sign-up process using Indian phone number validation and a 6-digit OTP structure (simulated in the provided code).

Responsive Design: Uses a modern layout with dedicated mobile navigation (sidebar menu).

📁 Project Structure (Frontend Focus)
The repository appears to be a pure HTML/CSS/JavaScript frontend application focused on user experience and authentication flow.

File	Description	Status
index.html	The main landing page, featuring a hero section and featured internships.	Complete
about.html	Details the mission, vision, values, team, and impact of the platform.	Complete
internships.html	The main internship browsing page, including search and filtering options (Location, Sector, Category, Type, Duration).	Complete
contact.html	Provides a contact form and company contact information.	Complete
userlogin.html	The primary page for user sign-in and sign-up using the phone/OTP flow.	Conflicted / In Progress
languages.js	The core JavaScript object defining all translation strings (en, hi, ta, bn).	Complete
loginuser.js	Contains all logic for phone authentication, OTP handling, timers, form validation, and successful sign-in/up simulation.	Merge Conflict
login.css	Styling for the userlogin.html page, including responsive and animation details.	Complete
styles.css	General CSS stylesheet for the rest of the site (implied from HTML).	N/A
hero-image.jpg	Image used for the main landing page hero section.	Complete
favicon.ico	Site favicon icon.	Complete

Export to Sheets
🛠️ Setup and Installation
This project is a static site and does not require a backend server for initial setup.

Clone the Repository:

Bash

git clone https://github.com/Ayush-delta/SkillBridge.git
cd SkillBridge
Resolve Conflicts (Critical):

Before proceeding, ensure all merge conflicts (e.g., in userlogin.html and loginuser.js) are resolved.

Manually choose the correct code blocks for each conflict (e.g., <<<<<<< HEAD vs. >>>>>>> remote_hash).

Open in Browser:

Simply open index.html in your preferred web browser to view the application.

⚙️ Development Notes (Authentication)
The loginuser.js file handles the entire authentication flow:

Navigation: showSignIn() and showSignUp() manage page visibility.

Validation: Uses validateIndianPhoneNumber() (10 digits, starting with 6-9).

OTP Handling: The setupOtpInputs() function provides logic for automatic focusing between OTP boxes and paste functionality.

Simulation: OTP sending, verification, and account creation are simulated using console.log() and setTimeout() and should be replaced with actual API calls in a production environment.

🆘 Merge Conflict Status
The repository is currently paused due to an uncommitted merge and unresolved conflicts, which is blocking the final push.

File	Conflict Type	Resolution
userlogin.html	HTML Structure / Text	Needs manual review in VS Code to accept or combine changes.
languages.js	Language Options	Appears to be adding/removing language options in the dropdown.
loginuser.js	JavaScript Logic	Appears to have two different versions of the signUpForm handler logic.
