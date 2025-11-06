Deep Feedback Thematic & Sentiment Analyzer with AI Insight
Steps:

Manual Trigger

Set Node – Paste the following vertical-style JSON array:

[
  {
    "User": "Alice",
    "Topic": "Support",
    "Feedback": "Very satisfied with the service."
  },
  {
    "User": "Bob",
    "Topic": "Product",
    "Feedback": "Quality could be better."
  },
  {
    "User": "Chloe",
    "Topic": "Delivery",
    "Feedback": "Fast but packaging was poor."
  },
  {
    "User": "Derek",
    "Topic": "Support",
    "Feedback": "Average experience overall."
  }
]
Function Node

Cluster feedback by Topic
Identify repeat submitters
Gemini Node – Prompt:
"Analyze feedback grouped by Topic, label each item for sentiment (Positive, Neutral, Negative), and synthesize key improvement themes. Highlight repeat submitters and topics with most negative sentiment. Output summary, actionable advice, and a one-line improvement plan for each topic."

Result:

Sentiment summary by topic
Thematic insights (main issues, strengths)
Actionable improvement lines per topic
List of repeat submitters and “problem” areas