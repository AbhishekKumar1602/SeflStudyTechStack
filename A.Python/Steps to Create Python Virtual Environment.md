# Steps to Create Python Virtual Environment

### 1. Install Python 3

```
sudo apt-get install python3
```

### 2. Install Python Package Manager - PIP 3

```
sudo apt-get install python3-pip
```

### 3. Install Python Venv Module

```
sudo apt-get install python3.10-venv
```

### 4. Create Python Virtual Environment
- Navigate to the desired directory and run:

```
python3 -m venv ./MyVenv
```

- `python3`: Invokes the Python 3 interpreter.
- `-m venv`: Uses the venv module to create a virtual environment.
- `./MyVenv`: Specifies the path where the virtual environment will be created.

### 5. Activate the Virtual Environment:

```
source ./MyVenv/bin/activate
```

### 6. Install Required Packages:
- While the virtual environment is active, install any required packages using pip:

```
pip install package_name
```

### 7. Deactivate the Virtual Environment:
- When done working in the virtual environment, deactivate it:

```
deactivate
```

**Note:** For future package installations, remember to activate the environment first, install packages, and then deactivate it. This approach keeps your project dependencies isolated and ensures a clean development environment.