Advanced Task Manager + AI Prioritization & Recommendation
Steps:

Manual Trigger

Set Node – Paste the following vertical-style JSON array:

text
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
IF Node/Function Node

Flag tasks blocked by incomplete dependencies

Cluster tasks by tag

Gemini Node – Prompt:
"Given this detailed list, analyze urgency and strategic value based on Priority, Status, Dependency, and Tags. Recommend an optimal order of execution, flag blocked tasks, surface strategic tasks for management attention, and output in readable list format."

Result:

Ordered priority task plan

Blocked tasks flagged

Strategic recommendations