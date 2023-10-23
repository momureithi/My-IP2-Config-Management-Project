This document provides details of the Ansible playbook structure and roles used to deploy the Yolomy e-Commerce web application. 

## Project Structure

The directory structure of the project is organized as follows:

- `playbook.yml`: The main Ansible playbook that orchestrates the deployment process.

- `roles/`: This directory contains the roles used in the playbook.

  - `clone-repository/`: Responsible for cloning of the repository from GitHub.

  - `docker-setup`: Responsible for the installation and starting of Docker, and containerization of the web application.

  - `network-setup`: Responsible for the creation of a custom bridge network.

  - `database-setup`: Responsible for the statrting of the MongoDB container.

  - `backend-setup/`: Responsible for setting up the backend of the application.

  - `frontend-setup/`: Responsible for setting up the frontend of the application.

- `tasks/`: The `tasks/main.yml` files within each role contain specific tasks related to that role.

## Commands Utilized

```ansible-galaxy init <role-name>``` - to create the specific roles

```ansible-playbook playbook.yaml``` - to run the Ansible playbook