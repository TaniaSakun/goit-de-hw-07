# goit-de-hw-07
The repository for the 6th GoItNeo Data Engineering homework

## Task Description:
Write a DAG that has the following tasks (each item → one task):
1. Creates a table.

2. Randomly chooses one of the three values ​​['Bronze', 'Silver', 'Gold'].

3. Depending on the chosen value, runs one of the three tasks (branches).

4. Description of the three tasks:
    1) The task counts the number of records in the olympic_dataset.athlete_event_results table that contain the Bronze record in the medal field, and writes the resulting value to the table created in item 1, along with the medal type and the time the record was created.

    2) The task counts the number of records in the olympic_dataset.athlete_event_results table that contain the Silver record in the medal field, and writes the resulting value to the table created in item 1, along with the medal type and the time the record was created.

    3) The task counts the number of records in the olympic_dataset.athlete_event_results table that contain the record Gold in the medal field, and writes the resulting value to the table created in step 1, along with the medal type and the time the record was created.

5. Starts a delay for the next task.

6. Checks with a sensor whether the newest record in the table created in step 1 is not older than 30 seconds (compared to the current time). The idea is to make sure that the record in the table has actually been written.

## Task Results:
![tasks_graph](p1_tasks_graph.png)

![active_tasks_graph](p2_active_tasks_graph.png)

![sql_results](p3_SQL_results.png)

![dag_tasks_chart](p4_DAG_task_chart.png)