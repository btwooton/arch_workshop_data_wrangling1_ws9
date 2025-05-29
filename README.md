# ARCH Workshop: Healthcare Data Wrangling in Python & Jupyter - I [WS9]

## 3 Options to Follow Along with the Hands On Module(s)

### *Option 1.* Links to Notebooks in Google Colab *(preferred)*:

1. [WS9 Hands On Module](https://colab.research.google.com/github/expmed/arch_workshop_data_wrangling1_ws9/blob/main/ws9_hands_on.ipynb)

### *Option 2.* Alternative Links to Run the Notebook(s) in Binder *(backup for attendees who do not have Google accounts)*:
**Note: mybinder.org offers significantly resource constrained environments to run interactive jupyter notebooks 
so you might run into memory issues while running some or all of the modules, depending on the size of the loaded data.
This service is also known to be unavailable from time to time at inconsistent and upredictable frequencies. Use at your own discretion.**
1. [WS9 Hands On Module](https://mybinder.org/v2/gh/expmed/arch_workshop_data_wrangling1_ws9/main?filepath=ws9_hands_on.ipynb)

### *Option 3.* Minimal Local Environment Instructions *(for Workshop Attendees who Want to Run Locally)* 

These instructions will help you set up Python, Jupyter, and the necessary packages for the hands-on exercises in this workshop.  

---

### **Step 1: Install Python**  
✅ **Check if Python is already installed**  
Open a terminal (Command Prompt on Windows, Terminal on macOS/Linux) and run:  
```sh
python --version
```
or  
```sh
python3 --version
```  
If Python is installed, you’ll see an output like `Python 3.x.x`. If not, follow the next step.  

✅ **Install Python (if not already installed)**  
- **Windows:** Download and install Python from [https://www.python.org/downloads/](https://www.python.org/downloads/). Make sure to check the box **"Add Python to PATH"** during installation.  
- **Mac:** Run the following command in Terminal:  
  ```sh
  brew install python3
  ```  
  *(Requires Homebrew. If not installed, visit [https://brew.sh/](https://brew.sh/))*  
- **Linux (Debian/Ubuntu):**  
  ```sh
  sudo apt update && sudo apt install python3 python3-venv python3-pip
  ```  

---

### **Step 2: Install Jupyter and Required Packages**  
📌 **Create a Virtual Environment** (Recommended)  
1. Open a terminal or command prompt and navigate to a directory where you want to store the workshop materials.  
2. Run the following commands:  
   ```sh
   python -m venv workshop_env  # Create a virtual environment
   source workshop_env/bin/activate  # Activate it (Mac/Linux)
   workshop_env\Scripts\activate     # Activate it (Windows)
   ```  

📌 **Install Required Packages**  
1. Download the ZIP file of the workshop repository from the provided link and extract it.  
2. In the terminal, navigate to the extracted folder using `cd <folder_name>`.  
3. Run:  
   ```sh
   pip install -r requirements.txt
   ```  

---

### **Step 3: Start Jupyter Notebook**  
Once installation is complete, launch Jupyter Notebook with:  
```sh
jupyter notebook
```  
This will open a web-based interface where you can run the hands-on exercises.  

---

### **Alternative: One-Step Installation (Without Virtual Environment)**  
If you prefer a simpler setup, you can install everything globally (not recommended):  
```sh
pip install jupyter pandas numpy matplotlib seaborn
```  
Then launch Jupyter Notebook with:  
```sh
jupyter notebook
```  

---

### **Troubleshooting**  
❓ *Command not found errors?* Try using `python3` instead of `python` or `pip3` instead of `pip`.  
❓ *Permission errors?* Use `pip install --user` or run with `sudo` (Linux/macOS).  
❓ *Windows users: If `jupyter notebook` doesn’t work, try running `python -m jupyter notebook`.  
