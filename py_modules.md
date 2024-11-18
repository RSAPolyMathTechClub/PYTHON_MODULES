
# Python Modules for Computer Science, IT, AI, and Data Science

## List installed

- To list the installed Python modules, you can use the following commands:

1. Using pip:
  
```bash
  pip list
```

- This will display a list of all installed Python modules and their versions.
  
1. Using pip freeze:

```bash
  pip freeze
```

- This will also list the installed modules but in a format that's typically used for creating requirements.txt files (e.g., module==version).
  
1. Using python -m pip:

```bash
  python -m pip list
```

This is equivalent to pip list and is sometimes preferred for clarity or when dealing with multiple Python versions.
4. Using conda (if using Anaconda):

```bash
    conda list
```

- This command lists all the packages installed in the current Conda environment, including non-Python packages.

5. Using pkg_resources in Python:

```python

    import pkg_resources
    installed_packages = pkg_resources.working_set
    for package in installed_packages:
        print(package.key, package.version)

```

- This will print a list of installed modules and their versions in your Python environment.

## How to install from a list in a file

1. Create a requirements file

- The file should contain one module per line. For example, you could have a file named requirements.txt that looks like this:

```txt
numpy
pandas
scikit-learn

```

- With versions
  
```txt

numpy==1.21.0
pandas==1.3.0
scikit-learn==0.24.2

```

1. Install from the file using pip

- To install the modules listed in the file, use the following command:

pip install -r requirements.txt

This command will read the requirements.txt file, and install all the modules listed there.
3. If you have a custom file

- If your list is stored in a file with a different name (e.g., my_modules.txt), replace requirements.txt with the path to your file:

```bash
pip install -r my_modules.txt
```

4. Creating a requirements.txt file

- If you want to generate a requirements.txt file for your current environment to share with others, you can run:

```bash
pip freeze > requirements.txt
```

- This will create a requirements.txt file with all the installed packages and their exact versions, which can be shared and used to recreate the environment.

## 0. Core Python Utilities

- Notes

## 1. Core Python Science Utilities

- **Modules:**
  
  - `numpy`: Numerical computations
  - `pandas`: Data manipulation and analysis
  - `scipy`: Scientific computing
  - `matplotlib`: Data visualization
  - `seaborn`: Statistical data visualization

- **Install Command:**

```bash

pip install numpy
pip install pandas
pip install scipy
pip install matplotlib
pip install seaborn
   
```

---

## 2. Artificial Intelligence and Machine Learning

- **Modules:**
  
  - `scikit-learn`: Machine learning algorithms
  - `tensorflow`: Deep learning framework
  - `keras`: High-level deep learning API
  - `pytorch`: Deep learning and AI research framework
  - `xgboost`: Gradient boosting algorithm
  - `lightgbm`: Light Gradient Boosting Machine
  - `catboost`: Gradient boosting by Yandex
  - `transformers`: Natural Language Processing (NLP) with transformers

- **Install Command:**
  
```bash

pip install scikit-learn
pip install tensorflow
pip install keras
pip install torch
pip install xgboost
pip install lightgbm
pip install catboost
pip install transformers

```

## 3. Data Science and Data Engineering

- **Modules:**
  
  - `dask`: Parallel computing
  - `pyarrow`: Columnar data processing
  - `pyspark`: Big data processing
  - `vaex`: Out-of-core DataFrames
  - `SQLAlchemy`: Database interaction
  - `pyodbc`: ODBC database connectivity

- **Install Command:**

```bash

pip install dask
pip install pyarrow
pip install pyspark
pip install vaex
pip install SQLAlchemy
pip install pyodbc

```

---

## 4. Natural Language Processing (NLP)

- **Modules:**
  
  - `nltk`: NLP tools
  - `spacy`: NLP pipeline
  - `gensim`: Topic modeling and vector space modeling
  - `textblob`: Simplified text processing
  - `wordcloud`: Generate word clouds

- **Install Command:**

```bash

pip install nltk
pip install spacy
pip install gensim
pip install textblob
pip install wordcloud

```

---

## 5. Computer Vision

- **Modules:**

  - `opencv-python`: Image and video processing
  - `imageio`: Reading and writing images
  - `Pillow`: Image manipulation
  - `torchvision`: Datasets and models for vision
  - `albumentations`: Image augmentation
  - `pyzbar`: Barcode and QR code detection

- **Install Command:**

```bash

pip install opencv-python
pip install imageio
pip install Pillow
pip install torchvision
pip install albumentations
pip install pyzbar

```

---

## 6. Scientific and Statistical Computing

- **Modules:**
  
  - `statsmodels`: Statistical modeling and testing
  - `sympy`: Symbolic mathematics
  - `networkx`: Graph and network analysis
  - `igraph`: Network analysis
  - `rpy2`: Integration with R

- **Install Command:**

```bash

pip install statsmodels
pip install sympy
pip install networkx
pip install igraph
pip install rpy2

```

---

## 7. Web Development and APIs

- **Modules:**
  
  - `flask`: Lightweight web framework
  - `django`: Full-stack web framework
  - `fastapi`: Modern web APIs
  - `requests`: HTTP requests
  - `beautifulsoup4`: Web scraping
  - `selenium`: Web automation

- **Install Command:**
  
```bash

pip install flask
pip install django
pip install fastapi
pip install requests
pip install beautifulsoup4
pip install selenium

```

---

## 8. Cybersecurity and Cryptography

- **Modules:**
  
  - `cryptography`: Encryption and security
  - `paramiko`: SSH protocol
  - `hashlib`: Hashing algorithms
  - `scapy`: Packet manipulation
  - `shodan`: Interfacing with Shodan API

- **Install Command:**

```bash

pip install cryptography
pip install paramiko
pip install hashlib
pip install scapy
pip install shodan

```

---

## 9. Development and Debugging Tools

- **Modules:**
  
  - `pytest`: Testing framework
  - `unittest`: Built-in testing framework
  - `pdb`: Python debugger
  - `jupyterlab`: Interactive notebooks
  - `black`: Code formatting
  - `mypy`: Static type checker

- **Install Command:**

```bash

pip install pytest
pip install jupyterlab
pip install black
pip install mypy

```

---

## 10. Cloud and DevOps

- **Modules:**
  
  - `boto3`: AWS SDK
  - `azure`: Azure SDK
  - `google-cloud`: GCP SDK
  - `docker`: Docker API for Python
  - `ansible`: IT automation

- **Install Command:**

```bash

pip install boto3
pip install azure
pip install google-cloud
pip install docker
pip install ansible

```

---

## 11. Miscellaneous

- **Modules:**

  - `tqdm`: Progress bars
  - `loguru`: Logging
  - `pyinstaller`: Convert scripts to executables
  - `pytz`: Time zone calculations

- **Install Command:**

```bash

pip install tqdm
pip install loguru
pip install pyinstaller
pip install pytz

```

---

## 12. GUI Modules

- **Modules:**

- `Tkinter`: Standard Python interface for the Tk GUI toolkit.
- `PyQt`: Python bindings for the Qt application framework.
- `PySide`: Official Python bindings for Qt, with LGPL licensing.
- `wxPython`: Wrapper for the wxWidgets C++ library, provides native-looking applications.
- `Kivy`: Framework for building cross-platform applications, especially for mobile and multitouch.
- `FLTK`: Lightweight and fast GUI toolkit, with Python bindings.
- `PyGTK`: Python bindings for GTK, commonly used in Linux applications.
- `Dear PyGui`: Fast and easy-to-use GUI toolkit with modern features.
- `TkinterDnD`: Adds drag-and-drop functionality to Tkinter-based applications.
- `Flask`: Web framework that can be used for web-based GUIs (with Flask-WTF).
- `PySimpleGUI`: A wrapper around Tkinter, Qt, WxPython, and Remi to simplify GUI creation.

- **Install Command:**

```bash

pip install tk
pip install pyqt5
pip install pyside2
pip install wxPython
pip install kivy
pip install fltk
pip install pygtk
pip install dearpygui
pip install tkinterdnd2
pip install flask flask-wtf
pip install PySimpleGUI

```
