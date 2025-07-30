# Appliq – AI Resume Analyzer

**Appliq** is a serverless AI-powered resume analyzer that helps job seekers understand how their resume performs against Applicant Tracking Systems (ATS) and where it can be improved. Upload your resume, get instant feedback, and optimize your application for better chances.

---

## 📌 Why Appliq?

In today’s job market, it's common to send out dozens of applications and hear nothing back, not even a rejection. This silence isn’t always a reflection of your qualifications. More often, it's because your resume isn't optimized for the systems that screen them.

**Appliq** helps close that gap by giving you clear, AI-generated insights into what recruiters and ATS systems are (and aren't) seeing.

---

## 🔍 Features

- **PDF Resume Uploads** – Easily drag & drop or upload your resume
- **Instant Previews** – View your resume image snapshot directly in-app
- **AI Feedback Engine** – Get automated, categorized feedback on:
  - ATS readability
  - Content quality
  - Tone and style
  - Skills and structure
- **Scoring Dashboard** – Visual scores with helpful tips and improvement areas
- **Modern, serverless tech** – No backend setup required

---

## ⚙️ Tech Stack

- **Frontend:** React + TypeScript
- **Styling:** TailwindCSS
- **Routing:** React Router v7
- **State Management:** Zustand
- **Tooling:** Vite
- **Storage & Auth:** [Puter.com](https://puter.com) APIs (file storage, auth, KV database, AI access)

---

## 🚀 Getting Started

### 1. Clone the project

[https://github.com/Genia89/ai-resume-analyzer](https://github.com/Genia89/ai-resume-analyzer)

```bash
    git clone https://github.com/Genia89/ai-resume-analyzer
```

### 2. Install dependencies

``` bash
    npm install
```
### 3. Start the development server
``` bash
    npm run dev
```
Your app will be available at: http://localhost:5173

## 📁 Project Structure
```
/public              → Static assets (icons, images, resumes)
/app
    ├── components     → Reusable UI elements (scoring, nav, ats, etc.)
    ├── lib            → Puter utilities
    ├── routes         → Route views (home, auth, resume, etc.)
/ constants      → Static resume and feedback config
/public     
/types     
```

## 🔒 Security & Hosting

Appliq uses [**Puter**](https://puter.com) for secure file storage, AI access, and serverless infrastructure. This means:

- No backend setup

- No database maintenance

- All data stays secure in your personal Puter environment

## 💡 Planned Enhancements
-  User accounts & saved resume history

-  AI-generated rewrite suggestions

-  Real-time resume grading

-  Resume templates for customization

-  Job description matching

## 🌐 Deployment

**Appliq** can be deployed to platforms like **Vercel**, **Netlify**, or **Railway** — but it’s designed for seamless deployment directly on [**Puter.com**](https://puter.com).

### ✅ Steps to Deploy on Puter

#### 1. Commit your changes to GitHub

```bash
  git add .
  git commit -m "ready for deploy"
  git push
```
  #### 2. Update config for static deployment
  In react-router.config.ts, ensure server-side rendering is disabled:
```
export default {
ssr: false, // Required for static HTML build
} satisfies Config;
```

#### Create the production build
``` bash
    npm run build
```

#### 4. Upload to Puter
- Go to Puter App Center

- Click “Add your app!” → “Create an App”

- Give your app a name (e.g., "Appliq – Resume Analyzer")

- Open the build/client/ folder in your file system

- Select all files inside and drag & drop them into the app folder on Puter

- Click "Deploy Now"

#### 5. Launch & Customize
- Click "Give it a try!" to open your deployed app inside your virtual computer

- Customize your app title, favicon, and name in the App Settings

- Copy your public URL (shown in settings) and share it anywhere