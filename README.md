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

## 🛠️ Setup Notes & Developer Tools

### Vite

This project uses [**Vite**](https://vite.dev), a fast build tool and dev server for modern frontend projects.

To create a new project with Vite, run:

```bash
    npm create vite@latest .
```
📝 The dot . at the end is important it installs the app into the current folder, and not adding a new folder.

### Puter.com Account
Appliq uses Puter.js for secure file storage, AI access, auth, and infinite scalability without any backend.

✅ Be sure to create a free account on [Puter](https://puter.com) before you start, since you’ll need API access and a virtual computer to deploy and test.
To use the app’s AI features (like resume upload, feedback, and scoring), a free [Puter.com](https://puter.com) account is required.
> 🧠 **Note:** A Puter account is also required to run the app itself — not just for developers!  
> Users need to log in with Puter to upload and analyze resumes using AI.

### AI Code Assistant: Junie AI Plugin
For smoother development, this project also used Junie AI, a JetBrains plugin that acts as your AI pair programmer.

💡 Highly recommended it improves productivity, offers code suggestions, refactoring help, and even generates components.

To install it:

1. Open your JetBrains IDE (like WebStorm)

2. Go to Plugins → Search for “Junie AI”

3. Install and restart the IDE

### Built With WebStorm
This app was built using WebStorm by JetBrains IDE for modern JavaScript and TypeScript development.

🧠 The combination of WebStorm + Junie AI + Vite makes development incredibly fast and enjoyable.


## 🚀 Getting Started

### 1. Clone the project

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
/constants      → Static resume and feedback config
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
  git commit -m "add your message"
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