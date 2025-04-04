# Project Structure

```console
bessel_project/
│── WORKSPACE
│── BUILD
│── requirements.txt
│
├── bessel_module/
│   ├── BUILD
│   ├── bessel.py
│
├── math_operations/
│   ├── BUILD
│   ├── math_ops.py
│
└── main/
    ├── BUILD
    ├── main.py

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

