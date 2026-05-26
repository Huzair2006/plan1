# Plan1

A simple web project with Vercel Speed Insights integration.

## Features

- ⚡ Vercel Speed Insights for real-time performance monitoring
- 🎨 Modern, responsive design
- 🚀 Built with Vite for optimal performance

## Setup

Install dependencies:

```bash
npm install
```

## Development

Run the development server:

```bash
npm run dev
```

## Build

Build for production:

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

## Vercel Speed Insights

This project includes Vercel Speed Insights to track real-world performance metrics. The Speed Insights component is initialized in `main.js` using:

```javascript
import { injectSpeedInsights } from '@vercel/speed-insights';
injectSpeedInsights();
```

To view Speed Insights data:
1. Deploy this project to Vercel
2. Enable Speed Insights in your Vercel dashboard
3. Visit your deployed site to generate traffic
4. View metrics in the Vercel Speed Insights dashboard

## Deployment

Deploy to Vercel:

```bash
npm install -g vercel
vercel
```

Or connect your GitHub repository to Vercel for automatic deployments.
