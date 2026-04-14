# CineSearch - Phase 2

CineSearch is a movie discovery web application built using Next.js and React. Users can search for movies, view details, add movies to Favorites, and save movies to a Watch Later list.

## Features

- Search movies by title
- View movie details
- Add/remove Favorites
- Add/remove Watch Later
- Dynamic routing for movie details
- Responsive layout

## Routes

- `/` → Home page (search and movie list)
- `/favorites` → Favorite movies
- `/watch-later` → Watch Later movies
- `/movies/[id]` → Movie details page

## Components

- Navbar → navigation menu
- Footer → footer section
- SearchBar → search input
- MovieList → list of movies
- MovieCard → displays each movie
- SummaryCard → small info cards
- EmptyState → message when no data

## State Management

The application uses React Context API to manage shared state:

- favorites
- watchLater

Functions allow adding and removing movies from these lists.

Data is stored in localStorage to persist after refresh.

## API Preparation

A file `movieService.ts` was created to prepare future API integration.

Currently, it uses local data but can be replaced with a real API in Phase 3.

## How to Run

```bash
npm install
npm run dev
