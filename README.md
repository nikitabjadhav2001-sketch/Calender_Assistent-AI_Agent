# Calender_Assistent-AI_Agent

Welcome! This is my first AI Agent workflow created with n8n.
Instead of just chatting or writing text, this AI agent actually uses tools to take real actions for me automatically.

💡 What Does This Workflow Do?
Every day, the workflow runs on a set schedule and completes four main steps:
Checks Google Calendar to see all scheduled events for the day.
Picks the 2 most important events.
Explains why these two meetings or tasks matter most.
Sends a summary email directly to my Gmail inbox.

⚙️ How the Workflow Works
Here is a simple flow of how the steps connect:
[ Schedule Trigger ]
         │
         ▼
    [ AI Agent ]
    ↙          ↘
[ Google ]    [ Gmail ]
[Calendar]


Explanation of Components:
Schedule Trigger: Starts the process automatically at a specific time each day.
AI Agent: The "brain" that reads the calendar data and decides what is important.
Google Calendar Tool: Fetches the list of events for the current day.
Gmail Tool: Sends the final summary email.

🛠️ Tools & Technologies Used
n8n: The platform used to build and visually manage the workflow.
Groq: Fast AI model provider used by the AI Agent to think and evaluate.
Google Calendar API: Used to read daily calendar events.
Gmail API: Used to send out the final email.
