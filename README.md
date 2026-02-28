# 03-react-movies

A movie search application built with React, TypeScript, and the [TMDB API](https://www.themoviedb.org/).

![React](https://img.shields.io/badge/React-18-61DAFB?logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript)
![Vite](https://img.shields.io/badge/Vite-5-646CFF?logo=vite)

## Features

- Search movies by keyword using the TMDB API
- Responsive movie grid with poster images
- Modal with full movie details — backdrop image, overview, release date, and rating
- Modal closes on close button click, `ESC` key, or outside click
- Toast notifications for empty search query or no results found
- Loading and error states handled gracefully

## Tech Stack

| Tool | Purpose |
|------|---------|
| React 18 | UI library |
| TypeScript | Type safety |
| Vite | Build tool |
| Axios | HTTP requests |
| React Hot Toast | Toast notifications |
| CSS Modules | Component scoped styles |
| Modern Normalize | Cross-browser style reset |

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/03-react-movies
cd 03-react-movies
```

### 2. Install dependencies

```bash
npm install
```

### 3. Set up environment variables

Create a `.env` file in the project root:

```
VITE_TMDB_TOKEN=your_tmdb_bearer_token_here
```

> To get your token: register at [themoviedb.org](https://www.themoviedb.org/) → Settings → API → copy the **API Read Access Token** (the long `eyJ...` token, not the short API Key)

### 4. Start the development server

```bash
npm run dev
```

## Project Structure

```
src/
├── components/
│   ├── App/
│   │   ├── App.tsx
│   │   └── App.module.css
│   ├── SearchBar/
│   │   ├── SearchBar.tsx
│   │   └── SearchBar.module.css
│   ├── MovieGrid/
│   │   ├── MovieGrid.tsx
│   │   └── MovieGrid.module.css
│   ├── MovieModal/
│   │   ├── MovieModal.tsx
│   │   └── MovieModal.module.css
│   ├── Loader/
│   │   ├── Loader.tsx
│   │   └── Loader.module.css
│   └── ErrorMessage/
│       ├── ErrorMessage.tsx
│       └── ErrorMessage.module.css
├── services/
│   └── movieService.ts
├── types/
│   └── movie.ts
└── main.tsx
```

## Available Scripts

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run preview  # Preview production build
```

## Environment Variables

| Variable | Description |
|----------|-------------|
| `VITE_TMDB_TOKEN` | TMDB API Read Access Token (Bearer) |

## Live Demo

[View on Vercel](#) https://03-react-movies-wine-rho.vercel.app/
