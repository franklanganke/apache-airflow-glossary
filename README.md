# discover-airflow
Confusing / missing stuff on Apache Airflow documenation

# Scheduler
* Scheduler starts the executor on startup.
* Scheduler sends tasks to the executor.

# Executor

## SequentialExecutor
* Default configured executor: runs a single task at a time.
* Runs out-of-the-box with local file-db.

## LocalExecutor
 * Parallelize task instances locally.
 * Depends on real database backend like MySQL or Postgres.
 
## CeleryExecutor 
 * Scaling out of workers
 * Depends on Celery
 * Celery depends on a broker (RabbitMQ, Redis, AWS SQS)
 * does celery need a db backend?
