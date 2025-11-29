
# Big Data Lab Sessions

This repository contains lab exercises and assignments for **Big Data Lab** sessions. The main focus is on **PySpark** for processing large datasets efficiently using Python.

![PySpark Logo](https://spark.apache.org/images/spark-logo-trademark.png)

---

## 🔹 Prerequisites

Before starting, ensure your system has the following installed:

- **Java 11** (OpenJDK recommended)  
  PySpark requires Java to run. Java 11 is compatible with PySpark 3.4.

- **Python 3.10**  
  The project and virtual environment use Python 3.10 for compatibility with PySpark.

- **PySpark 3.4**  
  PySpark 3.4 is used to run all Spark jobs.

- **Anaconda Navigator** (Recommended)  
  Anaconda provides an easy-to-use environment manager and package installer for data science workflows.

---

## 🔹 Setup Instructions (Option 1: Anaconda Navigator)

**🐍 Using Anaconda Navigator (Recommended)**

1️⃣ **Install Anaconda**
- Download from [Anaconda.com](https://www.anaconda.com/products/distribution)
- Follow the installation wizard for your operating system

![Anaconda Navigator](https://docs.anaconda.com/navigator/img/nav-defaults.png)

2️⃣ **Create Environment via Anaconda Navigator**
- Open Anaconda Navigator
- Click on "Environments" in the left panel
- Click "Create" button
- Name: `pyspark_bigdata`
- Python version: `3.10`

3️⃣ **Install Required Packages**
- Select your `pyspark_bigdata` environment
- Search and install the following packages:
  - `pyspark=3.4.0`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `jupyter`
  - `notebook`

4️⃣ **Launch Jupyter**
- From Anaconda Navigator home
- Make sure `pyspark_bigdata` environment is selected
- Click "Launch" under Jupyter Notebook or JupyterLab

---

## 🔹 Setup Instructions (Option 2: Manual Setup)

Follow these steps to set up your development environment:

1️⃣ **Install Java 11**

- **macOS (Homebrew):**
```bash
brew install openjdk@11
````

* **Linux (Ubuntu):**

```bash
sudo apt update
sudo apt install openjdk-11-jdk
```

* **Windows:**
  Download and install from [Adoptium](https://adoptium.net/) or Oracle.

* **Verify Java version:**

```bash
java -version
```

You should see `java version "11.x.x"`.

---

2️⃣ **Install Python 3.10**

* **macOS (Homebrew):**

```bash
brew install python@3.10
```

* **Linux (Ubuntu):**

```bash
sudo apt install python3.10 python3.10-venv python3.10-dev
```

* **Windows:**
  Download from [Python.org](https://www.python.org/downloads/release/python-3100/).

* **Verify Python version:**

```bash
python3 --version
# or
python3.10 --version
```

---

3️⃣ **Create a Virtual Environment**

```bash
python3.10 -m venv pyspark_env
```

* Activate virtual environment:

  * **macOS / Linux:** `source pyspark_env/bin/activate`
  * **Windows:** `pyspark_env\Scripts\activate`

* Install required packages:

```bash
pip install --upgrade pip
pip install pyspark==3.4.0 pandas matplotlib seaborn
```

---

4️⃣ **Project Structure**

```
bigdata-lab-sessions/
├── Day 01/
│   ├── Assignmentsession.ipynb
│   └── ...
├── Day 02/
│   └── ...
├── pyspark_env/       # Virtual environment (ignored in Git)
├── .gitignore
└── README.md
```

* Make sure to **ignore the virtual environment and .env files** in Git:

```
pyspark_env/
.env
__pycache__/
*.pyc
.DS_Store
```

---

5️⃣ **Running Notebooks**

**Via Anaconda Navigator:**
1. Open Anaconda Navigator
2. Select `pyspark_bigdata` environment
3. Launch Jupyter Notebook or JupyterLab
4. Navigate to the relevant notebook in `Day XX/` folder
5. Run each cell to perform PySpark operations

**Via Command Line:**
1. Activate the virtual environment.
2. Start Jupyter Notebook or Lab:

```bash
jupyter lab
# or
jupyter notebook
```

3. Open the relevant notebook in `Day XX/` folder.
4. Run each cell to perform PySpark operations and analyze data.

---

## 🔹 PySpark Overview

**Apache Spark** is a unified analytics engine for large-scale data processing. **PySpark** provides Python APIs for Spark functionality.

### Key Features:
- **Fast**: In-memory computing capabilities
- **Scalable**: Handles large datasets across clusters
- **Easy to Use**: Simple APIs in Python, Scala, Java, R
- **Versatile**: Batch processing, streaming, machine learning, graph processing

### PySpark Architecture:
```
Driver Program (Python) → SparkContext → Cluster Manager → Worker Nodes
```

![PySpark Architecture](https://spark.apache.org/docs/latest/img/cluster-overview.png)

---

## 🔹 Notes

* **Anaconda Navigator** is the recommended approach for beginners as it provides a visual interface for environment and package management.
* Use **PySpark DataFrames** for efficient large-scale data operations.
* Ensure **Java 11** and **Python 3.10** are correctly set; mismatched versions cause runtime errors.
* Follow the order of lab sessions to avoid dependency issues between notebooks.
* If using manual setup, make sure to activate your virtual environment before running notebooks.

---

## 🔹 Troubleshooting

**Common Issues:**
1. **Java not found**: Ensure Java 11 is installed and `JAVA_HOME` is set
2. **PySpark import error**: Check if PySpark is installed in the correct environment
3. **Kernel not found**: Make sure Jupyter is installed in the same environment as PySpark

**Environment Variables (if needed):**
```bash
export JAVA_HOME=/usr/lib/jvm/java-11-openjdk
export SPARK_HOME=/path/to/spark
export PYSPARK_PYTHON=python3.10
```

---

## 🔹 References

* [PySpark Official Documentation](https://spark.apache.org/docs/latest/api/python/)
* [Apache Spark Official Website](https://spark.apache.org/)
* [Anaconda Navigator Documentation](https://docs.anaconda.com/navigator/)
* [Java 11 Installation Guide](https://adoptium.net/)
* [Python 3.10 Downloads](https://www.python.org/downloads/release/python-3100/)

---

## 🔹 Lab Session Structure

```
Day 01/ - Introduction to PySpark and DataFrames
Day 02/ - Data Processing and Transformations
Day XX/ - Advanced Analytics and Machine Learning
```

**Happy Learning! 🚀**


