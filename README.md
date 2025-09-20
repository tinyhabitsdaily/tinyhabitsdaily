# TinyHabitsDaily Website

A beautiful landing page for the TinyHabitsDaily iOS app - showcasing tiny steps for massive results in habit formation.

## 🚀 Live Website

Visit: [https://tinyhabitsdaily.app](https://tinyhabitsdaily.app)

## 📱 Features

- Responsive design optimized for all devices
- Interactive screenshot gallery
- Smooth animations and transitions
- App Store download integration
- Modern, clean UI following iOS design principles

## 🛠 Deployment

This website is automatically deployed to GitHub Pages using GitHub Actions.

### GitHub Pages Setup

1. The site deploys automatically from the `main` branch
2. Custom domain configured via `CNAME` file
3. GitHub Actions workflow handles the deployment process

### DNS Configuration (Porkbun)

To route your custom domain through Porkbun:

1. **A Records** (for apex domain):
   ```
   Type: A
   Host: @
   Answer: 185.199.108.153
   
   Type: A
   Host: @
   Answer: 185.199.109.153
   
   Type: A
   Host: @
   Answer: 185.199.110.153
   
   Type: A
   Host: @
   Answer: 185.199.111.153
   ```

2. **CNAME Record** (for www subdomain):
   ```
   Type: CNAME
   Host: www
   Answer: tinyhabitsdaily.github.io
   ```

## 📁 Project Structure

```
├── index.html              # Main landing page
├── CNAME                   # Custom domain configuration
├── Screenshots/            # App screenshots
│   └── AppStore/          # App Store optimized images
├── TinyHabitsDaily/       # App assets
│   └── Assets.xcassets/   # App icon and assets
└── .github/
    └── workflows/
        └── deploy.yml     # GitHub Actions deployment
```

## 🔧 Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/tinyhabitsdaily/tinyhabitsdaily.git
   cd tinyhabitsdaily
   ```

2. Open `index.html` in your browser or use a local server:
   ```bash
   python -m http.server 8000
   # or
   npx serve .
   ```

## 📝 License

© 2024 TinyHabitsDaily. All rights reserved.
