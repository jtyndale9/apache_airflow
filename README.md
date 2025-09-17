# apache_airflow
Learning Apache Airflow to orchestrate data engineering pipelines


- Workflow: set of steps to accomplish data engineering task
- Airflow is a platform to program workflows
-   Create, schedule, monitor
- DAG (directed acyclic graphs)
    - Written in python
    - Made up of components (typically tasks) to be executed such as operators
    - Contain dependencies
- Operators: represent a single task in a workflow
    - BashOperator: executes a given bash command or script
    - PythonOperator: executes a python function/callable, can pass arguments
    - EmailOperator: Sends an email
- Task: instance of an operator, assigned to variables in Python, referred to by task_id
- Cron syntax: minute hour day_of_month month day_of_week


Airflow tasks test <dag_id> <task_id> [execution date]
Airflow tasks test example-etl download-file 2024-01-10
Airflow webserver –p 9090
