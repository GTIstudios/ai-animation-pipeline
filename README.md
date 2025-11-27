# 🎬 AI Animation Pipeline — GTI Studios (Space Bear & Her Kitty Cat Acolytes)

End-to-end AI animation pipeline used at **GTI Studios** to produce episodes of  
**Space Bear & Her Kitty Cat Acolytes** and related projects.

This repo documents the full production flow:

Script → ElevenLabs Voice → ComfyUI Animation → Automation (n8n) → Final Edit

It’s designed to show how modern AI tools can be combined into a **repeatable, production-grade pipeline** for animated content.

---

## 📌 Overview

This pipeline ties together multiple tools:

- **ElevenLabs** — character voice generation  
- **Custom Python TTS App** — (see: `elevenlabs-voice-app` repo)  
- **ComfyUI** — image-to-image, animation, style-lock, reactor scenes  
- **n8n** — automation (episode processing, YouTube uploads, file routing)  
- **Video Editing / Upscaling** — DaVinci / Topaz / other tools

The goal:  
**Turn scripts into finished animated episodes using AI-assisted workflows.**

---

## 🧱 High-Level Flow

```text
1) Write script (Space Bear episode or scene)
2) Generate voices with ElevenLabs + custom TTS app
3) Build shots & sequences in ComfyUI (style-locked)
4) Combine audio + visual timing (lip-sync / edit)
5) Upscale and finalize video
6) Automate exports / uploads with n8n
```

This repo contains **the JSON graphs, example configs, and documentation** for that process.

---

## 📂 Repository Structure

```text
ai-animation-pipeline/
│
├── comfyui/                  # Core ComfyUI workflows
│   ├── 01_stylelock_character.json
│   ├── 02_shot_animation.json
│   └── 03_reactor_scene.json
│
├── elevenlabs/               # Voice configuration examples
│   ├── voice_profiles_example.json
│   └── sample_script_space_bear.txt
│
├── n8n/                      # Automation workflows
│   ├── youtube_autoupload.json
│   └── episode_pipeline.json
│
├── docs/                     # Additional documentation & diagrams
│   ├── pipeline_overview.md
│   └── assets/
│       ├── pipeline_overview.png
│       └── scene_flow.png
│
├── examples/                 # Visual output samples (frames/clips)
│   ├── frames/
│   │   ├── reactor_frame_01.png
│   │   └── reactor_frame_02.png
│   └── clips/
│       └── reactor_scene_preview.mp4   (optional)
│
└── README.md
```

---

## 🎛 Tool Breakdown

### 🔊 Voice: ElevenLabs + Voice Automation App

The audio layer is handled by a custom Python tool:

- Repo: `elevenlabs-voice-app` (separate project)
- Role: generate character voices for:
  - Captain Bear
  - Onyx
  - Other Space Bear characters
  - Samurai Sass and beyond

Example assets in this repo:

- `elevenlabs/voice_profiles_example.json`
- `elevenlabs/sample_script_space_bear.txt`

These illustrate how voices and scripts are structured before animation.

---

### 🎨 Visuals: ComfyUI Workflows

The **`comfyui/`** folder contains JSON exports of real production graphs used for:

- Style-locking Space Bear and cat characters  
- Building shot templates (camera, lighting, FX)  
- Specific scenes (e.g., the reactor dance room)

Typical steps encoded in these graphs:

1. Load base character (or style-locked reference)
2. Apply animation / frame interpolation
3. Add lighting, FX, and scene-specific elements
4. Output frames or short clips

These workflows are meant to be **loaded directly into ComfyUI** for inspection.

---

### 🤖 Automation: n8n

The **`n8n/`** folder holds workflow exports that automate:

- Episode asset handling  
- YouTube upload preparation  
- File renaming and routing  
- Potential integration with future distribution flows

Examples:

- `youtube_autoupload.json` — scaffold for automated uploads  
- `episode_pipeline.json` — per-episode processing flow

---

## 🔍 Example Use Case (Space Bear Episode)

```text
1) Draft script for a 10-minute Space Bear episode
2) Use ElevenLabs Voice App to generate character lines
3) Feed timing + audio into ComfyUI for shot animation
4) Use specific ComfyUI graphs for:
     - Exterior shots
     - Reactor room dance scene
     - Dialogue close-ups
5) Export frames or video segments
6) Open in editor / upscaler for:
     - Final timing
     - Color / sound pass
7) Run n8n workflow to:
     - Prepare thumbnails / titles
     - Upload draft or final episode to YouTube
```

This repo documents **the “how”**, not just the buzzwords.

---

## 🧠 Skills Demonstrated

- AI workflow design & orchestration  
- ComfyUI graph design for animation and style consistency  
- Integration of TTS (ElevenLabs) into visual pipelines  
- Automation using n8n for content operations  
- Structuring complex projects into modular, reusable components  
- Documenting production-grade AI pipelines for others to follow

---

## 📝 Extended Description

The AI Animation Pipeline is the backbone of GTI Studios’ AI-native production process.  
Instead of treating tools like ElevenLabs, ComfyUI, or n8n as isolated experiments, this project shows how they are **wired together into a repeatable, end-to-end system** for animated storytelling.

The pipeline was built to:

1. **Move fast without sacrificing quality**  
   Scenes can be rebuilt, re-voiced, or re-rendered without restarting from scratch.

2. **Keep characters visually and vocally consistent**  
   Style-lock graphs and voice profiles ensure that Space Bear and her Kitty Cat Acolytes look and sound the same from episode to episode.

3. **Automate the boring parts**  
   Uploads, file renaming, asset routing, and other repetitive steps are pushed into n8n automation workflows.

4. **Scale across multiple shows**  
   While Space Bear is the primary use case, the same pipeline structure can be adapted to Samurai Sass or any future GTI Studios IP.

This repo is a **blueprint** for anyone wanting to use AI tools not just as toys, but as part of a real production environment.

---

## 🚧 Future Enhancements

- [ ] Add more ComfyUI graphs (lip-sync specific, camera motion presets)  
- [ ] Add detailed timing docs for audio → animation alignment  
- [ ] Include links to public example scenes on YouTube  
- [ ] Expand n8n workflows for multi-platform distribution  
- [ ] Add step-by-step setup guide for a fresh environment  

---
