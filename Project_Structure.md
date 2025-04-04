# Project Structure

```console
task_manager/
│── user/
│   ├── __init__.py
│   ├── user.py
│   ├── auth.py
│   └── BUILD
│
│── task/
│   ├── __init__.py
│   ├── task.py
│   └── BUILD
│
│── notification/
│   ├── __init__.py
│   ├── email.py
│   └── BUILD
│
│── app.py
│── BUILD
│── WORKSPACE
│
└── tests/
    ├── test_user.py
    ├── test_task.py
    ├── test_notification.py
    └── BUILD


```

# Dependency Graph

![image](https://github.com/user-attachments/assets/7196a9df-8163-4b8d-8549-910679ae7f62)


# Sequence Diagram

```console

 User           App              Task                  Notification
  |              |                |                        |
  | Login       ->                |                        | 
  |              |                |                        |
  |            Call Task         ->                        |
  |            Create Task        |                        |
  |              |                |                        |
  |              |       Send Notification ->              |
  |              |                |                  Email Sent

```
