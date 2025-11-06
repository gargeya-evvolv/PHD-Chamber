# Labs


## 1. Advanced Task Manager + AI Prioritization & Recommendation

**Steps:**

1. **Manual Trigger**

2. **Set Node** – Paste the following vertical-style JSON array:
    ```
    [
      {
        "Task": "Prepare compliance report",
        "Priority": "High",
        "Status": "Pending",
        "Tags": [
          "Compliance",
          "Finance"
        ],
        "Dependencies": [
          "Get sales data"
        ]
      },
      {
        "Task": "Schedule team meeting",
        "Priority": "Medium",
        "Status": "Done",
        "Tags": [
          "Management"
        ],
        "Dependencies": []
      },
      {
        "Task": "Review customer feedback",
        "Priority": "High",
        "Status": "In Progress",
        "Tags": [
          "Customer",
          "Insights"
        ],
        "Dependencies": [
          "Get last week's feedback"
        ],
        "EstimatedTime": "2h"
      }
    ]
    ```

3. **IF Node/Function Node**  
   - Flag tasks blocked by incomplete dependencies  
   - Cluster tasks by tag

4. **Gemini Node** – Prompt:  
   *"Given this detailed list, analyze urgency and strategic value based on Priority, Status, Dependency, and Tags. Recommend an optimal order of execution, flag blocked tasks, surface strategic tasks for management attention, and output in readable list format."*

5. **Result:**  
   - Ordered priority task plan  
   - Blocked tasks flagged  
   - Strategic recommendations

***

## 2. Smart Email Thread Analyzer & AI Action Suggestion

**Steps:**

1. **Manual Trigger**

2. **Set Node** – Paste the following vertical-style JSON array:
    ```
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
    ```

3. **Function Node**  
   - Group emails by thread  
   - Extract sequence and last sender  
   - Analyze overdue responses

4. **Gemini Node** – Prompt:  
   *"Review these email threads, identify which require urgent reply, generate suggested follow-up templates for each, and highlight long-unanswered client emails. Return thread summary and action items for my team."*

5. **Result:**  
   - Summary of the conversation  
   - Action recommendations (who should reply, why)  
   - Ready-to-send email response drafts

***

## 3. Deep Feedback Thematic & Sentiment Analyzer with AI Insight

**Steps:**

1. **Manual Trigger**

2. **Set Node** – Paste the following vertical-style JSON array:
    ```
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
    ```

3. **Function Node**  
   - Cluster feedback by Topic  
   - Identify repeat submitters

4. **Gemini Node** – Prompt:  
   *"Analyze feedback grouped by Topic, label each item for sentiment (Positive, Neutral, Negative), and synthesize key improvement themes. Highlight repeat submitters and topics with most negative sentiment. Output summary, actionable advice, and a one-line improvement plan for each topic."*

5. **Result:**  
   - Sentiment summary by topic  
   - Thematic insights (main issues, strengths)  
   - Actionable improvement lines per topic  
   - List of repeat submitters and “problem” areas

***

> **If you encounter any difficulties, please remember that our team is here to support you. If you need access to our instance or further assistance, don’t hesitate to reach out to any of our colleagues nearby—they will be happy to help.**
>
> *Hack:* Simply copy and paste the entire lab text into n8n’s Build with AI module to proceed.
>
> **Happy evolving!**

