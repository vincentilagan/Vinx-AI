# VinX-AI — AI-Powered Blender Addon

Control Blender with natural language using **Claude, ChatGPT, DeepSeek, or Gemini** — all in one free addon.

![VinX-AI Banner](https://vixels.site/vinx-ai/assets/og-image.png)

---

## What it does

Type what you want. VinX-AI sends it to your chosen AI provider, gets back Blender Python code, and executes it directly in your scene — automatically, step by step, until the task is done.

No coding required. Just bring your API key.

---

## Supported Providers

| Provider | Models |
|----------|--------|
| OpenAI | gpt-4.1, gpt-4.1-mini, gpt-4o |
| Anthropic Claude | claude-opus-4-7, claude-sonnet-4-6, claude-haiku-4-5 |
| DeepSeek | deepseek-chat, deepseek-reasoner |
| Google Gemini | gemini-2.0-flash, gemini-1.5-pro |

---

## Features

- Multi-provider support — switch between AI providers anytime
- Agentic loop — keeps executing until the task is complete
- Scene context awareness — reads your current scene before responding
- Reference image support — show the AI what you want
- User identity memory — remembers your name across sessions
- No subscriptions, no telemetry, no locked features

---

## Installation

**Blender 4.2+ (Extensions)**

1. Download `Vinx-AI.zip` from the [releases page](https://github.com/yourusername/VinX-AI/releases) or [vixels.site/vinx-ai](https://vixels.site/vinx-ai/)
2. Open Blender → Edit → Preferences → Add-ons → Install from Disk
3. Select the zip file → Enable the addon

**Blender 3.6 – 4.1 (Legacy)**

Same steps — the addon is compatible with both formats.

---

## Setup

1. Open Blender → Sidebar (N key) → **BlenderGPT** tab
2. Go to **Settings**
3. Choose your AI provider
4. Paste your API key
5. Select your model
6. Type a prompt and click **Execute**

API keys are saved locally on your machine — never sent anywhere except directly to the AI provider you choose.

---

## Usage

```
"Create a forest scene with 50 trees randomly scattered"
"Add a sun lamp at 45 degrees and render to /tmp/test.png"
"Make the selected object look like rusted metal"
```

The AI reads your current scene, writes the Python code, and runs it. If something fails, it tries again automatically.

---

## Sample Videos

- [How to Create a Forest Scene](https://youtu.be/ZUvcYHyQI3M)
- [Orange Render Sample](https://youtu.be/t_sMvzlCCFM)
- [Feature Overview](https://youtu.be/Msbd4MbBcu0)

---

## Project History

- **April 19, 2026** — VinX-AI v3 created, multi-provider support added
- **April 18, 2026** — First successful agentic test run
- **Earlier** — Original VinX-GPT with memory brain, local GGUF model, full learning system

The original version had a full memory/learning brain (learned skills, error memory, event logs). v3 strips that down to a lean, fast Blender control bridge — smooth AI-to-Blender communication, nothing else.

---

## File Structure

```
VinX-AI V3/
├── __init__.py
├── blender_manifest.toml
├── core/
│   ├── ai_engine.py      # Multi-provider API calls + agentic loop
│   ├── prefs.py          # Preferences + API key storage
│   ├── executor.py       # Blender Python execution
│   ├── scene_templates.py
│   └── user_profile.py   # Name + session memory
└── ui/
    └── panel_main.py     # Sidebar panel
```

---

## License

GPL-3.0 — free to use, modify, and distribute.

---

## Author

**Vincent Ilagan**
[vixels.site](https://vixels.site) · [vfxverse25@gmail.com](mailto:vfxverse25@gmail.com)

If this tool helped you, consider supporting via PayPal — my mother is currently hospitalized and every bit helps. Thank you.
