---
title: Setup
layout: page
nav_order: 6
---

# Setting Up Docker Environment in Visual Studio Code
This guide will walk you through the steps to set up the development environment for ROB 320. 

## Prerequisites
- If not already completed, follow the [EECS 280 Setup Tutorial](https://eecs280staff.github.io/tutorials/) with Visual Studio Code as your IDE.

## Installation Steps
1. **Install Docker**
   - Download and install Docker from the [official Docker website](https://www.docker.com/get-started).
   - Run the Docker Desktop application.
2. **Install Docker Extension for Visual Studio Code**
   - Open Visual Studio Code.
   - Go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window or use the keyboard shortcut `Ctrl+Shift+X`.
   - Search for "Docker" and install the official [Docker](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker) extension.
   - Search for "Dev Containers" and install the [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension.
3. **Verify Docker Installation**
   - Open a terminal in Visual Studio Code.
   - Run the following command to check if Docker is installed:
     ```bash
     docker --version
     ```
   - You should see the installed Docker version information.

## Test the Setup
1. **Pull a Sample Docker Image**
   - Open a terminal in Visual Studio Code.
   - Run the following command to pull a sample Docker image:
     ```bash
     docker pull hello-world
     ```
   - This command downloads a test image to verify that your Docker installation is working.
2. **Run the Sample Container**
   - Run the following command to start a container from the downloaded image:
     ```bash
     docker run hello-world
     ```
   - If everything is set up correctly, you should see a message indicating that your Docker installation is working.

## Install the ROB 320 Development Docker Image
1. **Pull the Docker Image**
   - Open a terminal in Visual Studio Code.
   - Run the following command to pull the Docker image:
     ```bash
     docker pull broderio/rob320student:latest
     ```
2. **Run and Start the Container**
   - Run the following command to run a container from the downloaded image:
     ```bash
     docker run --name rob320_dev -it -d -p 8000:8000 -p 8008:8008 broderio/rob320student:latest
     ```
   - Now that you have created the container, from here on out, you can use this command to start the container:
     ```bash
     docker start rob320_dev
     ```
3. **Open the Container in Visual Studio Code**
   - In Visual Studio Code, navigate to the Docker extension. You should see a green arrow followed by the image name and the container name.
   - Right-click on the container and press "Attach Visual Studio Code."
   - A new Visual Studio Code window should open and look like a typical workspace. This workspace exists within the Docker container, so any code written in this workspace will be saved within the container. Any code that is run will be run in the container. This will be the way that you develop code for this course.
That's it! You've successfully set up the Docker environment for ROB 320. If you encounter any issues or have questions, feel free to reach out during office hours.
