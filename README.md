# AI Executive & Task Management Agent

An AI-powered business assistant for employee lookup, task monitoring, and task status management, built with **n8n** and **Groq API (GPT OSS 20B)**.

The project demonstrates how a conversational AI agent can interact with structured company data through dedicated n8n workflows.

## Key Features

- **Task Search & Monitoring** — Search company tasks and retrieve information by employee, status, priority, and due date.
- **Employee Lookup** — Find employees by ID or name and retrieve employee details.
- **Task Status Updates** — Update existing task statuses, including reopening completed tasks.
- **Overdue Task Detection** — Identify overdue tasks by comparing deadlines with a specified date.
- **Error Handling** — Return a clear response when a requested task does not exist.
- **Multilingual Interaction** — Process business requests in different languages.

## Technology Stack

- n8n — Workflow automation
- Groq API — AI model integration
- GPT OSS 20B — Language model
- n8n Data Tables — Structured task and employee storage
- JSON — Workflow configuration and data exchange

## Project Architecture

The AI agent connects to three dedicated workflow tools:

| Workflow | Purpose |
|---|---|
| [Search Company Tasks](workflows/search-company-tasks.json) | Retrieve and filter company tasks |
| [Find Company Employees](workflows/find-company-employees.json) | Search employee records |
| [Update Task Status](workflows/update-task-status.json) | Modify existing task statuses |

The main AI agent configuration is available here:

**[AI Executive & Task Management Agent](workflows/ai-executive-task-management-agent.json)**

## Example Use Cases

- Find all active employees and display their details.
- Search for tasks assigned to a specific employee.
- Check whether a task is overdue.
- Change a task status from *To Do* to *In Progress* or *Completed*.
- Reopen a previously completed task.
- Handle requests involving nonexistent task IDs.

## Screenshots

Project workflow diagrams and example AI agent interactions are available in the [screenshots folder](screenshots/).

## Project Structure

```text
ai-executive-task-management-agent/
├── workflows/
│   ├── ai-executive-task-management-agent.json
│   ├── find-company-employees.json
│   ├── search-company-tasks.json
│   └── update-task-status.json
├── screenshots/
└── README.md
```

## Project Scope

This project focuses on **AI-assisted task monitoring, employee information retrieval, and task status updates**.

It demonstrates modular workflow design, AI-to-workflow integration, structured data processing, and practical business process automation.

---

**Portfolio Project | n8n Automation | AI Business Assistant**
