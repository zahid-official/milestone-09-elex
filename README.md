# 📚 Elex

**Elex** is a modern and responsive vocabulary learning platform designed to make language practice feel approachable, interactive, and visually engaging. Focused on Japanese vocabulary learning, the app combines guided lessons, protected learning routes, pronunciation support, embedded video tutorials, and user authentication to create a smooth learning experience from exploration to practice.

<div align="center">
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" alt="Firebase" />
  <img src="https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white" alt="React Router" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/DaisyUI-5A0EF8?style=for-the-badge" alt="DaisyUI" />
  <img src="https://img.shields.io/badge/Responsive-Design-green?style=for-the-badge" alt="Responsive Design" />
</div>

## 🔗 Quick Links

- **Live Website:** [elex-official.netlify.app](https://elex-official.netlify.app/)

## 🌟 Learning Experience

- **Structured Lesson Flow:** Browse lesson categories and move into vocabulary-based practice through a guided route structure.
- **Protected Learning Content:** Access lesson details, tutorials, and profile-related pages through authenticated private routes.
- **Interactive Vocabulary Cards:** Explore word cards with pronunciation, meaning, part of speech, difficulty level, and contextual usage.
- **Tutorial Support:** Learn through embedded video content that helps reinforce pronunciation and understanding.
- **Personalized Profile Access:** Registered users can manage their learning account and update profile information inside the app.
- **Responsive Interface:** Study comfortably across mobile, tablet, and desktop screens with a layout built for accessibility and ease of use.

## 🎯 Core Features

- **Authentication System:** Users can register, sign in, sign out, reset passwords, and continue with Google authentication using Firebase.
- **Route-Based Learning:** Lessons are organized through React Router, with category pages and individual lesson pages loaded dynamically from local JSON data.
- **Pronunciation Interaction:** Vocabulary cards use the browser speech synthesis API to pronounce Japanese words directly inside the lesson view.
- **Context-Driven Auth State:** Authentication state is shared across the app through a central provider and used to protect restricted content.
- **Dynamic Page Titles:** Each major page updates the browser title using `react-helmet-async`, improving usability and polish.

## 🛠️ Technologies Used

| Technology | Version | Purpose |
| :--- | :---: | :--- |
| **React** | `^18.3.1` | Component-based UI development |
| **JavaScript** | `ES6+` | App logic and interactivity |
| **Vite** | `^5.4.10` | Dev server and build tooling |
| **Firebase** | `^11.1.0` | Authentication and user management |
| **React Router DOM** | `^6.28.0` | Client-side routing |
| **Tailwind CSS** | `^3.4.15` | Utility-first styling |
| **DaisyUI** | `^4.12.14` | UI components |
| **React Toastify** | `^11.0.2` | Toast notifications |
| **React Helmet Async** | `^2.0.5` | Dynamic page titles |
| **Swiper** | `^11.2.1` | Interactive sliders and carousel UI |
| **AOS** | `^2.3.4` | Scroll animations |

## ⚙️ How It Works

1. Users start on the landing page and explore the platform overview
2. Lesson categories are loaded from `categories.json`
3. Selecting a lesson opens a protected vocabulary learning route
4. Vocabulary data is loaded from `words.json` and displayed as interactive cards
5. Users can watch tutorial videos, manage authentication, and update profile information from dedicated routes

## 📂 Project Structure

```bash
milestone-09/
├── package.json             # Dependencies and scripts
├── public/                  # Public assets and learning data
│   ├── categories.json      # Lesson category dataset
│   ├── words.json           # Vocabulary dataset
│   └── CNAME                # Deployment domain config
└── src/                     # Application source code
    ├── main.jsx             # React entry point
    ├── App.jsx              # Root app wrapper
    ├── Layout/              # Shared layout components
    ├── Routes/              # Route and private route setup
    ├── Pages/               # Main routed pages
    └── Components/          # Reusable UI and auth components
```

## 📋 Prerequisites

- **Node.js** and **npm** installed on your machine
- A Firebase project configured through environment variables
- A modern browser for local development preview

## 🚀 Getting Started

```bash
npm install
npm run dev
```

Create a `.env.local` file and provide the required Firebase environment variables before running the app locally.

## 📜 Available Scripts

```bash
npm run dev      # Start the Vite development server
npm run build    # Create a production build
npm run preview  # Preview the production build locally
npm run lint     # Run ESLint checks
```

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

  <p>Building polished digital experiences with passion and purposeful design</p>
</div>

## 🤝 Contributing

Contributions make the project better for everyone. If you would like to improve **Elex**, your contributions are always welcome.

```bash
1. Fork the project
2. Create your feature branch (git checkout -b feature/AmazingFeature)
3. Commit your changes (git commit -m 'Add some AmazingFeature')
4. Push to the branch (git push origin feature/AmazingFeature)
5. Open a Pull Request
```

<p align="center"><b>Elex</b><i> - Where every lesson turns vocabulary into confidence.</i></p>
