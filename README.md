# Velvet: setup

A private AI character chat app for your iPhone. It installs from Safari like a normal app. Your characters,
chats and API key stay on the phone. Messages go only to the AI service you pick.

## 1. Put it online (free, one time): GitHub Pages

1. Sign up at github.com (free).
2. Top right **+** → **New repository** → name it `velvet` → **Public** → **Create repository**.
3. Click **uploading an existing file** and drag in everything from this folder (`index.html`, `sw.js`,
   `manifest.webmanifest` and the `icons` folder; `README.md` is optional) → **Commit changes**.
4. In the repository, go to **Settings → Pages**, set Branch to **main** and the folder to **/ (root)**, then **Save**.
   After about a minute the app is live at `https://YOUR-USERNAME.github.io/velvet/`.

Anyone can see the code, but there's nothing personal in it. Your data never leaves the phone, and the page asks
search engines not to list it.

## 2. Install it on the iPhone

Open that link in **Safari** → **Share** → **Add to Home Screen** → **Add**. Always open Velvet from the home-screen
icon. It runs full screen, and its data belongs to that icon: **deleting the icon deletes your chats**, so export a
backup first (Settings → Export backup).

## 3. Connect an AI

1. Sign up at openrouter.ai → **Credits** → add a few dollars. Most roleplay models cost a few cents per long chat.
2. Go to openrouter.ai/keys → **Create key** → copy it.
3. In Velvet: **Settings** → paste the key → **Browse** → pick a model → **Test connection**.

**Choosing a model:** on openrouter.ai/models, set **Categories → Roleplay** and sort by **Top Weekly** to see what
people use for roleplay. Open-weight models (Llama, Mistral, Qwen, DeepSeek and their roleplay fine-tunes) usually
handle adult scenes. Models from OpenAI, Anthropic and Google refuse explicit content. If a model gets prudish or
dull, switch models. That makes a bigger difference than anything else.

**Privacy:** in OpenRouter's account settings (Privacy), you can switch off providers that may log or train on prompts.

## Using it

- **+** on the home screen: create a character, or import a character card (PNG or JSON in the
  SillyTavern / Chub format).
- Tap any message to copy, edit, delete it, or rewind the chat to that point.
- Swipe left on the latest reply (or tap ↻) to get a different version. Swipe right to go back.
- **⋯** in a chat → **Memory**: facts the character should always remember. Also **Start a new chat**.
- Settings: your name and persona, creativity, reply length, how much history the AI sees, and the roleplay
  instructions sent with every chat.

## Updating

Upload the changed files to the same GitHub repository. The phone gets the new version the next time you open
Velvet while online.

## Quick try without GitHub (home Wi-Fi only, PC must stay on)

```
python -m http.server 8790 --directory C:\Users\frynz\velvet
```

Allow it through the Windows firewall if Windows asks. Then on the iPhone, open `http://YOUR-PC-IP:8790`. You can find
the PC's IP address with `ipconfig`. In this mode, Copy and offline start don't work, because those need https.
