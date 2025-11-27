\# AI Animation Pipeline – Overview



This document explains the full production pipeline used at GTI Studios to create animated content for Space Bear \& Her Kitty Cat Acolytes and related IP. The goal is to show how voice, animation, automation, and distribution tools work together as a unified system.



---



\## 1. High-Level Workflow



1\. Script creation  

2\. Voice generation using ElevenLabs and the GTI Voice Automation App  

3\. Animation scenes produced in ComfyUI  

4\. Frame or video outputs prepared for editing  

5\. Optional upscaling and enhancement  

6\. Assembly in video editor  

7\. Automated clip generation and scheduling using n8n  

8\. Daily or weekly publishing of shorts and episodes



This system turns individual tools into a repeatable animation production pipeline.



---



\## 2. Modules in the Pipeline



\### 2.1 Voice Generation (ElevenLabs)

\- Character profiles maintained externally

\- Audio lines generated through the GTI Voice App

\- Filenames structured for editing and lip-sync



\### 2.2 Animation (ComfyUI)

\- Style-locked character templates

\- Separate workflows for action, dialogue, and scene-specific effects

\- JSON graphs exported as reusable production assets



\### 2.3 Automation (n8n)

\- Long video → viral clips

\- Caption generation

\- Cross-platform posting

\- Scheduled content calendar



\### 2.4 Editing / Assembly

\- Scenes combined, timed, and finalized in a video editor

\- Optional upscaling using Topaz or ComfyUI video tools



---



\## 3. Folder Breakdown



\### comfyui/

Contains production-ready scene and animation graphs used to render character motions, FX, and full scenes.



\### elevenlabs/

Provides example voice profiles and sample script text for demonstration.



\### n8n/

Houses workflows that automate content scheduling, posting, clipping, and distribution.



\### examples/

Offers reference imagery or frame exports taken from real production renders.



---



\## 4. Production Philosophy



1\. Keep everything modular  

2\. Store all configurations in human-readable formats  

3\. Use automation wherever possible  

4\. Maintain character consistency through style-locks  

5\. Build the pipeline to scale across multiple shows



---



\## 5. Future Additions



\- Expanded ComfyUI flows

\- More automation templates

\- Lip-sync metadata generation

\- Script-to-scene batch generation

\- Production metrics and reporting



This document will grow as GTI Studios evolves the pipeline.



