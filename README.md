# 🎬 Movie Explorer — PWA Version

> A Progressive Web App (PWA) built with React.js + Vite that lets users search, explore, and save TV shows and movies — installable directly on Android from the browser.

---

## 🌐 Live Demo

🔗 **[View Live on Vercel](#)** *(link will be added after deployment)*

---

## 📌 About This Project

Movie Explorer PWA is the mobile-optimized, installable version of my original Movie Explorer web app. It connects to the [TVMaze API](https://api.tvmaze.com/shows) to display a rich library of TV shows and movies, supports real-time search, and lets users manage a personal watchlist — all without needing to install anything from an app store.

### 🔗 Original Web Version

This project was cloned and upgraded from my original web repo:
👉 [Movie Explorer Web](https://github.com/nipuninduwaraedu/Movie_Explorer_Web.git)

Key upgrades in this version:
- Converted to a fully installable **Progressive Web App (PWA)**
- Added a **Web App Manifest** for home screen installation
- Integrated **Service Worker** via `vite-plugin-pwa` for offline support

---

## ✨ Features

### 📱 PWA Features
- Installable on Android via Chrome ("Add to Home Screen")
- Works offline after the first visit (cached assets via service worker)
- Launches in fullscreen — feels like a native app
- Custom app icon and splash screen via Web App Manifest

### 🎥 App Features
- Browse a curated list of TV shows and movies
- Real-time search powered by the TVMaze API
- Add and remove titles from a personal Watchlist
- Watchlist state managed globally with React Context API
- Fully responsive, mobile-first UI

---

## 🤔 What is a PWA?

A **Progressive Web App (PWA)** is a web application that behaves like a native mobile app. It can be installed on your device, works offline, and launches without a browser toolbar — all without going through an app store.

PWAs use two key technologies:
- **Service Worker** — a background script that caches files for offline use
- **Web App Manifest** — a JSON file that defines the app name, icon, and display settings

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| React.js | UI component library |
| Vite | Build tool and dev server |
| vite-plugin-pwa | PWA support (service worker + manifest) |
| React Context API | Global state management (Watchlist) |
| TVMaze API | TV show and movie data source |
| CSS / Flexbox | Responsive styling |
| Vercel | Deployment platform |

---

## 🌐 API Used

**TVMaze API** — Free, public REST API for TV show data.

- Base URL: `https://api.tvmaze.com/shows`
- 
---

## 📁 Project Structure

```
Movie_Explorer_Mobile/
├── public/
│   └── pwa-192.png.png /              # PWA icons 
├── src/
│   ├── components/         # Reusable UI components (Navbar, MovieCard, etc.)
│   ├── context/            # React Context API (WatchlistContext)
│   ├── pages/              # Page-level components (Home, Watchlist, Search)
│   ├── App.jsx             # Root component with routing
│   └── main.jsx            # Entry point
├── index.html
├── vite.config.js          # Vite + PWA plugin configuration
└── package.json
```

---

## ⚙️ Installation & Setup

> Make sure you have **Node.js** and **npm** installed.

```bash
# 1. Clone the repository
git clone https://github.com/nipuninduwaraedu/Movie_Explorer_Mobile.git

# 2. Navigate into the project folder
cd Movie_Explorer_Mobile

# 3. Install dependencies
npm install

# 4. Start the development server
npm run dev
```

Open `http://localhost:5173` in your browser.

---

## 📦 Build for Production

```bash
npm run build
```

This generates an optimized build in the `/dist` folder, including the service worker and manifest file required for PWA functionality.


---

## 📲 Installing on Android

1. Open the live Vercel URL in **Chrome on Android**
2. Tap the **three-dot menu** (⋮) in the top-right corner
3. Select **"Add to Home screen"**
4. Confirm the install prompt
5. The app icon will appear on your home screen and launch in fullscreen

---

## 📚 What I Learned

- Building and configuring a **PWA** from scratch using `vite-plugin-pwa`
- How **Service Workers** cache assets and enable offline functionality
- Managing shared state across components using **React Context API**
- Fetching and displaying data from a **REST API** (TVMaze)
- Structuring a **React + Vite** project for scalability
- Deploying a frontend project to **Vercel** with automatic CI/CD

---

## 🔮 Future Improvements

- [ ] Add genre-based filtering and sorting options
- [ ] Persist watchlist data using `localStorage`
- [ ] Add show detail pages with cast, rating, and synopsis
- [ ] Implement pagination or infinite scroll for the show list
- [ ] Add a dark/light theme toggle
- [ ] Write unit tests with React Testing Library

---

## 👨‍💻 Author

**Nipun Induwara**

- GitHub: [@nipuninduwaraedu](https://github.com/nipuninduwaraedu)

---

> ⭐ If you found this project useful or interesting, feel free to star the repo!
