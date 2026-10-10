# WhisperGuard

A discreet voice activated safety assistant. This is a simulation for a hackathon demo: nothing is recorded, nobody is called, and no message is sent anywhere. The whole app runs in the browser as a single page.

## Deploy on Maritime

1. Push this folder to a GitHub repo.
2. Deploy it as a public app:

```bash
npm install -g maritime-cli
maritime login
maritime create whisperguard --repo https://github.com/YOUR_USERNAME/whisperguard --public --port 3000
maritime status whisperguard
```

3. When the status shows active, open the public URL and click Play demo.

No API keys or environment variables are needed.

## Run locally

```bash
docker build -t whisperguard .
docker run -p 3000:3000 whisperguard
```

Then open http://localhost:3000

## Code phrases

Escape call: "did I leave the oven on"
Full alert: "remind me to buy blueberries"
All clear: "I found my keys"

All three can be changed in Settings on the page.
