---
layout: modlist
modlist: everwild
title: Everwild: SkyrimNet
---

# SkyrimNet (AI NPCs)

This section is for the SkyrimNet profile only and is not required if you're not on that profile.

SkyrimNet lets NPCs hold real conversations using AI. It needs a few pieces to work: an **LLM** (the brain, writes the dialogue), **TTS** (the voice) and **STT** (speech-to-text, only needed if you want to talk using your microphone). You can run each piece in the cloud (paid) or on your own PC (local), and mixing the two is totally fine.

You must pick **one** of the three options below. Everything is configured from the SkyrimNet dashboard.

> **THIS IS REQUIRED AND A SEPARATE DOWNLOAD FROM THE MODLIST:** <https://developer.nvidia.com/cuda-downloads>

## Step 1: First Launch

1. Launch Everwild through MO2 as normal and wait until the game is running (the main menu is fine). **The game must be running before the dashboard will load.**
2. SkyrimNet generates working default settings on first launch.
3. Once the game is running, open your web browser and go to `http://localhost:8080/` (or use the Open Dashboard entry in SkyrimNet's in-game wheel menu).
4. Follow the guided setup wizard, then continue to Step 2 below.

## Step 2: Start a New Game and Install the Addons

1. In-game, select **New Game** (or load your save) so SkyrimNet is fully active.
2. Once the new game is selected, go back to the SkyrimNet dashboard in your browser (`http://localhost:8080/`) and refresh the page.
3. At the **top of the page**, let it **install the addons**. Wait for the install to finish before continuing.
4. Then pick one of the options below to set up your LLM, voice and speech settings.

## Option A: Fateless (Recommended, easiest)

Fateless is SkyrimNet's own official service. One account covers everything SkyrimNet needs: dialogue, voices, speech recognition and bard songs. There are no API keys to manage, no other accounts to make and nothing to configure. The models are tuned for each job, so NPCs reply fast and stay in character. Because it all runs in the cloud, it barely affects your PC's performance.

1. Make sure SkyrimNet is **Beta29 or later** (you can check the version in your MO2 mod list).
2. Create an account at <https://fateless.ai>
3. On your account page, **pick a plan** (plans start at $10 a month) or **buy credit**.
4. Launch Everwild through MO2 as normal.
5. Open the SkyrimNet settings, choose **Fateless** as your provider and **sign in**.
6. Use the **Quick Setup** block on the dashboard Home page to test that dialogue and voice respond.
7. Load your save and talk to an NPC. That's it!

Tips:

- Fateless is optional. You can still use your own provider or run models locally.
- You can mix and match, for example Fateless for dialogue and a local engine for voices.
- Never share your Fateless login with anyone, including in Discord support posts.

## Option B: Other Paid / Cloud Providers

If you'd rather pick your own models, you can use your own API key. This is a bit more work than Fateless but gives you full control over which models you use and what you pay.

1. Go to <https://openrouter.ai> and make an account.
2. Add credits to your account (a few dollars lasts a long time) and create an **API key**.
3. In the SkyrimNet setup wizard (or in the dashboard under Providers → OpenRouter) paste in your key.
4. Pick a model. SkyrimNet ships with approved **presets** at several price points, so choose one of those if you're unsure. You can use a cheap, fast model for actions and a smarter model for dialogue.
5. Use the **Quick Setup** block on the dashboard Home page to test that your LLM responds.

Tips:

- Your key is stored once, so you don't have to re-enter it for each feature.
- The **Logs → API Requests** page shows what every request cost.
- Never share your API key with anyone, including in Discord support posts.
- NanoGPT, Nvidia NIM, Chutes or any custom OpenAI-compatible endpoint work the same way.

Cloud voice options (optional, paid): ElevenLabs and Inworld both support voice cloning.

## Option C: Local Hosting (free, but needs a strong PC)

Local hosting costs nothing per message, but the AI model has to share your graphics card with Skyrim. A heavily modded game already uses a lot of VRAM, so only do this if you have a high-end GPU (or a second PC on your network). Small local models give simpler conversations than Fateless or a cloud model.

**Local LLM**

1. Install a local model server such as **LM Studio** or **Ollama**.
2. Download a model and start the server. Small models such as **NVIDIA Nemotron 3.5 Bolt** are a good way to try SkyrimNet on an RTX GPU.
3. In the SkyrimNet dashboard, add a **custom provider** (OpenAI-compatible) and point it at your server:
   - LM Studio: `http://127.0.0.1:1234/v1`
   - Ollama: `http://localhost:11434/v1`
4. Enter the exact model name your server shows, and use any placeholder text for the API key if asked.
5. Test it with the Quick Setup block on the Home page.

If you have a second PC, run the server there and use that PC's LAN address instead of 127.0.0.1.

**Local Voice (TTS)**

- **Piper**: runs on your CPU inside the game, no GPU needed. Easiest choice, but no voice cloning.
- **PocketTTS**: runs locally with live voice cloning (GPU optional). Supports English, Spanish, French, German, Italian and Portuguese.
- **XTTS**: runs on a server you choose (your PC, your LAN, or a rented cloud GPU).

**Local Speech-to-Text (microphone)**

- SkyrimNet uses local **Whisper** by default and auto-downloads the model. It uses CUDA, Vulkan, OpenCL or CPU, whichever your PC supports.
- Smaller models are faster, bigger ones are more accurate. Cloud speech-to-text also works but is noticeably slower.

## Which one should I pick?

| | Fateless | Other cloud (OpenRouter etc.) | Local |
|---|---|---|---|
| Setup difficulty | Easiest (sign in) | Easy | Moderate |
| Cost | From $10/month | Small per-message cost | Free |
| PC requirements | Low | Low | RTX GPU recommended |
| Covers dialogue, voice and speech | Yes, one account | Dialogue (voice sold separately) | You set up each piece |

Not sure? Start with Fateless. If you later want more control, you can switch to your own provider or a local setup in the dashboard.

## SkyrimNet not working?
Join the discord and head to the support section. Please include your SkyrimNet log from the dashboard (and remove any API key or login details first).
