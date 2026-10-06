# Web Development Assignment  
## Personal Study Planner Web Application

### Module
Introduction to Web Development with Python

### Assignment Title
**Design and Development of a Personal Study Planner**

### Scenario

University students often need to keep track of assignments, revision tasks, deadlines, and other academic responsibilities.

Your task is to design and develop a simple **web-based Study Planner** that allows a student to create and manage their study tasks.

The application should be developed primarily using **Python**. You are recommended to use the **Flask** web framework together with HTML and CSS.

---

## Task

Develop a web application where a user can manage their university study tasks.

Each task should contain:

- Task name
- Module or subject
- Due date
- Priority
- Status

For example:

**Task:** Finish Programming Assignment  
**Module:** Computer Science  
**Due Date:** 15 October 2026  
**Priority:** High  
**Status:** In Progress

---

# Minimum Requirements

Your application must allow the user to:

### 1. View Tasks

The homepage should display all existing study tasks.

Each task should clearly show:

- Task name
- Module
- Due date
- Priority
- Status

---

### 2. Add a Task

The user should be able to complete a form containing:

- Task name
- Module
- Due date
- Priority
- Status

The task should then appear in the task list.

---

### 3. Edit a Task

The user should be able to edit an existing task.

For example, they may want to change:

- The deadline
- The priority
- The task name
- The status

---

### 4. Delete a Task

The user should be able to permanently remove a task.

---

### 5. Mark a Task as Completed

The user should be able to change the status of a task to:

- Not Started
- In Progress
- Completed

Completed tasks should be visually distinguishable from unfinished tasks.

---

# Technical Requirements

The project should use:

- **Python 3**
- **Flask**
- **HTML**
- **CSS**
- **SQLite**

A suggested project structure is:

```text
study-planner/
│
├── app.py
├── study_planner.db
│
├── templates/
│   ├── index.html
│   ├── add_task.html
│   └── edit_task.html
│
└── static/
    └── style.css
```

---

# Database

Create a database table called `tasks`.

A possible structure is:

```text
tasks
--------------------------------
id
title
module
due_date
priority
status
```

Example data:

```text
1 | Finish Python Assignment | Programming | 15/10/2026 | High | In Progress

2 | Revise Chapter 4 | Mathematics | 20/10/2026 | Medium | Not Started

3 | Prepare Presentation | Communication | 25/10/2026 | Low | Completed
```

---

# Suggested Pages

### Homepage – `/`

Displays the list of study tasks.

Example:

```text
--------------------------------------
        MY STUDY PLANNER
--------------------------------------

[ Add New Task ]

Python Assignment
Programming
Due: 15 October
Priority: HIGH
Status: In Progress

[Edit] [Complete] [Delete]

--------------------------------------

Math Revision
Mathematics
Due: 20 October
Priority: MEDIUM
Status: Not Started

[Edit] [Complete] [Delete]
```

### Add Task – `/add`

Contains a form allowing the user to create a new task.

### Edit Task – `/edit/<id>`

Allows the user to update an existing task.

### Delete Task – `/delete/<id>`

Deletes the selected task.

---

# Extension Features

Once the minimum application is working, you may attempt additional features.

Possible extensions include:

- Search for tasks
- Filter tasks by module
- Filter tasks by priority
- Filter completed and unfinished tasks
- Sort tasks by due date
- Show overdue tasks
- Add a dark mode
- Add task descriptions
- Display the percentage of tasks completed

For example:

```text
Study Progress

████████████░░░░░░░░

6 / 10 Tasks Completed
60%
```

---

# Advanced Challenge

For students wanting an additional challenge, implement a simple user account system.

Users should be able to:

- Register
- Log in
- Log out
- View only their own tasks

This could be implemented using Flask sessions and password hashing.

---

# Learning Outcomes

By completing this assignment, you should demonstrate an understanding of:

1. Creating a web server using Python and Flask.
2. Creating routes and handling HTTP requests.
3. Using HTML templates with Flask.
4. Processing HTML forms.
5. Connecting a Python application to an SQLite database.
6. Performing CRUD operations:
   - Create
   - Read
   - Update
   - Delete
7. Structuring a small web development project.
8. Applying basic HTML and CSS styling.

---

# Submission Requirements

Submit:

1. The complete source code.
2. The SQLite database.
3. A short `README.md` explaining:
   - How to install the application.
   - How to run the application.
   - What features were implemented.
4. Screenshots showing:
   - Homepage
   - Adding a task
   - Editing a task
   - Completed tasks

---

# Recommended Development Stages

**Stage 1:** Create a basic Flask application.

**Stage 2:** Create the HTML homepage.

**Stage 3:** Create the SQLite database.

**Stage 4:** Display database tasks on the homepage.

**Stage 5:** Implement adding tasks.

**Stage 6:** Implement editing tasks.

**Stage 7:** Implement deleting tasks.

**Stage 8:** Implement task completion.

**Stage 9:** Add CSS and improve the interface.

**Stage 10:** Attempt optional extension features.

---

# Assessment Criteria

| Area | Weight |
|---|---:|
| Python / Flask functionality | 30% |
| Database implementation | 20% |
| CRUD functionality | 20% |
| HTML / CSS interface | 15% |
| Code structure and readability | 10% |
| Additional features | 5% |

**Total: 100%**
