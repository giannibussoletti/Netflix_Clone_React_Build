**English** | [Italiano](README.it.md)

# 🎬 Netflix Clone — React (JavaScript)

First version of the Netflix Clone: a front-end application that replicates the Netflix interface, built with **React, JavaScript and Vite**. Movie and TV series data are retrieved from **The Movie Database (TMDB)** APIs.

> 🔄 **This project has a newer version.** It was later fully refactored to **TypeScript**, and the TMDB calls were moved to a dedicated Java Spring back-end that acts as a proxy, so the API key is no longer exposed on the client side.
> New version: [Netflix-Clone-Refactor-JS-to-TS](https://github.com/giannibussoletti/Netflix-Clone-Refactor-JS-to-TS) · [Live demo](https://netflixcloneportfolio.vercel.app/)

---

## ✨ Features

- **Home** — full-screen carousel featuring upcoming movies, followed by carousels of popular movies, top rated TV series and popular TV series
- **TV Shows** — page dedicated to TV series, organized in carousels
- **Movies** — page dedicated to movies, organized in carousels
- **Search** — search bar in the navbar that looks up movies, TV series and people at the same time
- **Details page** — reached from the main carousel or from a poster in the secondary carousels; it shows poster and title logo, plot, release year, runtime, genres and rating
- **Login Page** — purely visual mockup of the Netflix sign-in interface, with no real authentication system
- **Settings** — mockup of the settings page with profiles, account details, subscription plan and language

---

## 🛠️ Tech Stack

- [React](https://react.dev/) 19
- JavaScript (JSX)
- [Vite](https://vitejs.dev/)
- [React Router](https://reactrouter.com/)
- [React Bootstrap](https://react-bootstrap.github.io/) and [Bootstrap](https://getbootstrap.com/)
- [FontAwesome](https://fontawesome.com/)

**Data:** [TMDB API](https://developer.themoviedb.org/reference/intro/getting-started), called directly from the front-end with `fetch`.

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (LTS version recommended) and npm
- A TMDB **API Read Access Token**, which you can get for free from [themoviedb.org/settings/api](https://www.themoviedb.org/settings/api) after creating an account

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/giannibussoletti/Netflix_Clone_React_Build.git
   cd Netflix_Clone_React_Build
   ```

2. Install the dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file in the project root with your TMDB token:

   ```env
   VITE_API_KEY=your_tmdb_api_read_access_token
   ```

4. Start the development server:

   ```bash
   npm run dev
   ```

   The application will be available at [http://localhost:5173](http://localhost:5173).

> ⚠️ In this version the requests to TMDB start from the browser, so the token ends up in the client-side code. That's fine for local use, but it's one of the reasons the project was rebuilt with a back-end proxy in the [TypeScript version](https://github.com/giannibussoletti/Netflix-Clone-Refactor-JS-to-TS).
