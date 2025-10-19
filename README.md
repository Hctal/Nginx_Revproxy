# Nginx Reverse Proxy with Python Backends

## 📜 Project Description
This project is a beginner-friendly demonstration of setting up an Nginx reverse proxy. It includes two simple Python web servers as backend applications and an Nginx configuration file to route traffic to them. The project also serves as a practical example of debugging a common "404 Not Found" error caused by a port mismatch.

## 📁 Project Files
This repository contains the following files and directories:

*   `Installation_setup`: Contains the commands for installing Nginx and creating the backend applications and server setup.
*   `Nginx_config_proxy_app`: This is the Nginx configuration file that sets up the reverse proxy logic.
*   `Nginx_configuration`: Contains the commands to enable, test, and reload the Nginx configuration.
*   `Debugging`: Contains the commands used for troubleshooting the "404 Not Found" error, including checking jobs and logs.
*   `README.md`: You are here! This file explains the project and how to use the other files.

## 🚀 How to Run the Project

### Prerequisites
*   A Linux environment (tested on Ubuntu).
*   `sudo` or root privileges.
*   `python3` installed.

### 1. Installation and Setup
Follow the commands in the `Installation_setup` file to install Nginx and create the backend applications.

### 2. Configure Nginx
Use the `Nginx_config_proxy_app` file as a reference to create your Nginx configuration. Then, use the commands in `Nginx_configuration` to enable and apply the settings.

### 3. Start Backend Servers
Start your Python servers. These commands are included in the `Installation_setup` file but are repeated here for quick reference.
```sh
cd ~/app1
python3 -m http.server 8080 > /dev/null &
cd ~/app2
python3 -m http.server 8081 > /dev/null &
