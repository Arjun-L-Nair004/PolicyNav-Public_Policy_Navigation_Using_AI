# PolicyNav — Milestone 4: Admin Command Center & User Personalization

## Overview
Milestone 4 is the final delivery of the PolicyNav project, built as part of the Infosys Springboard AI Internship. This phase graduates the application from a collection of AI-powered tools into a fully governed, production-grade SaaS platform. Two major pillars define this milestone: a powerful **Admin Command Center** for real-time analytics and platform oversight, and a **User Profile Portal** that gives every user full control over their identity and account security.

---

## 1. Admin Dashboard (Management & Analytics)

The Admin panel functions as a centralized control room, giving platform administrators the tools to govern users, analyze behavior, and extract data — all from a single dark-themed, tab-organized interface.

### User Control

The platform enforces strict Role-Based Access Control (RBAC). Admins can promote standard users to Admin status, granting full dashboard access. Accounts flagged as suspicious can be manually blocked or unlocked at any time. A permanent delete option is also available, and it safely cascades the removal across all relational tables — erasing the user's history, OTP records, and feedback entries so no orphaned data is left behind.

![image alt](https://github.com/Arjun-L-Nair/Infosys_Springboard_PolicyNav_Public-_Policy_Navigation_Using_AI/blob/b419bb24e2d816851919ff61b208a33b57f7081f/milestone4/screenshots/user_control.png)

---

### Activity Tracking

A full-platform auditing module aggregates all user interactions into a single searchable feed. Admins can filter by individual user email to inspect exact AI prompts, generated responses, tool selections, and timestamps. System-level events such as logins and profile changes appear as compact cards, while AI tool interactions expand to show the complete prompt-response pair.

![image alt](https://github.com/Arjun-L-Nair/Infosys_Springboard_PolicyNav_Public-_Policy_Navigation_Using_AI/blob/b419bb24e2d816851919ff61b208a33b57f7081f/milestone4/screenshots/system%20analysis.png)
---

### Data Visualization

Using `pandas` for data aggregation and `plotly.express` for rendering, the Analytics tab generates two interactive dark-themed charts that surface actionable business intelligence at a glance:

- **AI Feature Popularity:** A bar chart plots the total usage count of each tool — Policy Assistant, Summarizer, Translator, Knowledge Graph — so admins know exactly where users spend their time.
- **Regional Language Utilization:** A pie chart breaks down which of the seven supported NLLB languages appeared most in user sessions, quantifying the platform's accessibility impact across different demographics.

![image alt](https://github.com/Arjun-L-Nair/Infosys_Springboard_PolicyNav_Public-_Policy_Navigation_Using_AI/blob/c9ea9bf22453bb449146c78d66a7732439de87db/milestone4/screenshots/Feedback%20analysis.png)

---

### Feedback Analysis

All user-submitted text comments — from both the general platform rating form and per-AI-tool feedback submissions — are automatically pulled and merged. The `wordcloud` library renders a visual sentiment map over a dark background, letting admins spot recurring themes, popular features, and friction points without manually reading individual rows. The raw feedback records are displayed in full below the cloud, split by feedback type.

![image alt](https://github.com/Arjun-L-Nair/Infosys_Springboard_PolicyNav_Public-_Policy_Navigation_Using_AI/blob/c9ea9bf22453bb449146c78d66a7732439de87db/milestone4/screenshots/Activity%20logs.png)

---

### Data Export

For offline reporting and compliance, three one-click `.csv` download buttons are available. Each button runs a `pandas` SQL query and streams the file directly to the admin's machine — covering the full user directory (with roles and block status), the complete activity log, and the granular AI tool performance dataset.

![image alt](https://github.com/Arjun-L-Nair/Infosys_Springboard_PolicyNav_Public-_Policy_Navigation_Using_AI/blob/c9ea9bf22453bb449146c78d66a7732439de87db/milestone4/screenshots/data%20exports.png)

---

## 2. User Dashboard & Profile Personalization

Standard users now have a dedicated settings portal split across two tabs: one for identity and one for security. Every change is validated server-side, logged to the activity table, and reflected in the UI immediately.

### Security Settings

- **Email Update:** The workflow requires the user to first confirm their current password, then sends a 6-digit OTP to the newly requested address. Only after successful OTP verification is the email swapped — and the update cascades across all relational tables so no history or feedback record is orphaned. The user is automatically logged out to force a clean re-authentication.
- **Password Change:** Requires the current password as verification. A live inline validator checks four criteria as the user types — minimum length, uppercase presence, numeric character, and special character — using colour-coded indicators. Once the new password is saved, the session is wiped and the user is redirected to the login screen.

![image alt](https://github.com/Arjun-L-Nair/Infosys_Springboard_PolicyNav_Public-_Policy_Navigation_Using_AI/blob/c9ea9bf22453bb449146c78d66a7732439de87db/milestone4/screenshots/user%20profile%201.png)

---

### Identity & Avatar Personalization

Users can upload a custom profile photo (PNG or JPG, capped at 5MB) without needing any external cloud storage integration. The image is read as bytes, encoded into a Base64 string, and stored directly in the SQLite `users` table. On the next render, the string is decoded and injected into the sidebar as a circular `<img>` element, instantly replacing the default placeholder. The 5MB cap is enforced on the backend before encoding begins.

![image alt](https://github.com/Arjun-L-Nair/Infosys_Springboard_PolicyNav_Public-_Policy_Navigation_Using_AI/blob/c9ea9bf22453bb449146c78d66a7732439de87db/milestone4/screenshots/user%20profile%202.png)

---

## Technology Stack

| Layer | Libraries & Tools |
|---|---|
| **Frontend UI** | Streamlit, Custom HTML/CSS, Native SVG Injection |
| **Analytics & Visualization** | Pandas, Plotly Express, Matplotlib, WordCloud |
| **Database** | SQLite (Users, Roles, Activity, Feedback, Base64 Avatars) |
| **Security** | bcrypt, hmac, hashlib, smtplib (SMTP), PyJWT, Base64 |
| **AI & Machine Learning** | HuggingFace Transformers (`google/flan-t5-base`), `facebook/nllb-200-distilled-600M`, Sentence-Transformers (`all-MiniLM-L6-v2`), FAISS |
| **NLP & Knowledge Graph** | spaCy, NetworkX, Pyvis |
| **Document Processing** | PyPDF, textstat, Wikipedia API |
| **Deployment** | Google Colab (T4 GPU), Pyngrok |

---

## How to Run (Google Colab)

The FAISS vector index, serialized chunks, and SQLite database are all persisted on Google Drive — no re-processing of PDFs is required on subsequent runs.

1. **Mount Google Drive** to access `policy_vector_db.index`, `chunks.pkl`, and `users.db`.
2. **Install dependencies:**
   ```bash
   pip install streamlit pyjwt bcrypt pyngrok plotly textstat transformers \
   sentence-transformers faiss-cpu spacy pandas matplotlib wordcloud \
   pyvis networkx duckduckgo_search pypdf
   python -m spacy download en_core_web_sm
   ```
3. **Set Colab Secrets** (`🔑` panel):

   | Key | Value |
   |---|---|
   | `EMAIL_ID` | Your Gmail address |
   | `EMAIL_APP_PASSWORD` | Gmail App Password (16 chars) |
   | `NGROK_AUTHTOKEN` | Your Ngrok auth token |

4. Run the final deployment cell — it kills stale Streamlit/Ngrok processes, starts a fresh tunnel, and prints the public URL.

> The first run takes 10–15 minutes to download models. Subsequent runs load from Drive in ~2 minutes.

---

## Team Contributions

This platform was built collaboratively as part of the Infosys Springboard Internship. Below is the breakdown of responsibilities and contributions for Milestone 4:

**Mainuddeen**
- Focus: Admin Dashboard Architecture & User Management
- Led the development of the Admin Command Center. Engineered the Role-Based Access Control (RBAC), implemented the soft-delete data anonymization logic, and built the account locking/unlocking mechanisms for user control.

**Srideepalakshmi**
- Focus: Admin Analytics & Data Visualization
- Collaborated heavily on the Admin panel. Integrated `pandas` and `plotly.express` to build the real-time interactive charts tracking AI feature popularity and regional language utilization.

**Arjun L Nair**
- Focus: Admin Activity Tracking & Data Export
- Worked on the Admin Dashboard by developing the searchable Global Activity Logs system and engineering the 1-click `.csv` data export buttons for offline reporting.

**Bhuvaneshwar Reddy Mandadapu**
- Focus: User Security Settings
- Developed the user settings portal. Focused on the secure email update workflow, integrating the new OTP verification email logic and ensuring automatic session logouts for enhanced security.

**Shambhavi Jha**
- Focus: User Profile Identity & UI/UX
- Implemented the user personalization features. Engineered the secure 5MB Avatar (DP) upload system using Base64 database storage, built the live password strength validation UI, and refined application styling.
