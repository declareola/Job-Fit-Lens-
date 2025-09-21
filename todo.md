# ✅ Job Application Assistant – To-Do

This file captures every step needed to build the Chrome Extension. Update as tasks get completed.

---

## 📌 Phase 1: Setup

* [ ] Initialize Chrome Extension with React + TypeScript
* [ ] Configure `manifest.json` (permissions: storage, contextMenus, activeTab)
* [ ] Set up Tailwind CSS for UI styling
* [ ] Connect Firebase Auth + Firestore

---

## 📌 Phase 2: Core Features

* [ ] Build **Profile Manager** in Options page
* [ ] Implement **Context Menu** → extract job posting text
* [ ] Integrate Prompt API + Writer API for content generation
* [ ] Save generated resumes and cover letters in Firestore

---

## 📌 Phase 3: Enhancements

* [ ] Add Proofreader API for grammar fixes
* [ ] Add Rewriter API for variations and tone adjustment
* [ ] Build Popup UI:

  * [ ] Quick view of generated applications
  * [ ] Copy/download buttons
  * [ ] View history

---

## 📌 Phase 4: Testing & UX

* [ ] Test on LinkedIn, Indeed, and Google Jobs
* [ ] Add loading states and error handling
* [ ] Optimize API calls for speed
* [ ] Finalize clean UI design + logo

---

## 📌 Phase 5: Demo & Submission

* [ ] Record demo video (<3 min) showing workflow
* [ ] Write clear GitHub README with setup instructions
* [ ] Add MIT License
* [ ] Submit project to Devpost for Google Hackathon 2025

---

## 📁 Proposed GitHub Repo Structure

```
job-application-assistant/
│── public/                # Static assets (icons, logos, manifest.json)
│   ├── icon16.png
│   ├── icon48.png
│   ├── icon128.png
│   └── manifest.json
│
│── src/                   # Source code
│   ├── background/        # Service worker scripts (context menus, APIs)
│   │   └── background.ts
│   │
│   ├── popup/             # Popup UI
│   │   ├── Popup.tsx
│   │   └── Popup.css
│   │
│   ├── options/           # Options page (Profile Manager)
│   │   ├── Options.tsx
│   │   └── Options.css
│   │
│   ├── components/        # Shared React components
│   │   ├── Button.tsx
│   │   ├── Card.tsx
│   │   └── Loader.tsx
│   │
│   ├── hooks/             # Custom React hooks
│   │   └── useAuth.ts
│   │
│   ├── services/          # API integrations (Prompt, Writer, Proofreader, Rewriter)
│   │   ├── prompt.ts
│   │   ├── writer.ts
│   │   ├── proofreader.ts
│   │   └── rewriter.ts
│   │
│   ├── utils/             # Helpers (parsers, formatters, constants)
│   │   └── parser.ts
│   │
│   └── index.tsx          # Entry point
│
│── styles/                # Global Tailwind overrides
│   └── globals.css
│
│── .gitignore
│── package.json
│── README.md
│── prd.md
│── todo.md
│── LICENSE

