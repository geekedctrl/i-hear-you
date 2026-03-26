# I'm Here For You 💛

A minimal, mobile-first emotional support web app designed to make reaching out effortless when you're overwhelmed.

## What is this?

This is a private tool for sending quick emotional support signals to someone you trust. No login, no data storage, no friction—just a few taps to let them know you need them.

**Perfect for:**
- Sharing how you're feeling in the moment
- Requesting immediate support (call, text, or just presence)
- Taking a calming breath when you need a moment
- Communicating when words are hard

## Featuresx

✨ **Minimal & Calming**
- Dark mode with soft pastel colors
- Large, easy-to-tap buttons
- No distracting elements—just what matters

🎯 **Quick to Use**
- 1–2 taps to send a signal
- Optional message field (or leave it blank)
- Smooth, gentle transitions

📳 **Real-Time Notifications**
- Sends notifications via ntfy.sh
- High priority alerts for urgent needs
- Includes intensity level and optional message

🧘 **Self-Care Option**
- 60-second breathing exercise with animated guide
- "You're safe" reassurance text
- Exit anytime

🔒 **Private**
- Nothing is saved
- Just a direct signal to your person
- No accounts, no tracking

## How It Works

1. **Check-in**: "Are you feeling overwhelmed?"
2. **Choose level**: A little / Very / I don't know / No
3. **Select action**: Call / Text / Just be there / Take a moment
4. **Optional message**: Type something or leave blank
5. **Send**: Notification goes to your person via ntfy.sh

## Setup

### Prerequisites
- A GitHub account (for hosting)
- A random ntfy.sh topic (keep it private)

### Step 1: Configure Your ntfy Topic

1. Open `index.html` in a text editor
2. Find line 414: `ntfyTopic: 'suba',`
3. Replace `'suba'` with your random topic (e.g., `'my-secret-topic-abc123'`)
   - Keep it private and hard to guess
   - Share the URL `https://ntfy.sh/your-topic-here` with the person you trust

### Step 2: Deploy to GitHub Pages

1. Create a new GitHub repository (e.g., `confess`)
2. Push this folder to the `main` branch
3. Go to **Settings > Pages**
4. Set source to `main` branch
5. Your app is now live at `https://yourusername.github.io/confess/`

### Step 3: Share the Link

Send the GitHub Pages URL to the person you trust. They can:
- Save it to their home screen
- Access it from any device
- Check for notifications at their ntfy.sh topic URL

## Receiving Notifications

You receive notifications in several ways:

**Option A: Web Dashboard**
- Visit `https://ntfy.sh/your-topic-here` (replace with your topic)
- Notifications appear in real-time
- Keep this tab open or check back anytime

**Option B: Phone App**
- Download the ntfy.sh app (Android/iOS)
- Subscribe to your topic
- Get push notifications

**Option C: Email**
- Subscribe to your topic via email at https://ntfy.sh/your-topic-here

## Design Philosophy

- **Minimal**: Every element serves a purpose
- **Calming**: Soft colors, no sudden changes
- **Accessible**: Large buttons for fingers/thumbs
- **Gentle**: Reassuring language, no judgment
- **Fast**: Reduce friction to asking for help

## Privacy

- ✅ No data is stored anywhere
- ✅ No cookies or tracking
- ✅ No accounts needed
- ✅ Runs entirely in your browser
- ✅ Messages sent only to your ntfy.sh topic

Each person maintains their own ntfy topic—only they know what they're subscribing to.

## Customization

Edit `index.html` to change:

- **Colors**: Edit CSS variables (~line 11–18)
- **Text/wording**: All user-facing text is in the HTML
- **Breathing timer**: Change `60` (~line 476) to a different duration

## How to Test Locally

1. Install Live Server (VS Code extension)
2. Open `index.html` with Live Server
3. Test at `http://localhost:5500`
4. Open browser dev tools (F12) to see console logs
5. Check console for debug messages when sending

## Troubleshooting

**Notifications not sending?**
1. Check browser console (F12) for errors
2. Make sure `CONFIG.ntfyTopic` is set to a valid topic (not `'YOUR_RANDOM_TOPIC'`)
3. Try visiting `https://ntfy.sh/your-topic` to confirm the topic works
4. Ensure you have internet connection

**Buttons not responding?**
- Hard refresh the page (Ctrl+Shift+R on Windows, Cmd+Shift+R on Mac)
- Clear browser cache

**Want to change your ntfy topic?**
- Edit line 414 in `index.html`
- Redeploy to GitHub Pages (push changes)
- Update the URL you share with your person

## Built With

- Pure HTML, CSS, and JavaScript (no dependencies)
- ntfy.sh for push notifications
- GitHub Pages for hosting

## License

MIT – feel free to fork and customize for your needs.

---

**Remember:** You're never a burden. This app exists because someone cares. 💛
