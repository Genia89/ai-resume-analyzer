# Resumind – AI Resume Analyzer

**Resumind** is an AI-powered resume analyzer that reads and scores resumes using ATS logic, offering tailored feedback to help users improve their job application success rate.

## Features

- Upload PDF resumes and preview them directly in the application
- AI-powered feedback and scoring on:
    - ATS readability
    - Content quality
    - Tone and style
    - Skills and structure
- Visual scoring with icons, color-coded sections, and actionable suggestions
- Resume snapshot preview using static image
- Built with a modern, fast, and scalable stack

## Tech Stack

- **React + TypeScript**
- **Tailwind CSS** for styling
- **Zustand** for state management
- **Vite** for fast builds and development
- **Puter.com** storage API
- **React Router v7** for routing

## Getting Started

### 1. Install dependencies

``` bash
    npm install
```
### 2. Start the development server
``` bash
    npm run dev
```
Visit the app at: http://localhost:5173

## Build for Production
``` bash
    npm run build
```
## Project Structure
```
/public             → Static assets (icons, images, resume files)
/src
  ├── components    → Reusable UI components
  ├── lib           → Zustand store and helper functions
  ├── pages         → Route views
  ├── styles        → Tailwind and global styles
  ├── constants     → Resume data and static settings
```

## Planned Features
- User accounts and persistent feedback

- AI-powered resume rewriting suggestions

- Real-time scoring and analysis

- Resume template generation and customization