# TimeBridge

A no-login required link generator for global time coordination. Perfect for scheduling events across different time zones without the headache.

## Features

- **Simple Event Creation**: Enter an event title and date/time in under 10 seconds
- **URL Hash Encoding**: Event data is encoded directly in the URL hash - no database required
- **Automatic Time Zone Conversion**: Viewers see the event time in their local time zone automatically
- **Live Countdown Timer**: Real-time countdown showing days, hours, minutes, and seconds
- **Add to Calendar**: One-click integration with Google Calendar and iCal downloads
- **No Login Required**: Share links instantly without forcing recipients to create accounts
- **Fully Responsive**: Works perfectly on desktop, tablet, and mobile devices

## How It Works

1. **Creator**: Enter event title and date/time, click "Generate Link"
2. **Share**: Copy the generated URL and share it with anyone
3. **Receiver**: Click the link to see the event in their local time zone with a live countdown

## Tech Stack

- **Frontend**: HTML, CSS (Tailwind CSS), Vanilla JavaScript
- **Time Handling**: Day.js with UTC and Timezone plugins
- **Hosting**: Can be deployed to Vercel, Netlify, or GitHub Pages (100% free)

## Local Development

1. Clone or download this repository
2. Open `index.html` in your browser
3. No build process or dependencies required!

## Deployment (Best Free Options)

### 🚀 Vercel (Recommended - Best for Global Performance)

**Why Vercel:**
- Global CDN with edge network (fastest worldwide)
- Free SSL certificates
- Custom domain support
- Automatic HTTPS
- Git integration for continuous deployment
- Best performance for static sites

**Steps:**
1. Go to [vercel.com](https://vercel.com) and sign up
2. Install Vercel CLI: `npm i -g vercel`
3. Run in project directory: `vercel`
4. Follow the prompts (select default settings)
5. Your site will be live at `https://your-project.vercel.app`

**Custom Domain:**
- Purchase a domain (e.g., from Namecheap, GoDaddy)
- Add domain in Vercel dashboard
- Update DNS records as instructed

### ⚡ Netlify (Excellent Alternative)

**Why Netlify:**
- Global CDN
- Free SSL and custom domains
- Drag-and-drop deployment
- Form handling (if needed later)
- Git integration

**Steps:**
1. Go to [netlify.com](https://netlify.com) and sign up
2. Drag and drop the project folder to Netlify's dashboard
3. Or use CLI: `npm install -g netlify-cli` then `netlify deploy`
4. Your site will be live at `https://random-name.netlify.app`

### 📦 GitHub Pages (Simple but Limited)

**Why GitHub Pages:**
- Completely free
- Integrated with GitHub
- Good for personal projects

**Limitations:**
- No custom domain on free tier (must pay for custom domain)
- Slower than Vercel/Netlify
- Limited to GitHub infrastructure

**Steps:**
1. Push code to GitHub repository
2. Go to Settings > Pages
3. Select main branch and save
4. Site will be at `https://username.github.io/repository-name`

## SEO Optimization

The site includes comprehensive SEO features:

### Implemented SEO Features:
- **Meta Tags**: Title, description, keywords optimized for search engines
- **Open Graph Tags**: For social media sharing (Facebook, LinkedIn)
- **Twitter Cards**: For Twitter sharing with rich previews
- **Structured Data (JSON-LD)**: Helps search engines understand the application
- **Sitemap.xml**: Helps search engines discover and index the site
- **Robots.txt**: Guides search engine crawlers
- **Canonical URL**: Prevents duplicate content issues
- **Responsive Design**: Mobile-friendly (Google ranking factor)

### SEO Checklist Before Launch:
- [ ] Update `https://timebridge.com` to your actual domain in meta tags
- [ ] Create and upload `og-image.png` (1200x630px) for social sharing
- [ ] Create and upload `twitter-image.png` (1200x600px) for Twitter
- [ ] Create and upload `favicon.ico` for browser tab icon
- [ ] Submit sitemap to Google Search Console
- [ ] Submit sitemap to Bing Webmaster Tools
- [ ] Add domain to Google Search Console for monitoring

### Submit to Search Engines:
1. **Google Search Console**: 
   - Go to [search.google.com/search-console](https://search.google.com/search-console)
   - Add your property (domain)
   - Verify ownership
   - Submit sitemap: `sitemap.xml`

2. **Bing Webmaster Tools**:
   - Go to [bing.com/webmasters](https://www.bing.com/webmasters)
   - Add your site
   - Verify ownership
   - Submit sitemap

## URL Structure

The event data is encoded in the URL hash using base64 encoding:
```
https://yourdomain.com/#event-eyJ0aXRsZSI6IkNvYWNoZWxsYSBMaXZlIFN0cmVhbSIsInRpbWVzdGFtcCI6MTc4MjM5NDgwMH0=
```

This approach eliminates the need for a backend database while keeping the URLs shareable.

## Customization

- Modify the gradient colors in the `.gradient-bg` CSS class
- Adjust the default event duration in the `downloadICS()` function (currently set to 1 hour)
- Change the countdown styling in the `.countdown-digit` CSS class
- Update SEO meta tags with your actual domain and branding

## Performance Tips

- The site is already optimized with CDN-hosted libraries
- No build step required for deployment
- Static files load instantly from edge networks
- Consider adding a service worker for offline support (PWA)

## License

MIT License - Feel free to use and modify as needed.
