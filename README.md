# Frontend-Reactjs
Built a Restaurent-Registartion WebApp UI using Reactjs along with Bootstrap 

Sure! Below is a README file for the series of commands you provided. This file explains what each command does and guides users through the process of installing Docker on a system, running a test container, and setting up Docker to start on boot.

---

# Docker Installation and Setup Guide

This guide will help you install Docker on your system, run a test container to verify the installation, and set up Docker to start on boot. Follow the steps below to get started.

## Prerequisites

- A Unix-based operating system (e.g., Ubuntu)
- Sudo privileges

## Installation Steps

1. **Update Package Information**
   ```sh
   sudo apt-get update
   ```
   This command updates the local package index, which helps ensure that you have the latest information on the newest versions of packages and their dependencies.

2. **Install Docker**
   ```sh
   sudo apt-get install docker.io -y
   ```
   This command installs Docker from the default Ubuntu repositories. The `-y` flag automatically confirms the installation, so you don't have to manually approve it.

3. **Start Docker Service**
   ```sh
   sudo systemctl start docker
   ```
   This command starts the Docker service. Docker must be running to use Docker commands.

4. **Run a Test Docker Container**
   ```sh
   sudo docker run hello-world
   ```
   This command runs a test container to verify that Docker is installed and working correctly. If Docker is installed correctly, you will see a message from the "hello-world" container.

5. **Check Running Processes**
   ```sh
   sudo ps
   ```
   This command lists the currently running processes. It can help verify that Docker is running as expected.

6. **Change Permissions on Docker Socket**
   ```sh
   sudo chmod 666 /var/run/docker.sock
   ```
   This command changes the permissions of the Docker socket file to allow non-root users to run Docker commands. Be cautious with this command, as it grants all users read and write access to the Docker socket, which can be a security risk.

7. **Enable Docker to Start on Boot**
   ```sh
   sudo systemctl enable docker
   ```
   This command configures Docker to start automatically at boot time.

8. **Verify Docker Installation**
   ```sh
   docker --version
   ```
   This command checks the installed version of Docker to ensure it's installed correctly.
 

