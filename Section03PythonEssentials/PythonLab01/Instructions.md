
# Project Setup Guide

This series will use **Python 3.12**. Follow the steps below to set up your environment, manage dependencies, and run your code efficiently.

> **Tip:** It's recommended to create a separate virtual environment for each project to avoid package conflicts and ensure compatibility.

### Prerequisites
Ensure you have [Anaconda](https://www.anaconda.com/products/distribution) installed for creating virtual environments and managing dependencies easily.

---

### Steps to Set Up a Project

1. **Create a Project Environment**  
   Navigate to your working directory and create a new virtual environment for your project:
   
   ```bash
   conda create -p venv python=3.12
   ```
   This will install Python 3.12 and a few basic packages. The setup time may vary depending on your internet speed.

2. **Activate the Environment**  
   Ensure you're in the project directory, then activate the environment:
   
   ```bash
   conda activate venv
   ```

3. **Verify Environment Activation**  
   After activating the environment, create a file named `app.py` and add a simple print command:

   ```python
   # app.py
   print("Environment setup successful")
   ```

   Run this in the terminal or IDE to check if the environment is correctly set up:
   
   ```bash
   python app.py
   ```

4. **Set Up Jupyter Notebook (Optional)**  
   Create a folder for your notebooks if needed and add a Jupyter Notebook file:

   - Create a new folder for notebooks, and inside it, create `test.ipynb`.
   - Open `test.ipynb` in Visual Studio Code. You should see "Detecting Kernels" at the top.
   - Select the environment you created earlier (usually named `venv`) to connect it.

   Add a simple test cell:

   ```python
   1 + 1
   ```

   If prompted to install `ipykernel` to run the code, install it by running:

   ```bash
   pip install ipykernel
   ```

   > **Note:** `ipykernel` enables Jupyter notebooks to run code.

5. **Managing Dependencies with `requirements.txt`**  
   An alternative way to install packages is by creating a `requirements.txt` file. List your packages in this file, and install them as follows:

   ```bash
   pip install -r requirements.txt
   ```

---

### Additional Tips
- **Organize Your Code**: Keep each project in its own folder to avoid mixing files from different projects.
- **Environment Naming**: If using multiple projects, give each environment a unique name for easy identification.
- **Troubleshooting**: Ensure that your virtual environment is active whenever you're working on the project to avoid issues with dependencies.

