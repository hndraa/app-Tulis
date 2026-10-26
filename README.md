# TULIS — Task Management Application

**SOFTWARE** | **DESKTOP APPLICATION** | **PYTHON ‧ PYQT5**

TULIS is a desktop task management application built with Python and PyQt5. It helps users organize daily activities, manage task priorities and durations, and track schedules through an interactive interface with search, filtering, editing, and deletion features.

## 01. Project Overview

### Description

TULIS is a desktop-based to-do list application developed entirely with Python and PyQt5 without using Qt Designer. The interface is constructed programmatically and uses `QStackedWidget` to manage navigation between application pages.

The application provides a centralized workspace for creating, viewing, organizing, and managing daily tasks.

### Objectives

- Simplify the process of recording and organizing daily activities.
- Provide task management features through an interactive graphical interface.
- Help users identify important tasks using priority levels and task highlighting.
- Improve navigation through animated page transitions.

### Problem Statement

Managing daily activities can become difficult when tasks are not organized by priority, duration, or execution time. Users also need convenient ways to locate specific tasks and update or remove tasks when plans change.

### Solution

TULIS combines task creation, task listing, search, filtering, and task actions in one desktop application. Users can create tasks with descriptions, categories, priorities, durations, and execution times, then view or modify their task information through a graphical interface.

### Key Features

- **Welcome Page:** Displays the application logo, animated background icons, and a button to enter the main page.
- **Task Management:** Displays tasks as individual cards in a scrollable grid layout.
- **Create Tasks:** Add tasks with a title, description, category, duration, priority, and execution time.
- **Task Priority:** Assign a priority level from 1 to 10 and optionally mark tasks as important to place them at the top of the list.
- **Search Tasks:** Find tasks by title using a keyword search field.
- **Filter Tasks:** Filter tasks by date, priority, and execution time.
- **View Task Details:** Display detailed information about a selected task.
- **Edit Tasks:** Update task titles, descriptions, and execution times.
- **Delete Tasks:** Select tasks for deletion and confirm the action before removing them.
- **Animated Navigation:** Use `QPropertyAnimation` to animate transitions between application pages.
- **Input Validation:** Display error messages when required task information is missing.
- **Interactive Interface:** Use styled buttons, task cards, icons, and floating action buttons.

## 02. Tech Stack

| Category | Technology |
|---|---|
| Programming Language | Python |
| GUI Framework | PyQt5 |
| Main Window and Navigation | `QMainWindow`, `QStackedWidget` |
| Layout Management | `QVBoxLayout`, `QHBoxLayout`, `QGridLayout` |
| User Interface Components | `QLabel`, `QPushButton`, `QLineEdit`, `QTextEdit`, `QComboBox`, `QSlider`, `QSpinBox`, `QRadioButton`, `QCheckBox` |
| Task Display | `QFrame`, `QScrollArea` |
| Dialogs and Menus | `QDialog`, `QMessageBox`, `QInputDialog`, `QMenu`, `QToolButton` |
| Animation and Rendering | `QPropertyAnimation`, `QTimer`, `QPainter` |
| Styling | Qt Style Sheets (`setStyleSheet()`) |
| Date and Time | Python `datetime`, PyQt5 `QDate` |
| Development Environment | Python and a compatible code editor |

## 03. Screenshots / Results

The following sections document the main application workflow. Add the corresponding screenshots from the project report or capture them from the running application.

### Welcome Page

The initial screen displays the TULIS logo, a Start button, animated background icons, and the application attribution.

<img width="500" height="680" alt="image" src="https://github.com/user-attachments/assets/4bc99d35-0455-477b-ac5c-da23f8472be8" />


### Task List

The main page displays tasks in a scrollable grid of cards. Each card contains the task title, description, duration, execution time, and creation timestamp.

<img width="500" height="681" alt="image" src="https://github.com/user-attachments/assets/58612e8b-94fb-44c7-8204-3dcdcbdc2208" />


### Search Tasks

Users can enter keywords in the search field to locate tasks by title.

<img width="501" height="681" alt="image" src="https://github.com/user-attachments/assets/c4cefa2f-dc4c-4bb0-b6ac-a55cfe2539ad" />


### Filter Tasks

The filter menu provides controls for filtering tasks by date, priority, and execution time.

<img width="607" height="699" alt="image" src="https://github.com/user-attachments/assets/05a7a4c4-1d6e-47bb-b278-56d90cc084a6" />

### Delete Tasks

Delete mode highlights task cards with red dashed borders. Users can select a task and confirm whether it should be removed.

<img width="504" height="680" alt="image" src="https://github.com/user-attachments/assets/983237ec-cbf2-4b34-93b2-74a12697a8bf" />

### View Task Details

View mode highlights selectable task cards. Selecting a card opens a dialog containing the task's details.

<img width="501" height="681" alt="image" src="https://github.com/user-attachments/assets/4da812f6-470e-4667-9a86-e828ad0e836e" />

### Edit Tasks

Edit mode highlights task cards with green dashed borders and allows users to update supported task information.

<img width="502" height="682" alt="image" src="https://github.com/user-attachments/assets/ade4ffc2-d8eb-4dbe-a747-cccc51296905" />

### Add New Task

The task creation page provides input fields for task information, including title, description, category, duration, priority, importance, and execution time.

<img width="503" height="680" alt="image" src="https://github.com/user-attachments/assets/e8c4b2e5-f52c-4024-9be5-0c5a9dbbefe8" />


### Results

The application demonstrates a multi-page task management workflow with interactive controls, task organization, search and filtering, and task modification features.

## 04. Installation & Usage

### Prerequisites

- Python 3.10 or a compatible Python version.
- pip package manager.
- PyQt5 library.

### Project Structure

The following is a suggested repository structure. Keep the existing source code and asset filenames consistent with the paths used in the application.

```text
app-tulis/
├── main.py
├── logo.png
├── Bg/
│   ├── todolist.png
│   ├── alarm.png
│   ├── check.png
│   ├── clock.png
│   ├── notes.png
│   ├── palette.png
│   ├── pen.png
│   ├── pencil.png
│   └── round.png
├── Icon/
│   ├── action.png
│   ├── filter.png
│   ├── add.png
│   └── back_icon.png
└── README.md
```

### Installation

**Step 1. Clone the repository**

```bash
git clone https://github.com/hndraa/app-Tulis.git
```

**Step 2. Navigate to the project directory**

```bash
cd app-Tulis
```

**Step 3. Install PyQt5**

```bash
python -m pip install PyQt5
```

### Configuration

Ensure that the required image assets are available at the paths referenced by the source code. The application uses relative paths for the logo, background icons, and interface icons.

Run the application from the project root directory so these paths can resolve correctly.

### Run the Application

Execute the main Python file:

```bash
python main.py
```

### Usage Instructions

1. Launch the application to open the Welcome Page.
2. Click **Mulai** to open the task list.
3. Use the search field to find tasks by title.
4. Open the filter menu to select date, priority, or execution-time criteria.
5. Use the action menu to select Delete, View, or Edit mode.
6. Select a task card to perform the chosen action.
7. Use the floating action button to open the new-task form.
8. Enter the required task information and save the task.
9. Mark important tasks when needed to place them at the top of the task list.
10. Use the back button to exit selection modes or return to the previous page.
