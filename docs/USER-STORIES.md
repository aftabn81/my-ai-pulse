# My AI Pulse — MVP User Stories

## Visitor Stories

| ID | User story | Acceptance criteria |
|---|---|---|
| US-01 | As a busy professional, I want three prioritized AI signals so I can separate signal from noise quickly. | Exactly three cards load; each shows source, title, and why it matters; each expands on tap. |
| US-02 | As a practical learner, I want three activity choices so I can select a move that fits my interest and available time. | Quick Win, Apply It, and Scale It each include a title, instructions, duration, and reusable prompt. |
| US-03 | As a user, I want to copy the prompt so I can use it immediately. | Copy button writes the full prompt to the clipboard and shows confirmation. |
| US-04 | As a returning user, I want to record multiple completed activities so I can see progress from 0/3 through 3/3. | Each completion is saved separately in browser storage, survives refresh, and resets for a new daily pulse. |
| US-05 | As a proud learner, I want share-ready text so I can post my progress. | Share button uses the native share sheet when available and otherwise copies formatted text. |
| US-06 | As a visitor, I want to know the content was prepared automatically so I can trust the always-on claim. | Header displays autonomous status and the latest generation timestamp. |

## Agent Stories

| ID | System story | Acceptance criteria |
|---|---|---|
| AS-01 | As the scheduled agent, I need to collect current public candidates without paid data APIs. | GitHub, Hacker News, and AWS ML Blog collectors run with timeouts and return normalized candidates. |
| AS-02 | As the Signal Engine, I need to rank evidence before using AI so cost stays low. | Duplicates are removed; candidates are scored deterministically; at most five enter the prompt. |
| AS-03 | As the AI formatter, I need to return a consistent pulse. | One Nova Micro call produces three signals and three activities in valid JSON. |
| AS-04 | As the publisher, I need to cache one result for all visitors. | Valid JSON is saved to S3 with a generation timestamp and no-store cache policy. |
| AS-05 | As a resilient agent, I need partial-source failures not to erase the last useful result. | Failed collectors are logged; existing output is preserved when insufficient candidates exist. |
