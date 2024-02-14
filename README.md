# airflow-code

## Overview

This repository houses the code, scripts, and libraries utilized by the Airflow instance managed through Helm. It is intended to be mounted to the Helm-Airflow instance via a Git Sync container, ensuring seamless synchronization of DAGs and associated files.

## Contents

1. **DAGs**: Directory containing Airflow DAGs. Each DAG file represents a workflow that can be scheduled and monitored by Airflow.
2. **Scripts**: Collection of utility scripts used within DAGs or for Airflow maintenance tasks.

## Setup

To utilize the contents of this repository within your Airflow instance, follow these steps:

1. Clone this repository to your local machine or server:

```
git clone https://github.com/lukedappleton/airflow-code.git
```

2. Configure the Git Sync container within your Helm-Airflow setup to mount this repository. Ensure appropriate permissions and access control are configured for secure synchronization.

3. Configure your Airflow DAGs to reference the scripts and libraries within this repository as necessary.

## Usage

- **DAGs**: Create or modify Airflow DAG files within the `dags/` directory. Ensure each DAG adheres to Airflow best practices and follows the defined workflow.
- **Scripts**: Develop and maintain utility scripts within the `scripts/` directory. These scripts can be invoked by Airflow tasks to perform various actions or tasks.

## Contributing

Contributions to this repository are welcome! If you have improvements, bug fixes, or new features to propose, please open a pull request. Ensure your code adheres to the established style guidelines and is well-documented.

## License

This repository is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the code as permitted by the license.
