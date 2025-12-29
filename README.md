# CineGeek Search Engine 🎬
> **Minimalist Unified Streaming Interface**

![Status](https://img.shields.io/badge/Status-Production-success?style=for-the-badge) ![Docker](https://img.shields.io/badge/Deployment-Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white) ![Astro](https://img.shields.io/badge/Framework-Astro-ff5d01?style=for-the-badge&logo=astro&logoColor=white) ![TypeScript](https://img.shields.io/badge/Language-TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

**CineGeek** is a privacy-focused, Google-inspired search engine for Movies and TV Series. Built for simplicity and speed, it aggregates multiple streaming sources into a single, unified interface that automatically detects content types and delivers instant playback.

---

## ✨ Features

- **🔍 Unified Search**: Intelligent input that automatically distinguishes between Movies and TV Series
- **🎨 Google-Style Design**: Clean, distraction-free interface with deep dark mode (`#202124`)
- **🌊 Multi-Source Aggregation**: 4 reliable streaming sources for maximum availability (`vidsrc`, `2embed`, etc.)
- **📱 Fluid Responsiveness**: Optimized layout that adapts seamlessly from mobile phones to desktops
- **⚡ Reactive UI**: Smooth fade-in animations and hover effects for a premium feel
- **🔌 Dockerized**: Plug & Play deployment with a single command
- **🛡️ Secure Config**: API keys managed via environment variables for safety

---

## 🚀 Quick Start

### Prerequisites

1.  **Docker Desktop**: Ensure Docker is running.
2.  **Git**: To clone the repository.
3.  **TMDb API Key**: Get one from [themoviedb.org](https://www.themoviedb.org/documentation/api).

### Installation & Run

1.  Clone the repository:
    ```bash
    git clone https://github.com/dragonpilee/CineGeek_Search_Engine.git
    cd CineGeek_Search_Engine
    ```

2.  **Configure Environment** (Critical):
    Create a `.env` file in the root directory:
    ```env
    PUBLIC_TMDB_API_KEY=your_tmdb_api_key_here
    ```

3.  Build and launch the container:
    ```bash
    docker compose up -d --build
    ```

4.  Open your browser and visit:
    **[http://localhost:8080](http://localhost:8080)**

### Docker Commands

```bash
# Restart containers
docker compose restart

# Stop containers
docker compose down

# View logs
docker compose logs -f
```

---

## 🛠️ Technology Stack

| Component | Technology |
|----------|------------|
| **Frontend Framework** | Astro |
| **Language** | TypeScript / JavaScript |
| **Styling** | Vanilla CSS (Scoped) |
| **Data Provider** | TMDb API |
| **Infrastructure** | Docker (Multi-stage Node/Nginx) |

---

## 📱 Mobile Access

CineGeek is designed to look great on your phone.

1.  **Find your PC IP**: Run `ipconfig` (Windows) or `ifconfig` (Mac/Linux).
2.  **Connect**: Navigate to `http://YOUR_PC_IP:8080` on your phone.
3.  **Experience**: The layout automatically adjusts margins, fonts, and button sizes for touch interaction.

---

## 🎨 Design Philosophy

- **Minimalism**: Removing clutter to focus entirely on the search experience
- **Familiarity**: Mimicking the widely loved "Google Dark" aesthetic for instant usability
- **Feedback**: Subtle animations provide visual confirmation of actions without slowing you down
- **Robustness**: Multiple fallback sources ensure you always find a working stream

---

## 🎯 How It Works

1.  **Search**: Author types a query (e.g., "Breaking Bad" or "Inception").
2.  **Detect**: The app queries TMDb to determine if it is a Movie or a TV Show.
3.  **Fetch**: Metadata is retrieved, and streaming links are generated for 4 different providers.
4.  **Play**: User selects a source (🔴, 🔵, 🟢, 🟡) to start streaming immediately.

---

## 📝 License

This project is open source.

---

<div align="center">
  <sub>Developed with ❤️ by CineGeek</sub><br>
  <sub>Minimalist Search Interface • Dockerized Deployment</sub>
</div>
