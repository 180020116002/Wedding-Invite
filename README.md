# Sam & Sofia Wedding Invitation 💍

A luxury Indian wedding invitation website with AI chatbot, animated event cards, ring toss game, scratch-reveal coins, and more.

## Deploy to Vercel

### 1. Push to GitHub
```bash
git init
git add .
git commit -m "Sam & Sofia wedding invitation"
git remote add origin https://github.com/YOUR_USERNAME/vivah-wedding.git
git push -u origin main
```

### 2. Connect to Vercel
1. Go to [vercel.com](https://vercel.com) → **New Project**
2. Import your GitHub repository
3. Vercel auto-detects the config — click **Deploy**

### 3. Add your Anthropic API Key
1. In Vercel dashboard → your project → **Settings** → **Environment Variables**
2. Add: `ANTHROPIC_API_KEY` = `sk-ant-...your key...`
3. Click **Save** then **Redeploy**

That's it! The AI chatbot will now work via the secure `/api/chat` serverless route.

## Project Structure
```
vivah-wedding/
├── public/
│   └── index.html          ← The full wedding invitation
├── api/
│   └── chat.js             ← Serverless API proxy for Anthropic
├── vercel.json             ← Vercel routing config
└── README.md
```

## Features
- 🎭 Lottie curtain reveal animation
- 🪙 Scratch-to-reveal date coins  
- 💌 5 sticky event cards with animated backgrounds (Celebration, Mehndi, Haldi, Sangeet, Reception)
- ⏳ Live countdown to the wedding
- 💍 Ring Toss mini-game (popup)
- 🤖 AI Vivah chatbot (bottom-right, appears after curtain opens)
- 📍 Venue, Gifts, Transport, RSVP sections
