# Campus Route Optimizer

A smart Next.js app that helps you find the best path across campus using 3 different algorithmic approaches. Built as part of AlgoNet Hackathon for the Design & Analysis of Algorithms course (CSET244).

## What it does

Given a start and end point, the app shows you:

- **Shortest Route** — via Dijkstra’s algorithm  
- **Least Crowd Path** — via a greedy approach  
- **Most Chill Route** — via DFS with chill heuristics  

All 3 routes are displayed with their respective values so users can pick based on mood or urgency.

## Tech Stack

- **Framework**: Next.js (TypeScript)
- **Styling**: Tailwind CSS
- **UI Components**: shadcn/ui
- **Algorithms**: Dijkstra, Greedy, DFS

## Features

- Clean and responsive UI  
- Dynamic graph logic with weighted paths  
- Uses React state for live updates  
- Easily extendable to real-world applications (campus maps, city routing, etc.)

## Setup & Run

```bash
npx create-next-app@latest campus-route-optimizer --typescript
cd campus-route-optimizer

# Tailwind setup
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p

# Edit tailwind.config.ts
# Add in content: ["./app/**/*.{js,ts,jsx,tsx}", "./components/**/*.{js,ts,jsx,tsx}"]

# Setup Tailwind in app/globals.css
@tailwind base;
@tailwind components;
@tailwind utilities;

# shadcn/ui setup
npx shadcn-ui@latest init
npx shadcn-ui@latest add card button

# Run app
npm run dev