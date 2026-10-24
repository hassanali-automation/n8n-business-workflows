# n8n Business Workflows

Importable n8n workflows for lead finding, call logging and AI content planning.

| Workflow | What it does | File |
|---|---|---|
| Restaurant Voice Agent Call Logger | Vapi sends an end-of-call report to a webhook, n8n keeps only finished calls and saves the caller number, summary and transcript as a row in Google Sheets | `restaurant-voice-agent-call-logger.json` |
| Cafe Lead Finder | Apify Google Maps scraper collects cafes, an IF node checks the rating, results are saved to Google Sheets and a summary email is sent | `cafe-lead-finder.json` |
| YouTube Shorts Script Agent | Every morning Gemini writes a new Shorts idea with script, video prompt, description and hashtags. It reads past titles to avoid repeats, stores the idea in an n8n Data Table and sends it to Discord | `youtube-shorts-script-agent.json` |

## How to use
1. In n8n: Workflows > Import from file > choose a JSON file.
2. Connect your own credentials (Google Sheets, Gmail, Apify, Gemini, Discord as needed).
3. Replace the placeholders `YOUR_SHEET_ID`, `YOUR_DATA_TABLE_ID`, `YOUR_APIFY_ACTOR_ID` and `you@example.com`.
4. Test with sample data first.

No credentials, keys or personal data are included.

Built by [Hassan Ali](https://github.com/hassanali-automation) · AI Automation Specialist
