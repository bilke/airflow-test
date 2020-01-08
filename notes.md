## Setup

```bash
virtualenv .venv
source .venv/bin/activate
pip install -r requirements.txt
airflow initdb
airflow webserver -p 8080
airflow scheduler
# Create ssh connection id `ssh_singularity1_conn_id`
airflow test ssh_example test_ssh_operator [current date]
```

## Tutorials

- https://hackersandslackers.com/data-pipelines-apache-airflow/
- https://hackersandslackers.com/automate-ssh-scp-python-paramiko

## Problems

- https://stackoverflow.com/questions/38992997/dag-not-visible-in-web-ui

## Ideas 

- https://kubernetes.io/blog/2018/06/28/airflow-on-kubernetes-part-1-a-different-kind-of-operator/
