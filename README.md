# AI-Powered-Automation-Workflow-Agent
🧭 Project Overview

This automation workflow uses n8n (an open-source automation tool) to fetch the latest drone-related news, summarize it using ChatGPT (OpenAI API), generate social media captions, and automatically post them to LinkedIn/Twitter every day.

The goal is to build a fully automated AI agent that handles content discovery, summarization, and posting — without manual effort.

⚙️ Workflow Summary
Step	Node Name	Function
1	Schedule Trigger	Runs the workflow automatically every day at 9:00 AM IST.
2	RSS Feed Read	Fetches the 3–5 latest drone-related news articles from Google News RSS feed.
3	OpenAI (Summarizer)	Uses GPT model to summarize each article in 2–3 short paragraphs and extract keywords/hashtags.
4	OpenAI (Caption Generator)	Formats the summary into a social-media-ready caption with hashtags and a link.
5	HTTP Request / Twitter Node	Posts the final caption to LinkedIn or Twitter using their respective APIs.
6	Email / Telegram Node (optional)	Sends a daily summary report of posted articles to the admin.
🧩 APIs & Keys Used
Service	Purpose	Required Key
OpenAI API	Text summarization and caption generation	OpenAI API Key
Twitter API	Auto-post to Twitter (X)	Developer API Key + Access Token
LinkedIn API	Auto-post to LinkedIn	Access Token + Profile ID
Email/Telegram (optional)	Send daily report	SMTP or Bot Token
📆 Automation Schedule

Trigger: Every day at 9:00 AM IST

Runs automatically — no manual start required.

Posts 3–5 summarized drone news updates daily.

📸 Documentation Screenshots

Include the following:

Full n8n Workflow Canvas view (showing all connected nodes).

Output logs from summarization and caption nodes.

Post success log (showing “Execution Successful” or API response).

(Optional) Screenshot or link to the actual LinkedIn/Twitter post.

✅ Expected Output Example

Generated Caption Example:

🚁 India’s drone sector continues to expand with new DGCA policies promoting local innovation.
The latest guidelines are expected to boost commercial drone adoption.
#DroneNews #DGCA #Aviation #Innovation #TechTrends
Read more 👉 [news link]

💡 Conclusion

This workflow demonstrates the use of AI + Automation for smart content curation.
It showcases:

Integration of AI models with real-time data

Automated social media content generation

End-to-end posting without manual steps
