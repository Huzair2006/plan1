# Plan1 - With Vercel Speed Insights

This project is now configured with Vercel Speed Insights for performance monitoring.

## Vercel Speed Insights Integration

Vercel Speed Insights has been successfully integrated into this project to track Core Web Vitals and performance metrics.

### What was installed:
- `@vercel/speed-insights` package (v1.1.0)

### How it works:
The Speed Insights tracking script is included in `index.html` using the vanilla JavaScript integration method:

```html
<script>
  window.si = window.si || function () { (window.siq = window.siq || []).push(arguments); };
</script>
<script defer src="/_vercel/speed-insights/script.js"></script>
```

### Setup Instructions:

1. **Enable Speed Insights on Vercel Dashboard:**
   - Go to your Vercel project dashboard
   - Navigate to Speed Insights from the sidebar
   - Click "Enable" to activate Speed Insights
   - This will add the `/_vercel/speed-insights/*` routes after your next deployment

2. **Deploy the project:**
   ```bash
   vercel deploy
   ```
   Or push to your connected Git repository for automatic deployment

3. **Monitor Performance:**
   - After deployment, visit your site to generate traffic
   - View performance metrics in the Vercel Dashboard under Speed Insights
   - Metrics will become visible after several days of visitor traffic

## Project Structure

- `index.html` - Main HTML file with Speed Insights integration
- `package.json` - Project configuration with @vercel/speed-insights dependency
- `vercel.json` - Vercel deployment configuration
- Media files: `camel.png`, `HafizUzair.jpeg`, `videoplayback.m4a`

## Local Development

```bash
# Install dependencies
npm install

# Serve the project locally
npm run dev

# Build (for this static project, just echoes "Build complete")
npm run build
```

## Performance Tracking

Once deployed on Vercel with Speed Insights enabled, this project will automatically track:
- Largest Contentful Paint (LCP)
- First Input Delay (FID)
- Cumulative Layout Shift (CLS)
- First Contentful Paint (FCP)
- Time to First Byte (TTFB)
- Interaction to Next Paint (INP)

All metrics are collected in accordance with the official Vercel Speed Insights documentation.
