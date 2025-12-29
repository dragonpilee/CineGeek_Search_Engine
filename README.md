# 🎬 CineGeek Search Engine

A minimalist, Google-inspired search engine for Movies and TV Series. Built with **Astro**, **Docker**, and **TMDb**.

![CineGeek Search](https://i.imgur.com/example-screenshot.png) 
*(Replace with actual screenshot)*

## ✨ Features

*   **Unified Search**: Intelligent search bar that automatically detects Movies and TV Series.
*   **Google-Style Design**: Clean, centered, and dark-themed (`#202124`) interface.
*   **Multi-Source Streaming**: Aggregates up to 4 reliable streaming sources:
    *   🔴 Source 1: `vidsrc.xyz`
    *   🔵 Source 2: `vidsrc.to`
    *   🟢 Source 3: `2embed.cc`
    *   🟡 Source 4: `vidsrc.cc`
*   **Responsive**: Fully optimized for mobile, tablet, and desktop.
*   **Dockerized**: Run anywhere with a single command.

## 🚀 Quick Start (Docker)

The easiest way to run CineGeek is with Docker.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/dragonpilee/CineGeek_Search_Engine.git
    cd CineGeek_Search_Engine
    ```

2.  **Create a `.env` file:**
    Copy the example env file and add your TMDb API Key.
    ```bash
    cp .env.example .env
    # Edit .env and set PUBLIC_TMDB_API_KEY=your_key_here
    ```

3.  **Run with Docker Compose:**
    ```bash
    docker compose up -d --build
    ```

4.  **Open in Browser:**
    Visit `http://localhost:8080`

## 🛠️ Development

To run locally without Docker:

1.  **Install Dependencies:**
    ```bash
    npm install
    ```

2.  **Start Dev Server:**
    ```bash
    npm run dev
    ```

## 📦 Deployment

### Netlify

This project is configured for easy deployment on Netlify.

1.  Push your code to GitHub.
2.  Import the project in Netlify.
3.  Set the **Build Command** to `npm run build`.
4.  Set the **Publish Directory** to `dist`.
5.  **Important**: Add `PUBLIC_TMDB_API_KEY` in Netlify's **Site Settings > Build & Deploy > Environment variables**.

## 📝 Configuration

### API Keys
This app requires a [TMDb API Key](https://www.themoviedb.org/documentation/api).
Set it in your `.env` file:

```ini
PUBLIC_TMDB_API_KEY=your_api_key_here
```

## 📄 License

Developed with ❤️ by CineGeek.
© 2025 CineGeek. All rights reserved.
