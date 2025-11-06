Smart Email Thread Analyzer & AI Action Suggestion
Steps:

Manual Trigger

Code Node – Paste the following vertical-style JSON array:

[
  {
    "Sender": "client@biz.com",
    "Subject": "Project Kickoff",
    "Body": "Let's schedule a call.",
    "ThreadId": "A"
  },
  {
    "Sender": "client@biz.com",
    "Subject": "RE: Project Kickoff",
    "Body": "Could you send over the agenda?",
    "ThreadId": "A"
  },
  {
    "Sender": "hr@company.com",
    "Subject": "Welcome",
    "Body": "Here are your onboarding steps.",
    "ThreadId": "B"
  }
]
Function Node

Group emails by thread
Extract sequence and last sender
Analyze overdue responses
Gemini Node – Prompt:
"Review these email threads, identify which require urgent reply, generate suggested follow-up templates for each, and highlight long-unanswered client emails. Return thread summary and action items for my team."

Result:

Summary of the conversation
Action recommendations (who should reply, why)
Ready-to-send email response drafts