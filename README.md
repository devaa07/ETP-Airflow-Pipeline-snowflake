# ETP-Airflow-Pipeline-snowflake
pipeline to create table and insert records on snowflake with airflow on AWS EC2

![Screen Shot 2023-12-30 at 8 07 18 PM](https://github.com/devaa07/ETP-Airflow-Pipeline-snowflake/assets/126756574/3d5ec534-3f3c-45d2-b13e-014c4a1e3d81)


# Step 1: Creating an EC2 instance and assign relevant Key-value pair, Security group

# Step 2: Install dependencies on EC2 instance(Airflow) 
        sudo apt update
        sudo apt install python3-pip
        sudo apt install python3.10-venv
        python3 -m venv airflow_snow_venv
        source airflow_snow_venv/bin/activate
        sudo pip install apache-airflow
        pip install apache-airflow-providers-snowflake
        pip install snowflake-connector-python
        pip install snowflake-sqlalchemy
        airflow standalone
        pip uninstall pydantic==2.0
        pip install pydantic==1.10.10

  # Step 3: Build the DAG, Look the DAG code file in the repo
            snow.py

  # Step 4: Trigger the DAG and everything is successful!!

  ![Screen Shot 2023-12-30 at 8 12 47 PM](https://github.com/devaa07/ETP-Airflow-Pipeline-snowflake/assets/126756574/a75f660c-87ab-4d36-965a-65b3b40f0c5c)
