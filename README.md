# Python & Jupyter Notebook Setup Guide

## Table of Contents
- [Running Existing Python Notebooks](#running-existing-python-notebooks)
  - [Option 1: Local Setup (VS Code)](#option-1-local-setup-vs-code)
  - [Option 2: Google Colab](#option-2-google-colab)
- [Initial Setup Requirements](#initial-setup-requirements)
- [Common Issues & Troubleshooting](#common-issues--troubleshooting)

## Running Existing Python Notebooks

We'll be working with notebooks from: https://github.com/impradp/EverythingWithPython

### Option 1: Local Setup (VS Code)

1. **Install Required Software**:
   - Python (from [python.org](https://python.org))
   - Git (from [git-scm.com](https://git-scm.com))
   - VS Code (from [code.visualstudio.com](https://code.visualstudio.com))

2. **Clone the Repository**:
   ```bash
   # Open terminal/command prompt and run:
   git clone https://github.com/impradp/EverythingWithPython
   cd EverythingWithPython
   ```

3. **Set Up Python Environment**:
   ```bash
   # Create virtual environment
   python -m venv venv

   # Activate virtual environment
   # For Windows:
   venv\Scripts\activate
   # For Mac/Linux:
   source venv/bin/activate

   # Install required packages
   pip install jupyter notebook ipykernel numpy pandas matplotlib seaborn scikit-learn
   ```

4. **Open in VS Code**:
   ```bash
   code .
   ```
   - Install Python and Jupyter extensions if prompted
   - Select your Python interpreter (from the venv)
   - Open any .ipynb file to start working

### Option 2: Google Colab

1. **Access Google Colab**:
   - Visit [colab.research.google.com](https://colab.research.google.com)
   - Sign in with your Google account

2. **Open Repository Notebooks**:
   - Click `File → Open Notebook`
   - Select the `GitHub` tab
   - Paste: `https://github.com/impradp/EverythingWithPython`
   - Choose the notebook you want to work with

3. **Clone Entire Repository in Colab** (if needed):
   ```python
   !git clone https://github.com/impradp/EverythingWithPython
   ```

### Why Choose Google Colab?
- No local setup required
- Pre-installed Python packages
- Free GPU access
- Easy sharing and collaboration
- Automatic saves to Google Drive

## Initial Setup Requirements

### For Local Setup:
1. **System Requirements**:
   - Windows 10/11, macOS, or Linux
   - At least 4GB RAM (8GB recommended)
   - 5GB free disk space

2. **VS Code Extensions**:
   - Python (by Microsoft)
   - Jupyter (by Microsoft)

### For Google Colab:
1. **Requirements**:
   - Modern web browser (Chrome recommended)
   - Google account
   - Stable internet connection

## Common Issues & Troubleshooting

### Local Setup Issues:

1. **Git Clone Failed**:
   ```bash
   # Alternative download method:
   # Download ZIP from GitHub website and extract
   ```

2. **Package Installation Errors**:
   ```bash
   # Update pip first
   pip install --upgrade pip
   
   # If still having issues:
   pip install --force-reinstall ipykernel
   ```

3. **Kernel Issues**:
   - Select Python kernel from venv
   - Restart kernel if notebooks freeze
   - Clear outputs and restart if memory issues occur

### Google Colab Issues:

1. **Runtime Disconnections**:
   - Keep browser tab active
   - Save work frequently
   - Reconnect to runtime if disconnected

2. **Resource Limits**:
   - Use `Runtime → Factory reset runtime` if running slow
   - Clear output cells to free memory
   - Disconnect when not in use

## Getting Help

- Repository Issues: Check the [GitHub Issues](https://github.com/impradp/EverythingWithPython/issues) page
- VS Code Help: [code.visualstudio.com/docs](https://code.visualstudio.com/docs)
- Colab FAQ: [research.google.com/colaboratory/faq.html](https://research.google.com/colaboratory/faq.html)
- Python Help: [python.org/doc](https://python.org/doc)

## Next Steps

After setup, start with the introductory notebooks in the repository. These will help you understand the basic concepts before moving to more advanced topics.

Remember to:
- Read the notebook descriptions before running
- Execute cells in order
- Save your work regularly
- Create copies of notebooks before experimenting

---

**Note**: If you encounter any specific issues not covered here, please raise an issue on the GitHub repository or consult with your instructor.