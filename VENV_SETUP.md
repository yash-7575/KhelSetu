# Virtual Environment Setup

This project uses a Python virtual environment to manage dependencies and ensure reproducible builds.

## Quick Start

### Option 1: Using the activation script (Windows)
```bash
# Double-click on activate_venv.bat or run:
activate_venv.bat
```

### Option 2: Manual activation
```bash
# Activate the virtual environment
venv\Scripts\activate

# Deactivate when done
deactivate
```

## Installing Dependencies

All required packages are already installed in the virtual environment. If you need to install additional packages:

```bash
# Activate the virtual environment first
venv\Scripts\activate

# Install new packages
pip install package_name

# Update requirements.txt
pip freeze > requirements.txt
```

## Recreating the Environment

If you need to recreate the virtual environment on a different machine:

```bash
# Create new virtual environment
python -m venv venv

# Activate it
venv\Scripts\activate

# Install all dependencies
pip install -r requirements.txt
```

## Running Jupyter Notebook

```bash
# Activate the virtual environment
venv\Scripts\activate

# Start Jupyter Notebook
jupyter notebook

# Or start Jupyter Lab
jupyter lab
```

## Project Dependencies

Key packages installed:
- **Python**: 3.11.9
- **OpenCV**: 4.11.0.86
- **MediaPipe**: 0.10.21
- **NumPy**: 1.26.4
- **Matplotlib**: 3.10.6
- **Jupyter**: 1.1.1

All dependencies with exact versions are listed in `requirements.txt`.

## Troubleshooting

If you encounter kernel issues:
1. Make sure the virtual environment is activated
2. The kernel should be registered as "Python (venv)" in Jupyter
3. If not, run: `python -m ipykernel install --user --name=venv --display-name="Python (venv)"`

