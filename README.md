<div align="center">

<img src="https://elex-official.netlify.app/assets/logo.png" alt="Elex Logo" width="50" />

# Elex — Japanese Vocabulary Learning Platform

A modern, interactive web application for mastering Japanese vocabulary through structured lessons, pronunciation practice, embedded video tutorials, and guided learning paths.

[![Live Demo](https://img.shields.io/badge/▶_Live_Demo-elex--official.netlify.app-00C853?style=for-the-badge&logo=netlify&logoColor=white)](https://elex-official.netlify.app/)
[![GitHub Repo](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/zahid-official/milestone-09-elex)

<br/>

<img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
<img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
<img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" alt="Firebase" />
<img src="https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white" alt="React Router" />
<img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS" />
<img src="https://img.shields.io/badge/DaisyUI-5A0EF8?style=for-the-badge" alt="DaisyUI" />

</div>

<br/>

## 📖 Table of Contents

- [Overview](#-overview)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [Architecture](#-architecture)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Environment Variables](#-environment-variables)
- [Available Scripts](#-available-scripts)
- [How It Works](#-how-it-works)
- [Contributing](#-contributing)
- [Author](#-author)

<br/>

## 🔍 Overview

**Elex** is a vocabulary learning platform focused on making Japanese language practice feel approachable, interactive, and visually engaging. The application combines guided lessons, protected learning routes, real-time pronunciation support, embedded video tutorials, and a complete user authentication system — delivering a seamless experience from exploration to practice.

> _Where every lesson turns vocabulary into confidence._

<br/>

## ✨ Key Features

### 🎓 Learning Experience

| Feature                          | Description                                                                                                  |
| :------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| **Structured Lesson Flow**       | Browse categorized lessons and progress through vocabulary practice via a guided route system                |
| **Interactive Vocabulary Cards** | Explore word cards displaying pronunciation, meaning, part of speech, difficulty level, and contextual usage |
| **Pronunciation Engine**         | Hear Japanese words spoken aloud using the browser's built-in Web Speech Synthesis API                       |
| **Video Tutorials**              | Reinforce learning through embedded video content directly within the platform                               |

### 🔐 Authentication & Security

| Feature                | Description                                                                                  |
| :--------------------- | :------------------------------------------------------------------------------------------- |
| **Multi-Method Auth**  | Register, sign in, sign out, and reset passwords — plus Google OAuth via Firebase            |
| **Protected Routes**   | Lesson details, tutorials, and profile pages are secured behind authenticated private routes |
| **Profile Management** | Registered users can view and update their account information within the app                |

### 🎨 User Interface

| Feature                 | Description                                                           |
| :---------------------- | :-------------------------------------------------------------------- |
| **Responsive Design**   | Fully optimized for mobile, tablet, and desktop viewports             |
| **Scroll Animations**   | Smooth AOS-powered animations triggered on scroll for a polished feel |
| **Interactive Sliders** | Swiper-based carousels for dynamic content presentation               |
| **Dynamic Page Titles** | Each page updates the browser tab title via `react-helmet-async`      |
| **Toast Notifications** | User-friendly feedback through `react-toastify` alerts                |

<br/>

## 🛠️ Tech Stack

| Technology             |  Version   | Purpose                                     |
| :--------------------- | :--------: | :------------------------------------------ |
| **React**              | `^18.3.1`  | Component-based UI development              |
| **JavaScript**         |   `ES6+`   | Application logic and interactivity         |
| **Vite**               | `^5.4.10`  | Lightning-fast dev server and build tooling |
| **Firebase**           | `^11.1.0`  | Authentication and user management          |
| **React Router DOM**   | `^6.28.0`  | Declarative client-side routing             |
| **Tailwind CSS**       | `^3.4.15`  | Utility-first CSS framework                 |
| **DaisyUI**            | `^4.12.14` | Tailwind-based UI component library         |
| **React Toastify**     | `^11.0.2`  | Toast notification system                   |
| **React Helmet Async** |     —      | Dynamic document head management            |
| **Swiper**             | `^11.2.1`  | Touch-enabled slider and carousel           |
| **AOS**                |  `^2.3.4`  | Animate On Scroll library                   |
| **React Icons**        |  `^5.3.0`  | Popular icon sets as React components       |
| **React CountUp**      |  `^6.5.3`  | Animated number counting                    |
| **Animate.css**        |  `^4.1.1`  | Pre-built CSS animations                    |

<br/>

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                        Browser                              │
├─────────────────────────────────────────────────────────────┤
│  React App (Vite)                                           │
│  ┌───────────┐  ┌──────────────┐  ┌──────────────────────┐  │
│  │  Layout    │  │  React       │  │  Auth Provider       │  │
│  │  (Navbar + │◄─┤  Router      │  │  (Firebase Context)  │  │
│  │   Footer)  │  │  (Public +   │  │                      │  │
│  │           │  │   Private)   │  │  • Login / Register  │  │
│  └───────────┘  └──────┬───────┘  │  • Google OAuth      │  │
│                        │          │  • Password Reset     │  │
│               ┌────────▼────────┐ └──────────────────────┘  │
│               │     Pages       │                           │
│               │  Home │ Learn   │                           │
│               │  About│ Profile │                           │
│               │  Tutorials      │                           │
│               └────────┬────────┘                           │
│                        │                                    │
│               ┌────────▼────────┐                           │
│               │   Components    │                           │
│               │  Cards │ Banner │                           │
│               │  Slider│ Videos │                           │
│               └─────────────────┘                           │
├─────────────────────────────────────────────────────────────┤
│  Static Data: categories.json · words.json                  │
└─────────────────────────────────────────────────────────────┘
```

<br/>

## 📂 Project Structure

```
milestone-09/
│
├── index.html                     # HTML entry point
├── package.json                   # Dependencies and scripts
├── vite.config.js                 # Vite configuration
│
├── public/                        # Static assets and learning data
│   ├── assets/                    # Images and media files
│   ├── categories.json            # Lesson category dataset
│   └── words.json                 # Vocabulary dataset
│
└── src/
    ├── main.jsx                   # React DOM entry point
    ├── App.jsx                    # Root application wrapper
    │
    ├── Layout/                    # Shared layout (Navbar + Footer)
    ├── Routes/                    # Route config and private route guard
    ├── Pages/                     # Routed pages — Home, Learn, About, Profile, Tutorials
    │
    └── Components/
        ├── Auth/                  # Firebase authentication (Login, Register, OAuth)
        ├── Home/                  # Landing page sections (Banner, Features, Slider)
        ├── Learn/                 # Lesson cards, vocabulary cards, embedded videos
        └── Profile/               # Profile display and update forms
```

<br/>

## 🚀 Getting Started

### Prerequisites

| Requirement          | Details                              |
| :------------------- | :----------------------------------- |
| **Node.js**          | v18 or higher recommended            |
| **npm**              | Comes bundled with Node.js           |
| **Firebase Project** | Required for authentication features |
| **Modern Browser**   | Chrome, Firefox, Safari, or Edge     |

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/zahid-official/milestone-09-elex.git

# 2. Navigate to the project directory
cd milestone-09-elex

# 3. Install dependencies
npm install

# 4. Set up environment variables (see section below)

# 5. Start the development server
npm run dev
```

The application will be available at `http://localhost:5173` by default.

<br/>

## 🔑 Environment Variables

Create a `.env.local` file in the project root with the following Firebase credentials:

```env
VITE_apiKey=your_firebase_api_key
VITE_authDomain=your_project.firebaseapp.com
VITE_projectId=your_project_id
VITE_storageBucket=your_project.appspot.com
VITE_messagingSenderId=your_sender_id
VITE_appId=your_app_id
```

> **Note:** All environment variables must be prefixed with `VITE_` for Vite to expose them to the client bundle. Never commit `.env.local` to version control.

<br/>

## 📜 Available Scripts

| Command           | Description                                 |
| :---------------- | :------------------------------------------ |
| `npm run dev`     | Start the Vite development server with HMR  |
| `npm run build`   | Create an optimized production build        |
| `npm run preview` | Preview the production build locally        |
| `npm run lint`    | Run ESLint to check for code quality issues |

<br/>

## ⚙️ How It Works

```
User lands on Home ──► Browses Lesson Categories ──► Selects a Lesson
                                                          │
                              ┌────────────────────────────┘
                              ▼
                    Route requires auth?
                     ┌──── Yes ────┐
                     ▼             ▼
                Not logged in   Logged in
                     │             │
                     ▼             ▼
                Redirect to    Load Lesson
                Login Page     Vocabulary
                     │             │
                     ▼             ▼
                Authenticate   Interactive Cards
                (Email/Google) (Pronunciation + Usage)
                     │             │
                     ▼             ▼
                Return to ────► Watch Tutorials
                Lesson           & Manage Profile
```

1. **Landing** — Users explore the platform overview, features, and success metrics on the home page.
2. **Category Browsing** — Lesson categories are rendered dynamically from `categories.json`.
3. **Authenticated Learning** — Selecting a lesson triggers a private route; unauthenticated users are redirected to sign in.
4. **Vocabulary Practice** — Words from `words.json` are presented as interactive cards with pronunciation, meaning, and difficulty tags.
5. **Extended Learning** — Users can access embedded video tutorials, manage their profile, and update account details.

<br/>

## 👤 Author

<div align="center">
  <a href="https://github.com/zahid-official">
    <img src="https://github.com/zahid-official.png" width="100" height="100" style="border-radius: 50%;" alt="Zahid Official" />
  </a>

  <h3>Zahid Official</h3>
  <p><b>Web Developer | Tech Enthusiast</b></p>

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/zahid-official)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/zahid-web)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:zahid.official8@gmail.com)

  <p>Building polished digital experiences with passion and purposeful design</p>
</div>

<br/>

## 🤝 Contributing

Contributions are welcome and appreciated! Here's how you can help improve **Elex**:

```bash
# 1. Fork the repository

# 2. Create a feature branch
git checkout -b feature/your-feature-name

# 3. Make your changes and commit
git commit -m "feat: add your feature description"

# 4. Push to your fork
git push origin feature/your-feature-name

# 5. Open a Pull Request against the main branch
```

Please ensure your code follows the existing project conventions and passes linting before submitting.