Based on the repository content, here is a complete README for your Init-Mini-Project.

---

# Managing Scheduled Tasks

A PowerShell script designed to automate the management of scheduled tasks on Windows systems. This project serves as an introductory exercise for students to learn about scripting, task scheduling, and PowerShell functionalities.

## Features

- **Create Scheduled Task**: Easily create new scheduled tasks with various trigger options (At Logon, Daily, Weekly, One Time).
- **View Scheduled Tasks**: Display a list of existing scheduled tasks with details such as Task Name, State, Next Run Time, and Last Run Time.
- **Modify Scheduled Task**: Update an existing task's program path or trigger settings.
- **Delete Scheduled Task**: Remove a scheduled task from the system.
- **Check Task Status**: Monitor the current status of a specific scheduled task.
- **Export Task List**: Save the list of scheduled tasks to a CSV file for reporting or auditing purposes.

## Project Structure

```
Init-Mini-Project/
├── Init Project File.ps1    # Main PowerShell script for task automation
└── README.md                # Project documentation
```

## Prerequisites

- Windows operating system
- PowerShell (version 5.1 or higher recommended)

## Getting Started

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/Ariashakoo/Init-Mini-Project.git
   cd Init-Mini-Project
   ```

2. Open PowerShell as an administrator (right-click PowerShell and select "Run as administrator").

3. Run the script:
   ```powershell
   .\Init Project File.ps1
   ```

4. Follow the interactive menu to manage your scheduled tasks.

## Usage

The script presents an interactive menu with the following options:

```
== Scheduled Tasks Automation ==
1. Create Scheduled Task
2. View Scheduled Tasks
3. Modify Scheduled Task
4. Delete Scheduled Task
5. Check Task Status
6. Export Task List
7. Exit
```

### 1. Create Scheduled Task
- Enter a task name
- Enter the full path of the program or script to run
- Select a trigger type: At Logon, Daily, Weekly, or One Time
- Provide additional details based on the trigger type (e.g., start time, days of week, run date)

### 2. View Scheduled Tasks
Displays a formatted table of all existing scheduled tasks with their current state and run times.

### 3. Modify Scheduled Task
- Enter the name of the task to modify
- Update the program path or trigger settings

### 4. Delete Scheduled Task
- Enter the name of the task to delete

### 5. Check Task Status
- Enter the name of the task to check
- Displays the current state (Running, Ready, Disabled, etc.)

### 6. Export Task List
- Enter an output file path (e.g., `C:\ScheduledTasks.csv`)
- Saves the task list as a CSV file

## Script Functions Overview

| Function | Description |
|----------|-------------|
| `Create-ScheduledTask` | Creates a new scheduled task with user-specified triggers and settings |
| `Show-ScheduledTasks` | Displays all existing scheduled tasks in a table format |
| `Modify-ScheduledTask` | Updates an existing task's program path or trigger settings |
| `Remove-ScheduledTask` | Deletes a specified scheduled task |
| `Check-TaskStatus` | Checks and displays the status of a specified task |
| `Export-TaskList` | Exports the task list to a CSV file |
| `Main` | Displays the interactive menu and handles user input |

## Known Limitations / TODOs

The script is designed as an introductory project and contains several incomplete sections that can be extended:

- **Weekly trigger**: The weekly trigger implementation needs to be completed
- **One Time trigger**: The one-time trigger implementation needs to be completed
- **Task registration**: The task registration logic needs to be implemented
- **Action update**: The action update logic for task modification needs to be implemented
- **Trigger modification**: The trigger modification logic needs to be implemented
- **Task deletion**: The task deletion logic needs to be implemented
- **CSV export**: The CSV export functionality needs to be implemented

## Possible Improvements

- **Error handling**: Add comprehensive error handling for all operations
- **Logging**: Implement logging to track all actions performed
- **Scheduled task credentials**: Add support for running tasks with specific user credentials
- **Multiple actions**: Support tasks with multiple actions (e.g., running multiple programs)
- **GUI interface**: Build a graphical user interface for easier task management
- **Scheduled task history**: Display historical run data for each task

## Technologies Used

- **PowerShell** — Windows scripting and automation language

## License

This project is open source and available under the [MIT License](LICENSE).

## Contact

For any questions or suggestions, please open an issue on GitHub or reach out to the repository owner.

---

## Suggested Topics for Your Repository

Remember to add these topics to your repository by clicking the gear icon in the "About" section on the main page:

