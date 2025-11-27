\# 🎬# 🎬 AI Animation Pipeline — GTI Studios (Space Bear \& Her Kitty Cat Acolytes)



This repository contains the complete AI-assisted animation pipeline used at GTI Studios.  

It provides the technical foundation behind producing animated episodes of \*\*Space Bear \& Her Kitty Cat Acolytes\*\* and related projects using AI-driven tools for voice, animation, automation, and distribution.



This system demonstrates a full production workflow:



Script → Voice Generation → ComfyUI Animation → Editing → Automation → Social Distribution



---



\[Pipeline Overview](docs/pipeline\_overview.md)  

\[Architecture Diagram](docs/architecture\_diagram.txt)



---



\## 📌 Overview



The GTI Studios pipeline integrates multiple AI and automation tools into a unified, production-ready system:



\- \*\*ElevenLabs\*\* for character voice generation  

\- \*\*Custom Python Voice Automation App\*\* for consistent voice output  

\- \*\*ComfyUI\*\* for scene animation, style-locking, and video generation  

\- \*\*n8n\*\* for automated clipping, scheduling, and social platform posting  

\- \*\*Video editing + upscaling\*\* for final assembly and polish  



This repo documents every component used to create animated content end-to-end.



---



\## 🎛 Pipeline Flow



```

1\) Script (episode or short)

2\) ElevenLabs voice generation via GTI Voice App

3\) ComfyUI animation workflows (style-locked scenes)

4\) Frame/video exports

5\) Video editing \& assembly

6\) Upscaling (optional)

7\) n8n automation creates clips \& schedules posts

8\) Daily/weekly posting to social platforms

```



This results in a complete AI-native animation production pipeline.



---



\## 📂 Repository Structure



```

ai-animation-pipeline/

│

├── comfyui/

│   ├── 01\_reference\_setup.json

│   ├── 02\_character\_stylelock.json

│   ├── 03\_action\_scene\_animation.json

│   ├── 04\_lip\_sync\_setup.json

│   └── 05\_video\_patch\_flow.json

│

├── elevenlabs/

│   ├── voice\_profiles\_example.json

│   └── sample\_script\_space\_bear.txt

│

├── n8n/

│   └── youtube\_viral\_clip\_scheduler.json

│

├── examples/

│   └── frames/

│       ├── reactor\_frame\_01.png

│       └── reactor\_frame\_02.png

│

├── docs/

│   ├── pipeline\_overview.md

│   └── architecture\_diagram.txt

│

└── README.md

```



Each folder represents a real production module used at GTI Studios.



---



\## 🎨 ComfyUI Workflows (Animation)



The `comfyui/` folder contains JSON workflows for:



\- \*\*Character style-locking\*\*  

\- \*\*Reference pipelines\*\*  

\- \*\*Action or dialogue scenes\*\*  

\- \*\*Lip-sync preparation\*\*  

\- \*\*Video patching and enhancement\*\*



These are the actual production graphs used to animate Space Bear episodes.



Workflows are intentionally modular so scenes can be re-rendered or updated without rebuilding the entire pipeline.



---



\## 🔊 ElevenLabs Voice Layer (Audio)



The `elevenlabs/` folder contains:



\- Example voice profiles  

\- Sample Space Bear script lines  



These show how GTI Studios generates:

\- Consistent character voices  

\- Scene-specific delivery  

\- Structured filenames ready for editing  



The full voice generation engine lives in a separate repo:  

\*\*`elevenlabs-voice-app`\*\*



---



\## 🤖 Automation Workflows (n8n)



The `n8n/` folder contains the automation engine used for distribution.



\### `youtube\_viral\_clip\_scheduler.json`

This workflow:



1\. Takes a long-form YouTube video  

2\. Automatically analyzes and identifies highlight moments  

3\. Generates \*\*3–6 short viral clips\*\*  

4\. Adds automated captions  

5\. Reformats video for Shorts/Reels/TikTok  

6\. Schedules daily or every-other-day posts  

7\. Auto-publishes clips to:

&nbsp;  - TikTok  

&nbsp;  - Instagram Reels  

&nbsp;  - YouTube Shorts  



This turns a single long-form video into \*\*an entire week of social media growth\*\* with no manual effort.



---



\## 🧠 Skills Demonstrated



\- AI workflow engineering  

\- Production-ready ComfyUI graph design  

\- API-based voice generation pipeline  

\- Automation architecture (n8n)  

\- Video processing \& format conversion  

\- Pipeline documentation \& reproducibility  

\- Real-world media operations  

\- End-to-end system design  

\- Building scalable creative workflows  



This repo demonstrates both technical and creative engineering ability.



---



\## 📚 Documentation



Additional repo documentation is stored in the `docs/` folder:



\### Pipeline Overview  

`docs/pipeline\_overview.md`  

Explains the complete GTI Studios animation process.



\### Architecture Diagram  

`docs/architecture\_diagram.txt`  

ASCII system diagram showing the entire pipeline in one view.



---



\## 🚧 Future Enhancements



\- Additional ComfyUI scene presets  

\- Expanded n8n distribution modules  

\- Thumbnail auto-generation  

\- Lip-sync JSON automation  

\- Script-to-animation batch generation  

\- Multi-show support (Space Bear, Samurai Sass)  

\- Analytics and reporting workflows  



GTI Studios will continue to evolve this pipeline as production scales.



&nbsp;AI Animation Pipeline — GTI Studios (Space Bear \& Her Kitty Cat Acolytes)



This repository contains the complete AI-assisted animation pipeline used at GTI Studios.  

It provides the technical foundation behind producing animated episodes of \*\*Space Bear \& Her Kitty Cat Acolytes\*\* and related projects using AI-driven tools for voice, animation, automation, and distribution.



This system demonstrates a full production workflow:



Script → Voice Generation → ComfyUI Animation → Editing → Automation → Social Distribution



---



\[Pipeline Overview](docs/pipeline\_overview.md)  

\[Architecture Diagram](docs/architecture\_diagram.txt)



---



\## 📌 Overview



The GTI Studios pipeline integrates multiple AI and automation tools into a unified, production-ready system:



\- \*\*ElevenLabs\*\* for character voice generation  

\- \*\*Custom Python Voice Automation App\*\* for consistent voice output  

\- \*\*ComfyUI\*\* for scene animation, style-locking, and video generation  

\- \*\*n8n\*\* for automated clipping, scheduling, and social platform posting  

\- \*\*Video editing + upscaling\*\* for final assembly and polish  



This repo documents every component used to create animated content end-to-end.



---



\## 🎛 Pipeline Flow



```

1\) Script (episode or short)

2\) ElevenLabs voice generation via GTI Voice App

3\) ComfyUI animation workflows (style-locked scenes)

4\) Frame/video exports

5\) Video editing \& assembly

6\) Upscaling (optional)

7\) n8n automation creates clips \& schedules posts

8\) Daily/weekly posting to social platforms

```



This results in a complete AI-native animation production pipeline.



---



\## 📂 Repository Structure



```

ai-animation-pipeline/

│

├── comfyui/

│   ├── 01\_reference\_setup.json

│   ├── 02\_character\_stylelock.json

│   ├── 03\_action\_scene\_animation.json

│   ├── 04\_lip\_sync\_setup.json

│   └── 05\_video\_patch\_flow.json

│

├── elevenlabs/

│   ├── voice\_profiles\_example.json

│   └── sample\_script\_space\_bear.txt

│

├── n8n/

│   └── youtube\_viral\_clip\_scheduler.json

│

├── examples/

│   └── frames/

│       ├── reactor\_frame\_01.png

│       └── reactor\_frame\_02.png

│

├── docs/

│   ├── pipeline\_overview.md

│   └── architecture\_diagram.txt

│

└── README.md

```



Each folder represents a real production module used at GTI Studios.



---



\## 🎨 ComfyUI Workflows (Animation)



The `comfyui/` folder contains JSON workflows for:



\- \*\*Character style-locking\*\*  

\- \*\*Reference pipelines\*\*  

\- \*\*Action or dialogue scenes\*\*  

\- \*\*Lip-sync preparation\*\*  

\- \*\*Video patching and enhancement\*\*



These are the actual production graphs used to animate Space Bear episodes.



Workflows are intentionally modular so scenes can be re-rendered or updated without rebuilding the entire pipeline.



---



\## 🔊 ElevenLabs Voice Layer (Audio)



The `elevenlabs/` folder contains:



\- Example voice profiles  

\- Sample Space Bear script lines  



These show how GTI Studios generates:

\- Consistent character voices  

\- Scene-specific delivery  

\- Structured filenames ready for editing  



The full voice generation engine lives in a separate repo:  

\*\*`elevenlabs-voice-app`\*\*



---



\## 🤖 Automation Workflows (n8n)



The `n8n/` folder contains the automation engine used for distribution.



\### `youtube\_viral\_clip\_scheduler.json`

This workflow:



1\. Takes a long-form YouTube video  

2\. Automatically analyzes and identifies highlight moments  

3\. Generates \*\*3–6 short viral clips\*\*  

4\. Adds automated captions  

5\. Reformats video for Shorts/Reels/TikTok  

6\. Schedules daily or every-other-day posts  

7\. Auto-publishes clips to:

&nbsp;  - TikTok  

&nbsp;  - Instagram Reels  

&nbsp;  - YouTube Shorts  



This turns a single long-form video into \*\*an entire week of social media growth\*\* with no manual effort.



---



\## 🧠 Skills Demonstrated



\- AI workflow engineering  

\- Production-ready ComfyUI graph design  

\- API-based voice generation pipeline  

\- Automation architecture (n8n)  

\- Video processing \& format conversion  

\- Pipeline documentation \& reproducibility  

\- Real-world media operations  

\- End-to-end system design  

\- Building scalable creative workflows  



This repo demonstrates both technical and creative engineering ability.



---



\## 📚 Documentation



Additional repo documentation is stored in the `docs/` folder:



\### Pipeline Overview  

`docs/pipeline\_overview.md`  

Explains the complete GTI Studios animation process.



\### Architecture Diagram  

`docs/architecture\_diagram.txt`  

ASCII system diagram showing the entire pipeline in one view.



---



\## 🚧 Future Enhancements



\- Additional ComfyUI scene presets  

\- Expanded n8n distribution modules  

\- Thumbnail auto-generation  

\- Lip-sync JSON automation  

\- Script-to-animation batch generation  

\- Multi-show support (Space Bear, Samurai Sass)  

\- Analytics and reporting workflows  



GTI Studios will continue to evolve this pipeline as production scales.





