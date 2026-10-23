# Yokeshwaran R — Developer Portfolio

A modern, fast, responsive personal developer portfolio website built for **Yokeshwaran R**, B.Sc. Computer Science student at Hindustan Institute of Technology and Science (HITS), Chennai, and aspiring Backend / Software Developer.

Built with **React**, **Vite**, **Lucide React**, and **Vanilla CSS** with a futuristic dark theme, electric blue/cyan accents, and glassmorphic aesthetics.

---

## 🚀 Quick Start

### 1. Install Dependencies
```bash
npm install
```

### 2. Start the Local Development Server
```bash
npm run dev
```
The website will be available at: `http://localhost:3000/`

### 3. Build for Production
```bash
npm run build
```
The optimized production output will be generated inside the `dist/` directory, ready to deploy to Vercel, Netlify, or GitHub Pages.

---

## 🛠️ Technology Stack

- **Core**: React 18, JavaScript (ES6+), HTML5 Semantic markup
- **Build Tool**: Vite 6 (Ultra-fast HMR and bundle compilation)
- **Styling**: Vanilla CSS (Custom Design System with CSS variables, Glassmorphism, Responsive Grid, and Reduced-Motion accessibility)
- **Icons**: Lucide React

---

## 📁 Project Structure

```
yokeshportfolio/
├── index.html              # HTML entry point with meta tags & Google fonts
├── package.json            # Scripts & dependencies
├── vite.config.js          # Vite configuration (port 3000)
├── dist/                   # Production build output
├── public/                 # Static assets (add your profile image here)
└── src/
    ├── main.jsx            # React root mount
    ├── App.jsx             # Main interactive application & layout
    ├── portfolioData.js    # 🌟 Centralized data file (edit all content here!)
    └── styles.css          # Design system, glassmorphism, responsive styles
```

---

## ✏️ How to Customize Your Portfolio

All your data, projects, social links, and details are centralized in **[`src/portfolioData.js`](src/portfolioData.js)**. You do not need to touch complex React code to update your info!

### 1. Add Your Real GitHub & LinkedIn Links
Open `src/portfolioData.js` and locate `personalData.socials`:
```javascript
socials: {
  github: {
    name: "GitHub",
    url: "https://github.com/your-real-username", // <-- Replace with your link
    isPlaceholder: false                          // <-- Set to false
  },
  linkedin: {
    name: "LinkedIn",
    url: "https://linkedin.com/in/your-real-handle", // <-- Replace with your link
    isPlaceholder: false                            // <-- Set to false
  },
  // ...
}
```

### 2. Add Your Profile Photo
1. Copy your photo into the `public/` folder (e.g. `public/profile.jpg`).
2. In `src/portfolioData.js`, set `profileImage`:
```javascript
profileImage: "/profile.jpg",
```
*(If left `null`, the site displays the futuristic CSS-designed avatar with your initials "YR" automatically!)*

### 3. Adding or Updating Projects
In `src/portfolioData.js`, add or edit items in the `projects` array:
```javascript
{
  id: "my-new-project",
  title: "E-Commerce Backend API",
  isExample: false,
  badge: "Featured Project",
  shortDescription: "A scalable REST API built with Python, FastAPI and MongoDB.",
  techTags: ["Python", "FastAPI", "MongoDB", "JWT"],
  image: null,
  githubUrl: "https://github.com/your-username/my-api",
  liveUrl: "https://api.example.com",
  status: "Completed"
}
```

### 4. Updating Certificates or Internship
Edit `certificates` or `internshipExperience` in `src/portfolioData.js`. The UI will adapt immediately!

---

## 📱 Features Included

- **Futuristic Dark Glassmorphic Design**: Electric blue & cyan accents, subtle radial glows, and high-contrast typography.
- **Responsive Layout**: Fluid experience across mobile, tablet, and desktop screens with a working mobile navigation drawer.
- **Accessible & Performance-Minded**: Respects `prefers-reduced-motion`, visible keyboard focus states, zero bloat, and fast load times.
- **Smart Contact Integration**:
  - One-click copy for Email (`yokeshwaran021@gmail.com`) and Phone (`+91 6379042330`).
  - Working `tel:` and `mailto:` links.
  - Functional contact form with validation and client-side `mailto:` fallback pre-populating recipient, subject, and message.
- **Safe Placeholders**: Interactive toasts inform visitors when clicking editable placeholder links or demo-pending buttons, preventing dead links.
- **Back-to-Top**: Smooth scrolling with dynamic current year calculation.
