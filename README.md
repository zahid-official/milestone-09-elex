<div align="center">

<img src="https://elex-official.netlify.app/assets/logo.png" alt="Elex Logo" width="50" />

# Elex - Japanese Vocabulary Learning Platform

A modern, interactive web application for mastering Japanese vocabulary through structured lessons, pronunciation practice, embedded video tutorials, and guided learning paths.

[![Live Demo](https://img.shields.io/badge/▶_Live_Demo-elex--official.netlify.app-00C853?style=for-the-badge&logo=netlify&logoColor=white)](https://elex-official.netlify.app/)
[![GitHub Repo](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/zahid-official/milestone-09-elex)
<img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
<img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
<img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" alt="Firebase" />
<img src="https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white" alt="React Router" />
<img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS" />
<img src="https://img.shields.io/badge/DaisyUI-5A0EF8?style=for-the-badge" alt="DaisyUI" />

</div>

<br/>

## 🔍 Overview

**Elex** is a vocabulary learning platform focused on making Japanese language practice feel approachable, interactive, and visually engaging. The application combines guided lessons, protected learning routes, real-time pronunciation support, embedded video tutorials, and a complete user authentication system — delivering a seamless experience from exploration to practice.

> _Where every lesson turns vocabulary into confidence._

<br/>

## ✨ Key Features

### 🎓 Learning Experience

<table align="center">
<thead>
<tr><th align="left">Feature</th><th align="left">Description</th></tr>
</thead>
<tbody>
<tr><td><b>Structured Lesson Flow</b></td><td>Browse categorized lessons and progress through vocabulary practice via a guided route system</td></tr>
<tr><td><b>Interactive Vocabulary Cards</b></td><td>Explore word cards displaying pronunciation, meaning, part of speech, difficulty level, and contextual usage</td></tr>
<tr><td><b>Pronunciation Engine</b></td><td>Hear Japanese words spoken aloud using the browser's built-in Web Speech Synthesis API</td></tr>
<tr><td><b>Video Tutorials</b></td><td>Reinforce learning through embedded video content directly within the platform</td></tr>
</tbody>
</table>

### 🔐 Authentication & Security

<table align="center">
<thead>
<tr><th align="left">Feature</th><th align="left">Description</th></tr>
</thead>
<tbody>
<tr><td><b>Multi-Method Auth</b></td><td>Register, sign in, sign out, and reset passwords — plus Google OAuth via Firebase</td></tr>
<tr><td><b>Protected Routes</b></td><td>Lesson details, tutorials, and profile pages are secured behind authenticated private routes</td></tr>
<tr><td><b>Profile Management</b></td><td>Registered users can view and update their account information within the app</td></tr>
</tbody>
</table>

### 🎨 User Interface

<table align="center">
<thead>
<tr><th align="left">Feature</th><th align="left">Description</th></tr>
</thead>
<tbody>
<tr><td><b>Responsive Design</b></td><td>Fully optimized for mobile, tablet, and desktop viewports</td></tr>
<tr><td><b>Scroll Animations</b></td><td>Smooth AOS-powered animations triggered on scroll for a polished feel</td></tr>
<tr><td><b>Interactive Sliders</b></td><td>Swiper-based carousels for dynamic content presentation</td></tr>
<tr><td><b>Dynamic Page Titles</b></td><td>Each page updates the browser tab title via <code>react-helmet-async</code></td></tr>
<tr><td><b>Toast Notifications</b></td><td>User-friendly feedback through <code>react-toastify</code> alerts</td></tr>
</tbody>
</table>

<br/>

## 🛠️ Tech Stack

<table align="center">
<thead>
<tr><th align="left">Technology</th><th align="center">Version</th><th align="left">Purpose</th></tr>
</thead>
<tbody>
<tr><td><b>React</b></td><td align="center"><code>^18.3.1</code></td><td>Component-based UI development</td></tr>
<tr><td><b>JavaScript</b></td><td align="center"><code>ES6+</code></td><td>Application logic and interactivity</td></tr>
<tr><td><b>Vite</b></td><td align="center"><code>^5.4.10</code></td><td>Lightning-fast dev server and build tooling</td></tr>
<tr><td><b>Firebase</b></td><td align="center"><code>^11.1.0</code></td><td>Authentication and user management</td></tr>
<tr><td><b>React Router DOM</b></td><td align="center"><code>^6.28.0</code></td><td>Declarative client-side routing</td></tr>
<tr><td><b>Tailwind CSS</b></td><td align="center"><code>^3.4.15</code></td><td>Utility-first CSS framework</td></tr>
<tr><td><b>DaisyUI</b></td><td align="center"><code>^4.12.14</code></td><td>Tailwind-based UI component library</td></tr>
<tr><td><b>React Toastify</b></td><td align="center"><code>^11.0.2</code></td><td>Toast notification system</td></tr>
<tr><td><b>React Helmet Async</b></td><td align="center">—</td><td>Dynamic document head management</td></tr>
<tr><td><b>Swiper</b></td><td align="center"><code>^11.2.1</code></td><td>Touch-enabled slider and carousel</td></tr>
<tr><td><b>AOS</b></td><td align="center"><code>^2.3.4</code></td><td>Animate On Scroll library</td></tr>
<tr><td><b>React Icons</b></td><td align="center"><code>^5.3.0</code></td><td>Popular icon sets as React components</td></tr>
<tr><td><b>React CountUp</b></td><td align="center"><code>^6.5.3</code></td><td>Animated number counting</td></tr>
<tr><td><b>Animate.css</b></td><td align="center"><code>^4.1.1</code></td><td>Pre-built CSS animations</td></tr>
</tbody>
</table>

<br/>

## 🏗️ Architecture

<div align="center">
<pre>
┌─────────────────────────────────────────────────────────────┐
│                        Browser                              │
├─────────────────────────────────────────────────────────────┤
│  React App (Vite)                                           │
│  ┌───────────┐  ┌──────────────┐  ┌──────────────────────┐  │
│  │  Layout   │  │  React       │  │  Auth Provider       │  │
│  │  (Navbar+ │◄─┤  Router      │  │  (Firebase Context)  │  │
│  │   Footer) │  │  (Public +   │  │                      │  │
│  │           │  │   Private)   │  │  • Login / Register  │  │
│  └───────────┘  └──────┬───────┘  │  • Google OAuth      │  │
│                        │          │  • Password Reset    │  │
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
</pre>
</div>

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

<table align="center">
<thead>
<tr><th align="left">Requirement</th><th align="left">Details</th></tr>
</thead>
<tbody>
<tr><td><b>Node.js</b></td><td>v18 or higher recommended</td></tr>
<tr><td><b>npm</b></td><td>Comes bundled with Node.js</td></tr>
<tr><td><b>Firebase Project</b></td><td>Required for authentication features</td></tr>
<tr><td><b>Modern Browser</b></td><td>Chrome, Firefox, Safari, or Edge</td></tr>
</tbody>
</table>

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

<table align="center">
<thead>
<tr><th align="left">Command</th><th align="left">Description</th></tr>
</thead>
<tbody>
<tr><td><code>npm run dev</code></td><td>Start the Vite development server with HMR</td></tr>
<tr><td><code>npm run build</code></td><td>Create an optimized production build</td></tr>
<tr><td><code>npm run preview</code></td><td>Preview the production build locally</td></tr>
<tr><td><code>npm run lint</code></td><td>Run ESLint to check for code quality issues</td></tr>
</tbody>
</table>

<br/>

## ⚙️ How It Works

<div align="center">
<pre>
User lands on Home ──► Browses Lesson Categories ──► Selects a Lesson
                                                          │
                              ┌───────────────────────────┘
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
                Lesson           &amp; Manage Profile
</pre>
</div>

1. **Landing** — Users explore the platform overview, features, and success metrics on the home page.
2. **Category Browsing** — Lesson categories are rendered dynamically from `categories.json`.
3. **Authenticated Learning** — Selecting a lesson triggers a private route; unauthenticated users are redirected to sign in.
4. **Vocabulary Practice** — Words from `words.json` are presented as interactive cards with pronunciation, meaning, and difficulty tags.
5. **Extended Learning** — Users can access embedded video tutorials, manage their profile, and update account details.

<br/>

## 🌟 Author

<div align="center">
  <a href="https://github.com/zahid-official">
    <img src="https://github.com/zahid-official.png" width="100" height="100" style="border-radius: 50%;" alt="Zahid Official" />
  </a>

  <h3>Zahid Official</h3>
  <p><b>Web Developer | Tech Enthusiast</b></p>

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/zahid-official)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/zahid-web)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:zahid.official8@gmail.com)

  <p>Creating impactful digital experiences with passion and purposeful design</p>
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

<p align="center"><b>Elex</b><i> - Where every lesson brings your language goals closer with confidence.</i></p>
