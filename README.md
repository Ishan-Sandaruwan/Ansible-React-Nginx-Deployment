# Ansible React Nginx Deployment

Automate the deployment of a React (Vite) frontend application using Ansible and Nginx. This playbook installs Node.js, clones the React app, builds it, and configures Nginx for static website hosting, enabling fast and reliable web deployment with minimal manual setup.

## Features

- Installs the latest Nginx web server
- Adds NodeSource Node.js 22 repository and installs Node.js
- Clones a React (Vite) frontend application from a Git repository
- Installs npm dependencies and builds the React app
- Configures Nginx to serve the static website
- Ensures Nginx is running and enabled on boot

## Prerequisites

- A target server running Ubuntu
- SSH access with a user having `sudo` privileges
- Ansible installed on the control machine

## Usage

1. Clone this repository:
```
git clone https://github.com/Ishan-Sandaruwan/ansible-react-nginx-deployment.git
cd ansible-react-nginx-deployment
```

2. Update your hosts inventory file with your target server

3. Run the Ansible playbook
```
ansible-playbook -i inventory setup_server.yml
```
