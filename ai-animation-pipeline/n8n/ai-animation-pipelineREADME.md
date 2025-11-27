\## 🤖 Automation Workflows (n8n)



This folder contains the automation layer of the GTI Studios production pipeline.  

These workflows handle repetitive, time-consuming, or error-prone tasks that occur during episode creation, processing, and distribution.



All workflows were exported directly from the live GTI Studios n8n Docker instance using:



```

n8n export:workflow --all --decrypted --output=/home/node/.n8n/exported\_workflows

```



\### Included Workflows



\#### `workflow\_1.json` (rename according to purpose)

This workflow automates part of the GTI Studios episode production process.  

Depending on the version exported, this file may include steps such as:



\- Automated asset collection  

\- File routing and renaming  

\- Episode scaffolding  

\- YouTube metadata generation  

\- Upload preparation or triggering  

\- Notification or reporting nodes  

\- Integration points with other parts of the pipeline



Once identified, this workflow should be renamed to reflect its exact purpose:



Example renames:

\- `youtube\_autoupload.json`  

\- `episode\_builder.json`  

\- `asset\_pipeline.json`  

\- `postproduction\_automation.json`  



\### Purpose of n8n in This Pipeline



n8n acts as the \*\*orchestration system\*\* connecting the voice generation layer, visual animation layer, and final distribution layer.  



Key responsibilities:

\- Moving files automatically between tools  

\- Triggering workflow sequences  

\- Preparing uploads in the background  

\- Structuring episode folders  

\- Ensuring consistent naming for audio → animation → editing  

\- Reducing manual redundant effort during production  



By treating n8n as part of the animation pipeline itself, GTI Studios can maintain consistent production cycles while reducing the amount of manual overhead needed to complete each episode.



\### Usage Notes



\- These JSON files can be imported directly into any n8n instance via \*\*Import Workflow → Upload File\*\*.

\- They are provided for documentation, reproducibility, and employer review.

\- Sensitive connection credentials have been excluded to prevent exposure of private environment variables.



\### Future Expansion



\- Additional automation pipelines for multi-platform distribution  

\- Workflow to auto-generate thumbnails and metadata  

\- Batch-render or batch-upload orchestration  

\- Episode completion metrics and tracking  

\- Slack/Discord notifications for production events  



The n8n folder represents the automation backbone that allows GTI Studios to scale the animation process beyond single episodes into a repeatable, production-ready operation.



