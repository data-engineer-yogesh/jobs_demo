# jobs_demo

Databricks Lakeflow Jobs Demo
This repository demonstrates the core features of Databricks Lakeflow Jobs through practical examples. It is designed to help data engineers understand how to build, configure, and orchestrate production-ready workflows using Lakeflow Jobs.

------------------------

### Project Overview
This project covers the following Lakeflow Jobs concepts with hands-on examples:

1.  Overview and Demo of Lakeflow Jobs
2.  Classic Job Compute
3.  Python Script Tasks
4.  Passing Parameters into Notebook Tasks
5.  Passing Task Values Between Notebook Tasks
6.  Passing Parameters into Python Script Tasks
7.  Task Failures and Dependencies
8.  Concurrent Executions
9.  Branching Control with the If-Else Task
10. Running Tasks in a Loop with the For Each Task

---------------------
###  Topics Covered
1. Lakeflow Jobs Overview
Introduction to Lakeflow Jobs
Creating and scheduling jobs
Managing workflows
Monitoring job execution

2. Classic Job Compute
Learn how to:
Configure Classic Job Compute
Select cluster configurations
Run jobs on dedicated compute resources

3. Python Script Tasks
This example demonstrates:
Running standalone Python scripts
Configuring Python task execution
Managing script parameters

4. Passing Parameters into Notebook Tasks
Examples include:
Base Parameters
Widgets Dynamic parameter values

5. Passing Task Values Between Notebook Tasks
Learn how one task can produce output and another task can consume it using task values.

```
Example Flow:

Notebook A
      │
      ▼
Set Task Value
      │
      ▼
Notebook B
Reads Task Value

```

6. Passing Parameters into Python Script Tasks
This section demonstrates:
Named parameters
Command-line arguments
Dynamic runtime parameters

7. Task Failures and Dependencies
Examples include:
Success dependency
Failure dependency
Handling failed tasks
Retry behavior

```
Workflow Example:

Task A
 │
 ├── Success → Task B
 │
 └── Failure → Task C

```

8. Concurrent Executions
Learn how to execute multiple tasks in parallel to improve workflow performance.

```
Example:

          Start
            │
     ┌──────┴──────┐
     ▼             ▼
   Task A       Task B
     │             │
     └──────┬──────┘
            ▼
         Final Task

```
9. Branching with If-Else Task
This demo shows conditional execution based on runtime conditions.

```
Example:

        Condition
        /      \
     True      False
      │          │
 Task A      Task B

```

10. For Each Task
Learn how to iterate over a collection and execute the same task multiple times.

Example:

Items:
- File1
- File2

```
For Each Item
      │
      ▼
Process File
```

### Learning Outcomes
After completing this project, you will understand:

- Creating Lakeflow Jobs
- Configuring Job Compute
- Notebook Tasks
- Python Script Tasks
- Parameter Passing
- Task Values
- Dependencies
- Parallel Execution
- Conditional Branching
- For Each Loops
- End-to-End Workflow Orchestration

-------

## Technologies Used :
- Databricks
- Lakeflow Jobs
- Python
- Databricks Notebooks
- Workflow Orchestration

---------------
##  License

This project is licensed under the **MIT License**. You are free to use, modify, and distribute this project for personal and commercial purposes, provided that the original copyright and license notice are included.


---
