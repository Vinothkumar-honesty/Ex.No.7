# Exno.7-Develop a prompt-based application tailored to their personal needs, fostering creativity and practical problem-solving skills while leveraging the capabilities of large language models.

# Date:19.05.2026
# Register no.:212224040361
# Aim: To develop a prompt-based application using ChatGPT - To demonstrate how to create a prompt-based application to organize daily tasks, showing the progression from simple to more advanced prompt designs and their corresponding outputs.

#AI Tools Required: 


# Explanation: 
Prompt:
"Design a personal productivity assistant that can help manage daily tasks, schedule reminders, suggest wellness tips, and answer general queries. The assistant should interact using natural language and be adaptable to the user’s changing preferences over time."
Procedure:
1. Define the core requirements of a personal productivity assistant.
2. Identify and construct appropriate prompts for each task using an LLM (e.g., ChatGPT).
3. Simulate natural user interaction through a simple interface or command-line system.
4. Collect feedback or inputs from users and adapt responses accordingly.
5. (Optional) Integrate basic memory to simulate preference adaptation.
EXPECTED OUTPUT: - (attached the drive link)
Output (Example Response by LLM):
Personal Productivity Assistant Features:
1. Daily Task Manager:
o Accept tasks via natural language (e.g., "Remind me to call mom at 6 PM").
o Organize tasks by priority and deadline.
o Provide daily summaries and pending items.
2. Smart Scheduler:
o Schedule events and set reminders using contextual understanding.
o Notify user of overlapping appointments or free time slots.
3. Wellness Tips Generator:
o Suggest daily wellness advice (hydration, exercise, screen-time breaks).
o Adapt suggestions based on past user preferences and responses.


# Explanation: 
Prompt:
"Design a personal productivity assistant that can help manage daily tasks, schedule reminders, suggest wellness tips, and answer general queries. The assistant should interact using natural language and be adaptable to the user’s changing preferences over time."
Procedure:
1. Define the core requirements of a personal productivity assistant.
2. Identify and construct appropriate prompts for each task using an LLM (e.g., ChatGPT).
3. Simulate natural user interaction through a simple interface or command-line system.
4. Collect feedback or inputs from users and adapt responses accordingly.
5. (Optional) Integrate basic memory to simulate preference adaptation.
EXPECTED OUTPUT: - (attached the drive link)
Output (Example Response by LLM):
Personal Productivity Assistant Features:
1. Daily Task Manager:
o Accept tasks via natural language (e.g., "Remind me to call mom at 6 PM").
o Organize tasks by priority and deadline.
o Provide daily summaries and pending items.
2. Smart Scheduler:
o Schedule events and set reminders using contextual understanding.
o Notify user of overlapping appointments or free time slots.
3. Wellness Tips Generator:
o Suggest daily wellness advice (hydration, exercise, screen-time breaks).
o Adapt suggestions based on past user preferences and responses.
### Output
# 🚀 Project Title

### **Prompt-Based Task Organizer using ChatGPT**
# 🎯 Objective

To demonstrate how to **create a prompt-driven system that organizes daily tasks**, evolving **step-by-step**:

1. **Basic Prompting**
2. **Structured Output Prompting**
3. **Context-aware Prompting**
4. **Memory & iterative planning**
5. **Full Application-Style Prompt Flow**

---

## 1️⃣ Basic Prompt – Task List Generation

**Goal**: Provide ChatGPT with tasks, get a simple organized list.

**Prompt Example**

```
I need help organizing my day. Here are my tasks:
- Study Machine Learning
- Grocery shopping
- Gym workout
- Complete college assignment
- Call my friend
Arrange them in order of productivity with morning, afternoon, evening schedule.
```

**Possible Output**

```
📅 Daily Schedule

Morning:
1. Study Machine Learning
2. Complete college assignment

Afternoon:
3. Grocery shopping
4. Call your friend

Evening:
5. Gym workout
```

---

## 2️⃣ Intermediate Prompt – Add Priority, Duration & Reminders

**Prompt**

```
Organize my tasks into a schedule. Assign priorities (High/Medium/Low),
estimate duration, and add reminder times to keep me on track.

Tasks:
1) Study Machine Learning – 2 hours
2) Grocery shopping – 1 hour
3) Gym workout – 1.5 hours
4) Assignment – 3 hours
5) Call friend – 30 min
Plan for tomorrow starting from 7:00 AM.
```

**Output**

```
🗓 Task Schedule with Priority & Duration

7:00 AM - 9:00 AM | Study Machine Learning | Priority: High  
9:15 AM - 12:15 PM | Complete Assignment | Priority: High  
12:30 PM - 1:30 PM | Grocery Shopping | Priority: Medium  
2:00 PM - 2:30 PM | Call Friend | Priority: Low  
6:00 PM - 7:30 PM | Gym Workout | Priority: Medium  

⏰ Reminders Set:
• Study start reminder: 6:55 AM
• Assignment start reminder: 9:10 AM
```

---

## 3️⃣ Advanced Prompt – Context-aware task management

Now the assistant reasons, handles urgency, energy levels, dependencies.

**Prompt**

```
You are my Daily Task Assistant.  
Consider urgency, mental focus levels, and breaks. I prefer study tasks in the morning and workouts in the evening.
Organize tasks into a realistic schedule and add motivational notes.
```

**Output**
💡 Optimized Plan with Breaks + Motivation

Morning (High Focus)  
• 7:00–9:00 AM → Machine Learning study  
✨ Tip: Start with recap notes for 10 min.

Break 15 min

• 9:15–12:00 PM → Assignment writing session  
✨ Motivation: "Deep work now saves stress later!"

Afternoon  
• 1:00–2:00 PM → Grocery shopping  
• 2:30–3:00 PM → Call friend  
(Helps relax after heavy study tasks)

Evening  
• 6:00–7:30 PM → Gym workout  
💪 "Push today to grow stronger tomorrow!"
```

---

## 4️⃣ Intelligent Iterative Workflow Prompt

Allows **adding, removing, updating tasks** like an app chat.

**System Prompt Template**

```
You are a Task Planner Assistant. Maintain a list of user tasks and update it when asked.
For each request, respond with the updated task list formatted in a table:

Columns → Task | Priority | Duration | Status | Notes
```

**Example Conversation**

```
User: Add a task: prepare presentation tomorrow – priority high – 2 hours
Assistant: (updates table)

User: Mark grocery shopping as completed
Assistant: (updates table)

User: Reschedule gym to morning
Assistant: (assistant adjusts plan automatically)
```

---

## 5️⃣ Full Application-Style Prompt Framework

> This can be used to build a web/app UI later.

```
### Mode: Daily Task Manager
Store tasks internally and interact using these commands:

ADD: Add a new task  
UPDATE: Modify an existing task  
DELETE: Remove a task  
PLAN: Generate a time schedule  
SUMMARY: Show tasks with pending %, productivity score  
EXPORT: Provide tasks in JSON format for integration  

Respond always in structured format.
When PLAN is requested, analyze workload realistically.

User Input Example:
ADD: Study AI – 2 hrs – High priority – Notes: "Exam next week"
```

Example Output:

```
Task added successfully 👍

📌 Current Task List
| Task               | Priority | Duration | Status     | Notes             |
|-------------------|----------|----------|------------|------------------|
| Study AI          | High     | 2 hrs    | Pending    | Exam next week    |
| Grocery Shopping  | Medium   | 1 hr     | Pending    | Buy vegetables    |
```

---

# Optional Python Mini-App (Interactive Console Version)

```python
# task_manager.py

tasks = []

def add_task(name, priority="Medium", duration="1 hr", notes=""):
    tasks.append({"task": name, "priority": priority, "duration": duration, "status": "Pending", "notes": notes})

def show_tasks():
    print("\nCurrent Task List:")
    for i, t in enumerate(tasks, 1):
        print(f"{i}. {t['task']} | {t['priority']} | {t['duration']} | {t['status']} | {t['notes']}")

add_task("Study AI", "High", "2 hrs", "Exam next week")
add_task("Gym", "Medium", "1.5 hrs")
show_tasks()
```

---

# What You Have Now ✔

| Step                                    | Achieved |
| --------------------------------------- | -------- |
| Prompt evolution from simple → advanced | Yes      |
| Designed task prompts for ChatGPT       | Yes      |
| Outputs for each prompt style           | Yes      |
| Application-like conversation flows     | Yes      |
| Mini Python integration example         | Yes      |

---

If you want, I can extend this into:

### 🔧 Next Upgradable Versions

✔ **GUI / Streamlit Task Organizer**
✔ **Auto reminders + calendar integration**
✔ **Memory-based personal planner**
✔ **Export to PDF/Excel**
✔ **Mobile chatbot UI**

# Result: 
The corresponding Prompt is executed successfully.

