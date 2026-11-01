# Velvet

A private AI character chat app for iPhone. It installs from Safari like a normal app. Your characters, chats and
API key stay on the phone. Messages go only to the AI service you pick.

**Live app:** https://ntrslover67-spec.github.io/velvet/

## Install it on the iPhone

Open the link in **Safari** → **Share** → **Add to Home Screen** → **Add**. Always open Velvet from the home-screen
icon. It runs full screen, and its data belongs to that icon: **deleting the icon deletes your chats**, so export a
backup first (Settings → Export backup).

## Connect an AI

1. Sign up at openrouter.ai → **Credits** → add a few dollars. Most roleplay models cost a few cents per long chat.
2. Go to openrouter.ai/keys → **Create key** → copy it.
3. In Velvet: **Settings** → paste the key → **Browse** → pick a model → **Test connection**.

**Choosing a model:** on openrouter.ai/models, set **Categories → Roleplay** and sort by **Top Weekly**. Open-weight
models (Llama, Mistral, Qwen, DeepSeek and their roleplay fine-tunes) usually handle adult scenes. Models from OpenAI,
Anthropic and Google refuse explicit content. If a model gets prudish, dull or repetitive, try another one. That
makes a bigger difference than any setting.

**Privacy:** in OpenRouter's account settings (Privacy), you can switch off providers that may log or train on prompts.

## Features

- **Discover**: 26 built-in characters (anime, fantasy, realistic, sci-fi, supernatural), each with their own voice,
  quirks and two stories to start from. Filter by category or search.
- **Stories**: every character can have several opening scenarios. Start as many separate chats as you like (⋯ → All chats).
- **Steer the story** (⋯ menu): set reply length and a director's note ("slow burn", "add a twist"…) that guides
  every reply until you clear it.
- **Memory** (⋯ menu): pinned memories, plus an automatic "story so far" that gets written as long chats outgrow the
  AI's memory, so characters don't forget what happened.
- **💡 Reply ideas**: three suggested replies in your voice. Tap one to drop it into the message box.
- **Message menu** (tap a message): copy, edit, read aloud, continue a cut-off reply, new reply, rewind, delete.
  Swipe left on the latest reply for another version, and swipe right to go back.
- **Less robotic replies**: writing rules in the system prompt, a list of overused phrases to avoid, a note that
  stops the character opening every reply the same way, and sampling settings (Settings → Less repetitive replies).
- **Read aloud**: each character gets their own iPhone voice. You can turn on auto-read in Settings.
- **App lock**: a 4-digit PIN, which also hides chats in the app switcher.
- **Your own characters**: create them (photo, emoji, tags, stories, example dialogue, voice, per-character model),
  import SillyTavern/Chub cards (PNG or JSON), and export your own as cards.
- **Backup**: export and import everything as one file.

## Updating

Upload changed files to the GitHub repository (Add file → Upload files). The phone gets the new version the next
time you open Velvet while online.
