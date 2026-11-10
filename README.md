# Kitty AI Companion (`v1.0.0`)

**Desktop companion, instant hold-to-speak voice typing, and AI text enhancer for Windows (10 / 11 · 64-bit).**

Kitty sits cleanly on your desktop and lets you hold **Caps Lock** to dictate anywhere, or highlight text and press **`F7` / `F8` / `F9`** to fix grammar, engineer AI prompts, or polish writing across any app.

---

## Download (`v1.0.0`)

Choose the download that fits your setup — **most users should choose the Installer**:

| Option | File | Size | Best For |
|---|---|---|---|
| **Option 1: Windows Installer *(Recommended)*** | [**KittySetup.exe**](https://github.com/Divyaraj94/kitty-releases/releases/latest/download/KittySetup.exe) | ~65 MB | **All regular Windows users.** Quick setup wizard, no admin password needed, Start Menu & optional Desktop/Startup icons, easy uninstall, and smooth future updates. |
| **Option 2: Portable Zip *(Optional — No-Install)*** | [**Kitty-Portable.zip**](https://github.com/Divyaraj94/kitty-releases/releases/latest/download/Kitty-Portable.zip) | ~90 MB | **Locked-down PCs or no-install use.** Just unzip anywhere and double-click `Kitty.exe` without running an installer *(manual updates by re-extracting)*. |

- **Browse All Releases & Release Notes:** [Releases Page](https://github.com/Divyaraj94/kitty-releases/releases)
- **System Requirements:** Windows 10 or Windows 11 (64-bit / x64), plus a working microphone for Voice Typing.

---

## Step 1: Install & Launch Kitty

### Option 1 — Windows Installer (`KittySetup.exe`) *(Recommended)*
1. Download [**KittySetup.exe**](https://github.com/Divyaraj94/kitty-releases/releases/latest/download/KittySetup.exe).
2. Double-click `KittySetup.exe`.
   - *If Windows SmartScreen shows **"Windows protected your PC"**:* click **More info** → **Run anyway**.
3. Follow the quick setup steps (admin rights are **not** required — Kitty installs cleanly under `%LOCALAPPDATA%\Programs\Kitty`).
4. Optionally check **Create a desktop shortcut** or **Launch Kitty automatically when Windows starts**, then finish to launch Kitty.

### Option 2 — Portable Zip (`Kitty-Portable.zip`) *(No-Install)*
1. Download [**Kitty-Portable.zip**](https://github.com/Divyaraj94/kitty-releases/releases/latest/download/Kitty-Portable.zip).
2. Right-click `Kitty-Portable.zip` → **Extract All...** into a regular folder (for example on your Desktop or Documents).
3. Open the extracted `Kitty` folder and double-click **`Kitty.exe`**.
   - *If Windows SmartScreen prompts:* click **More info** → **Run anyway**.

Once launched, Kitty the cat appears on your desktop. Click and drag her anywhere on your screen!

---

## Step 2: One-Time Free Setup (Cloud or Offline Mode)

Single-click **Kitty** on your desktop to open **Settings**. Choose either mode below:

### Option A: Cloud Mode *(Recommended — Fastest, Voice Typing + AI Text Hotkeys)*
1. At the top of Settings, keep **Cloud API** selected.
2. Under **Cloud Provider**:
   - **Groq (Ultra-Fast LPU)** *(Recommended free starter)* or **Gemini (Google Multimodal Voice)** — both support **Voice Typing + AI Text Hotkeys** and offer free API keys with no credit card required.
   - *(**OpenAI** and **Anthropic Claude** keys are also supported for `F7` / `F8` / `F9` AI Text Hotkeys.)*
   - *Tip:* If you add **both** a Groq key and a Gemini key, Kitty automatically falls back to Gemini if Groq hits a rate limit.
3. Click the green **Free Key ↗** button next to Groq or Gemini → sign in with Google → create and copy your API key.
4. Paste the key into Kitty and click **Save Settings ↗**. Kitty plays a happy animation when ready!

### Option B: Offline / Local Mode *(100% Private, No Internet — AI Text Hotkeys Only)*
> **Note:** Local Ollama powers **`F7` / `F8` / `F9` AI text hotkeys** completely offline on your PC. Hold-to-speak **Voice Typing** requires a free Groq or Gemini Cloud API key.

1. At the top of Settings, switch to **Local (Ollama)**.
2. If Ollama isn't installed yet, click **Get Ollama (Free) ↗**, install Ollama once, and reopen Kitty Settings.
3. Pick a starter model (`qwen2:1.5b` ~900 MB recommended, `qwen2:0.5b` ~350 MB, or `llama3` ~4.7 GB) and click **Download Model ⬇** right inside Kitty.
4. Once Ollama shows active, click **Save Settings ↗**.

---

## Step 3: How to Use Kitty

### 1. Hold-to-Speak Voice Typing (`Caps Lock` default)
1. Click your cursor inside **any app** (WhatsApp, Gmail, Chrome, Word, VS Code, Notepad, etc.).
2. **Hold down `Caps Lock`** (quick taps under ~0.35s cancel automatically so normal typing stays safe).
3. Speak naturally in **English, Hindi, Gujarati, or a natural mix** — a live soundwave pill appears while Kitty listens.
4. **Release `Caps Lock`** — Kitty cleans filler words, fixes punctuation, and types the text right at your cursor.

**Built-in Voice Commands:**
- Say **`"new line"`** or **`"enter"`** → inserts a line break.
- Say **`"new paragraph"`** → inserts a blank line / new paragraph.
- Say **`"scratch that"`** or **`"cancel that"`** → cancels dictation without pasting.
- **Spoken Lists:** Say *"we need three things: first debug, second test, third deploy"* and Kitty formats it into neat list lines.

### 2. AI Text Magic Hotkeys (`F7` / `F8` / `F9`)
Highlight any text anywhere on Windows and press:
- **`F7` — Fix Grammar:** Fixes spelling, punctuation, and grammar while keeping your meaning.
- **`F8` — Prompt Agent:** Turns rough notes into a clear, structured AI prompt.
- **`F9` — Mix Polish:** Rewrites text cleanly in a crisp, concise tone.

### 3. Smart Features & Controls
- **App-Aware Tone** *(on by default)*: Automatically adapts output style for code editors (VS Code / terminals), chat apps (WhatsApp / Slack), email (Gmail / Outlook), and AI chats.
- **Custom Shortcuts:** Customize `Hold to Speak`, `F7`, `F8`, `F9`, or toggle hotkeys anytime in Settings → **Automation & Shortcuts**.
- **Dictation Hub:** Click Kitty → **Dictation Hub** (or System Tray → **Dictation History Hub**) to view past transcripts, speaking speed (WPM) & word counts, and click **Copy ↗** anytime.
- **Built-in Guide:** Click Kitty → **How to Use** anytime inside the app.

---

## Updates, Data, Exiting & Uninstalling

- **Where Your Data Lives:** Settings, Windows DPAPI-encrypted API keys (protected for your Windows user account), and local dictation history stay safely in `%APPDATA%\Kitty` (`settings.json` and `kitty_history.sqlite`). Installing future updates preserves all your data.
- **Checking for Updates:** Kitty checks quietly at startup. You can also click the **`v1.0.0`** badge in Settings (or right-click the System Tray icon → **Check for Updates...**).
- **Exiting Kitty:** Right-click the **Kitty** icon in the Windows System Tray (bottom-right near the clock — click `^` if hidden) → **Exit**.
- **Uninstalling / Removing:**
  - *Installer (`KittySetup.exe`):* Windows **Settings → Apps → Installed apps → Kitty AI Companion → Uninstall** (or use the Start Menu uninstall shortcut).
  - *Portable (`Kitty-Portable.zip`):* Exit Kitty from the System Tray and delete the extracted `Kitty` folder.

---

## Troubleshooting

- **Windows SmartScreen shows *"Windows protected your PC"*:** Click **More info** → **Run anyway**.
- **Holding `Caps Lock` didn't paste anything:** Make sure you **hold** `Caps Lock` while speaking (rather than tapping briefly), check your default Windows microphone, and confirm a **Groq** or **Gemini** key is saved in Settings.
- **Hotkeys don't respond in an Administrator app:** Windows blocks normal-privilege global hotkeys inside elevated (`Run as Administrator`) windows. Use Kitty with standard-privilege apps.
- **Can't see the Kitty tray icon:** Click the small `^` arrow in the bottom-right Windows taskbar near the clock.
