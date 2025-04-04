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

```console

               +----------------------+
               |      main.py          |
               | (Entry point)         |
               +----------------------+
                          |
       --------------------------------------
       |                                    |
+-------------------+                 +------------------+
|  bessel.py       |                 |  math_ops.py     |
|  (Bessel Calc)   |                 |  (Math Utils)    |
+-------------------+                 +------------------+
       |                                    |
       |                                    |
+-------------------+                 +------------------+
|  SciPy           |                 | NumPy           |
|  NumPy           |                 |                |
|  Matplotlib      |                 |                |
+-------------------+                 +------------------+

```

