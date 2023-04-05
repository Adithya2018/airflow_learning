# Airflow Tutorial

## Part 1 - Run Airflow in Python Env

### Creating new python environment and activate it

```bash
python3 -m venv airflow_tutorial
```

```bash
source airflow_tutorial/Scripts/activate
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
