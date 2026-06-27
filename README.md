# CyberSecurityBotAwareness - Part 3

**Student:** Nomhle Yolanda Makhanya  
**Student Number:** ST10470578  
**Module:** PROG6221 - Programming 2B  
**Institution:** Rosebank International
---

## Project Overview

CyberSecurityBotAwareness is a WPF-based Cybersecurity Awareness Chatbot built in C#. 
This is Part 3 of the POE, which enhances the existing chatbot from Parts 1 and 2 with 
advanced features including a Task Manager, Cybersecurity Quiz, NLP Simulation, and Activity Log.

---

## Features

### Part 1 & 2 (Existing Features)
- Keyword-based cybersecurity responses (passwords, phishing, malware, VPNs, etc.)
- Sentiment detection (worried, curious, frustrated)
- Conversation memory (remembers username and favourite topic)
- Random varied responses using Lists and Dictionaries
- Dark pink and navy themed GUI

### Part 3 (New Features)

####  Task 1 - Task Assistant with Database Integration
- Add cybersecurity-related tasks with a title and description
- Set optional reminder dates for tasks
- View all tasks in a list
- Mark tasks as completed
- Delete tasks
- All tasks stored and retrieved from a SQL Server LocalDB database

####  Task 2 - Cybersecurity Mini-Game (Quiz)
- 12 questions covering key cybersecurity topics
- Mix of multiple choice and true/false questions
- One question displayed at a time
- Immediate feedback after each answer
- Correct answer highlighted in green, wrong in red
- Final score with performance message
- Play Again option

####  Task 3 - NLP Simulation
- Keyword intent detection using string.Contains()
- Recognises varied phrasings such as:
  - "remind me", "set a reminder", "don't let me forget" → opens Task Manager
  - "quiz", "test me", "challenge me" → opens Quiz
  - "show activity log", "what have you done" → shows Activity Log
  - "add task", "create task", "new task" → opens Task Manager
- Responds naturally to user input even if worded differently

####  Task 4 - Activity Log
- Records all key actions with timestamps
- Tracks tasks added, completed, deleted
- Tracks quiz started and completed with score
- Tracks NLP interactions
- View last 10 actions via chat command or button
- Accessible by typing "show activity log" or "what have you done for me?"

---

## Technologies Used

- **Language:** C#
- **Framework:** WPF (Windows Presentation Foundation)
- **Database:** SQL Server LocalDB
- **IDE:** Visual Studio 2026
- **Version Control:** GitHub

---
## Video Presentation
https://youtu.be/zLgpglnVB1U 

## How to Run

1. Clone the repository
2. Open `CyberSecurityBotAwareness.sln` in Visual Studio
3. Ensure SQL Server LocalDB is installed
4. Build the solution (Ctrl + Shift + B)
5. Press F5 to run

---

## Database Setup

The database and table are created automatically when the app runs for the first time.
Connection string used:

Server=(localdb)\MSSQLLocalDB;Database=cybersecurity_bot;Trusted_Connection=True;
