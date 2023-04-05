# Airflow Tutorial

## Pre-Requisites:

1. If Windows, WSL is necessary for the initial parts. If you have Mac or Linux ignore this part.
2. Docker
3. python3 (obviously!!!)
4. Pandas library (pip install pandas)
5. virtualenv library (pip install virtualenv)

## Part 1 - Run Airflow in Python Env

### Creating new python environment and activate it

```bash
python3 -m venv airflow_tutorial
```

```bash
source airflow_tutorial/bin/activate
```

### Installation of airflow

```bash
pip install 'apache-airflow==2.5.3' --constraint "https://raw.githubusercontent.com/apache/airflow/constraints-2.5.3/constraints-3.7.txt"
```

### Setting up airflow

1. Setting up environment variables for airflow

```bash
export AIRFLOW_HOME=.
```

2. Initializing airflow databases:

```bash
airflow db init
```

3. Starting airflow server

```bash
airflow webserver -p 8080
```

## Reference

1. https://youtu.be/K9AnJ9_ZAXE
2. https://stackoverflow.com/questions/67030075/modulenotfounderror-no-module-named-pwd-airflow-python
3. https://stackoverflow.com/questions/72194598/airflow-standalone-cannot-use-relative-path
