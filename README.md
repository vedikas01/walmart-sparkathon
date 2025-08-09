# 🏷️ Walmart Sparkathon – AI-Driven Multi-modal Shopping Assistant

**Problem Statement**: Customers often hesitate to purchase apparel online due to uncertainty about fit, appearance, and style suitability, leading to lower confidence, increased returns, and a less engaging shopping experience.

**Solution**: An AI-driven Multi-modal Shopping Assistant that understands text, voice, and image queries, provides personalized recommendations, and enables Virtual Try-On using GenAI to overlay selected apparel on user images/videos, boosting confidence in purchases.

## 👥 Team Members & Responsibilities

We are a team of four collaborating on this project for the Walmart Sparkathon. **Harshit** is leading the frontend development and handling DevOps responsibilities, setting up the monorepo with Turborepo and pnpm, and guiding the overall project structure. **Vedika** is responsible for building the backend using Node.js with GraphQL, managing all server-side logic and API development. **Dristant** is focusing on the mobile application, developing it using **Kotlin (Android)** to ensure seamless user experience on mobile platforms. **Manodeep** is handling all the AI-related features and integrations, working with APIs like Tavily and Groq to power intelligent features within the application. Together, we're aiming to build a full-stack solution with both web and mobile interfaces, supported by robust AI capabilities.

| Name | Role | Responsibilities |
|------|------|------------------|
| **Harshit** | Frontend & DevOps | Next.js web app, Turborepo setup, project architecture |
| **Vedika** | Backend Developer | Node.js + GraphQL API, MongoDB, server-side logic |
| **Dristant** | Mobile Developer | Kotlin (Android) app, mobile UI/UX |
| **Manodeep** | AI Developer | Tavily API, Groq API, AI features & integrations |

## 🚀 Features

1. **Multi-modal Inputs**: Text, voice, or upload reference image → get suggestions
2. **AI-Powered Virtual Try-On**: 
   - User uploads a photo or short video
   - AI generates a realistic preview of selected apparel on the user
3. **Personalized Recommendations**: Based on previous purchases, trends, or user preferences
4. **Voice Assistant** (Optional): "Show me formal shoes for weddings" → curated feed
5. **AR Integration** (Stretch Goal): Live try-on using phone camera

## 🛠️ Tech Stack

| Component | Technology |
|-----------|------------|
| **Mobile App** | Kotlin (Android) |
| **Web App** | Next.js (React) + Tailwind CSS |
| **Backend/API** | Node.js + Apollo Server (GraphQL) |
| **Database** | MongoDB Atlas |
| **AI APIs** | Tavily API, Groq API, Replicate API (for try-on) |
| **Voice Input** | Android SpeechRecognizer API (mobile), Web Speech API (web) |
| **Image Storage** | Cloudinary |
| **Deployment** | Vercel (frontend), Render/Railway/Fly.io (backend), MongoDB Atlas |
| **Authentication** | Firebase Auth or Auth0 (Optional) |
| **Monorepo** | Turborepo + pnpm |

## 📦 Monorepo Structure

```
walmart-sparkathon/
├── apps/
│   ├── web/         → Next.js frontend
│   ├── api/         → Node.js GraphQL backend  
│   ├── ai/          → AI backend/service (Tavily, Groq)
│   └── mobile/      → Kotlin (Android) app
├── packages/
│   ├── common/      → Shared types and utilities
│   └── ai-utils/    → (optional, shared AI helpers)
├── turbo.json
├── pnpm-workspace.yaml
└── package.json
```

## 🚀 Getting Started

### ✅ Prerequisites
- **Node.js** (Recommended via [nvm](https://github.com/nvm-sh/nvm)):
  ```bash
  nvm install node
  ```
- **pnpm** (installed globally):
  ```bash
  npm install -g pnpm
  ```
- **Android Studio** (for mobile app):
  - Download from https://developer.android.com/studio

### 📥 Clone the Repository
```bash
git clone https://github.com/Harsh-GAMMARAYS/walmart-sparkathon.git
cd walmart-sparkathon
```

### 📦 Install Dependencies (for web/api/ai)
```bash
pnpm install
```

### 🏃 Running Applications
Each team member can run their specific app:

**Harshit (Web Frontend):**
```bash
cd apps/web
pnpm dev
```

**Vedika (Backend API):**
```bash
cd apps/api  
pnpm dev
```

**Dristant (Mobile App):**
- Open `apps/mobile/` in Android Studio
- Build and run the app on an emulator or device

**Manodeep (AI Service):**
```bash
cd apps/ai
pnpm dev
```

## 💻 Development Workflow

### 🌿 Branching Strategy
1. Create feature branches:
   ```bash
   git checkout -b feature/<feature-name>
   ```
   Examples:
   - `feature/api-setup`
   - `feature/mobile-login-screen`
   - `feature/ai-product-recommender`
   - `feature/frontend-homepage`

2. Commit with descriptive messages:
   ```bash
   git commit -m "feat: added virtual try-on API integration"
   git commit -m "fix: resolved GraphQL schema validation issue"
   ```

3. Push and create Pull Requests:
   ```bash
   git push --set-upstream origin feature/<branch-name>
   ```

### 🔄 Team Collaboration
- **Daily Syncs**: Quick 15-minute standups
- **Code Reviews**: All PRs require review before merge
- **Communication**: WhatsApp/Slack for quick updates
- **Documentation**: Keep README and code comments updated

## ⚙️ Useful Commands

| Command | Description |
|---------|-------------|
| `pnpm dev` | Run dev server (per app) |
| `pnpm build` | Build app (per app) |
| `pnpm install` | Install dependencies |
| `turbo run dev` | Run all apps in parallel |
| `turbo run build` | Build all apps |

## 🎯 Project Goals

- **Reduce Returns**: Help customers make confident purchase decisions
- **Boost Personalization**: AI-driven recommendations for better customer experience  
- **Cutting-edge Tech**: Multi-modal AI interaction (text, voice, image)
- **Seamless Experience**: Works across web and mobile platforms

## 🆘 Need Help?
- **DevOps/Frontend Issues**: Contact @Harshit
- **Backend/API Issues**: Contact @Vedika  
- **Mobile App Issues**: Contact @Dristant
- **AI Integration Issues**: Contact @Manodeep

---

**Built with ❤️ for Walmart Sparkathon 2025**
