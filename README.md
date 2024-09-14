# Task-Management-System-with-Cpp

This project is a simple Task Management System implemented in C++. It allows users to manage tasks through a command-line interface (CLI). The system provides functionalities for task creation, deletion, status updates, categorization, priority settings, and more. Tasks are stored in a JSON file for persistence, allowing the system to retain tasks even after restarting the program.

Features
Task Creation: Users can add new tasks with a name, category (e.g., Work, Personal), priority (Low, Medium, High), and a due date.
Task Deletion: Users can delete tasks by specifying the task name.
Task Status: Tasks can be marked as Pending, Completed, or Overdue.
Task Categories: Tasks can be organized under different categories like Work, Personal, etc.
Priorities: Tasks can be assigned priority levels (Low, Medium, High).
Due Dates: Users can set deadlines for each task.
Task Storage: Tasks are saved in a JSON file (tasks.json), so they persist between program runs.
Task Sorting: Users can sort tasks by priority or deadline.
Search Functionality: Users can search for tasks by keywords in the task name or category.
Command-Line Interface (CLI): The entire system runs in the command-line interface.
Prerequisites
To compile and run the project, you'll need:

A C++ compiler that supports C++11 or later.
The nlohmann/json library for JSON handling. You can add this as a header file (json.hpp).
Installation
Clone the repository or download the task_manager.cpp file to your local machine.
Download the JSON library from nlohmann/json and place the json.hpp file in your project directory.
Compile the program with your preferred C++ compiler.
Example using g++:
bash
Kodu kopyala
g++ -std=c++11 task_manager.cpp -o task_manager
Run the compiled program:
bash
Kodu kopyala
./task_manager
Usage
Once you run the program, you'll be presented with a menu of options:

mathematica
Kodu kopyala
Task Management System Menu:
1. Add Task
2. Delete Task
3. Update Task Status
4. List All Tasks
5. Search Task
6. Sort Tasks by Deadline
7. Sort Tasks by Priority
8. Exit
Add Task
Input the task details when prompted: task name, category, priority, and due date (YYYY-MM-DD format).
Delete Task
Specify the task name to delete it.
Update Task Status
Specify the task name and choose the new status: Pending, Completed, or Overdue.
List All Tasks
Lists all current tasks along with their details.
Search Task
Search for tasks by entering a keyword (this will search in both the task name and category).
Sort Tasks
Choose to sort tasks by deadline or by priority.
Exit
Exits the program.
File Handling
All tasks are saved to a file called tasks.json. This file is automatically created and updated each time a task is added, deleted, or modified.
When the program starts, it will load tasks from the tasks.json file.
Example Task JSON Structure
Here’s an example of how tasks are saved in tasks.json:

json
Kodu kopyala
[
    {
        "name": "Finish report",
        "category": "Work",
        "priority": "High",
        "dueDate": "2024-09-15",
        "status": "Pending"
    },
    {
        "name": "Grocery shopping",
        "category": "Personal",
        "priority": "Medium",
        "dueDate": "2024-09-17",
        "status": "Pending"
    }
]
Future Enhancements
Possible future improvements to the system:

Add notifications or reminders for overdue tasks.
Support for recurring tasks.
Implementing a GUI (Graphical User Interface).
Support for filtering tasks based on different criteria (category, priority, status).
License

Thanks for checking out my repository.

