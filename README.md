# SkillBridge: Find Your Perfect Internship  

https://ayush-delta.github.io/Recommendation-System/

SkillBridge is an internship discovery platform designed to bridge the gap between student aspirations and real opportunities across India. It offers personalized internship recommendations, multilingual support, and a clean, mobile-responsive user interface.  

---

## 🌟 Key Features  

- **Personalized Internship Recommendations**  
  Matches opportunities to a user’s skills and preferences.  

- **Multi-language Support**  
  Includes translations for **English (en)**, **Hindi (hi)**, **Tamil (ta)**, and **Bengali (bn)** for broad accessibility across India.  

- **Phone Authentication Flow**  
  Implements sign-in/sign-up using **Indian phone number validation** and a **6-digit OTP structure** (simulated in the code).  

- **Responsive Design**  
  Modern layout with dedicated mobile navigation (sidebar menu).  

---

## 📁 Project Structure (Frontend Focus)  

| File             | Description                                                                 | Status             |
|------------------|-----------------------------------------------------------------------------|--------------------|
| `index.html`     | Landing page with hero section and featured internships.                   | ✅ Complete        |
| `about.html`     | Mission, vision, values, team, and impact details.                         | ✅ Complete        |
| `internships.html` | Main internship browsing page with search and filtering.                 | ✅ Complete        |
| `contact.html`   | Contact form and company information.                                      | ✅ Complete        |
| `userlogin.html` | User sign-in/sign-up (phone/OTP flow).                                     | ⚠️ In Progress / Conflicted |
| `languages.js`   | Defines translation strings (en, hi, ta, bn).                              | ✅ Complete        |
| `loginuser.js`   | Handles phone authentication, OTP, validation, and simulation.             | ⚠️ Merge Conflict |
| `login.css`      | Styling for login page (responsive + animations).                          | ✅ Complete        |
| `styles.css`     | General stylesheet for rest of the site.                                   | ✅ Complete        |
| `hero-image.jpg` | Hero image used on landing page.                                           | ✅ Complete        |
| `favicon.ico`    | Website favicon.                                                           | ✅ Complete        |

---

## 🛠️ Setup & Installation  

This is a **static frontend project**, so no backend setup is required.  

### Clone Repository  
```bash
git clone https://github.com/Ayush-delta/SkillBridge.git
cd SkillBridge
```

### Resolve Merge Conflicts (⚠️ Critical)  
Before proceeding, resolve conflicts in:  
- `userlogin.html` (HTML structure / text differences)  
- `languages.js` (language dropdown updates)  
- `loginuser.js` (signUpForm logic differences)  

In **VS Code**, search for conflict markers:  
```
<<<<<<< HEAD
...your code...
=======
...incoming code...
>>>>>>> branch
```
Manually choose or merge the correct logic.  

### Run Project  
Simply open `index.html` in your web browser.  

---

## ⚙️ Development Notes (Authentication Flow)  

- **Navigation**:  
  `showSignIn()` and `showSignUp()` toggle visibility between login forms.  

- **Validation**:  
  `validateIndianPhoneNumber()` ensures numbers are **10 digits** and start with **6–9**.  

- **OTP Handling**:  
  `setupOtpInputs()` handles **auto-focus between input boxes** and **paste functionality**.  

- **Simulation**:  
  OTP sending, verification, and account creation are **simulated** with `console.log()` + `setTimeout()`.  
  👉 Replace with **real API calls** in production.  

---

## 🆘 Merge Conflict Status  

| File             | Conflict Type               | Resolution Needed |
|------------------|-----------------------------|------------------|
| `userlogin.html` | HTML structure & text        | Manual merge      |
| `languages.js`   | Language dropdown updates    | Confirm changes   |
| `loginuser.js`   | Sign-up logic differences    | Decide correct flow |

---

## 🚀 Future Enhancements  

- ✅ Backend integration for **real OTP authentication**.  
- ✅ Database support for saving **user preferences** & **internship applications**.  
- ✅ AI-powered recommendations for **personalized matches**.  

---

## 📌 License  

This project is open-source and available under the **MIT License**.  

---
