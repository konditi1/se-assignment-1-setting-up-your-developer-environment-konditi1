# Ecommerce Project Setup

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Setup Process](#setup-process)
  - [Step 1: Creating and Activating Python Virtual Environment](#step-1-creating-and-activating-python-virtual-environment)
  - [Step 2: Initializing Node.js Project](#step-2-initializing-nodejs-project)
  - [Step 3: Installing Dependencies](#step-3-installing-dependencies)
  - [Step 4: Configuring Scripts](#step-4-configuring-scripts)
  - [Step 5: Creating the Server File](#step-5-creating-the-server-file)
  - [Step 6: Starting the Server](#step-6-starting-the-server)
- [Step-by-Step Guide to Install and Configure MySQL on Ubuntu](#step-by-step-guide-to-install-and-configure-mysql-on-ubuntu)


## Introduction
This document provides a detailed guide on setting up a development environment for an ecommerce project using Python and Node.js. The setup includes creating a Python virtual environment, initializing a Node.js project, installing necessary dependencies, and configuring start scripts.

## Prerequisites
Before starting the setup process, ensure you have the following installed on your system:

- **Python** (version 3.6 or higher)
  - To check if Python is installed and its version:
    ```bash
    python --version
    ```
  - To install Python on Linux:
    ```bash
    sudo apt update
    sudo apt install python3
    ```

- **Node.js** (version 12 or higher)
  - To install Node.js on Linux:
    ```bash
    sudo apt update
    sudo npm install -g n
    sudo n lts
    ```

- **npm** (Node Package Manager, usually comes with Node.js)
  - To check if npm is installed and its version:
    ```bash
    npm -v
    ```
  - To update npm to the latest version:
    ```bash
    npm install -g npm
    ```

To verify the installation of Python, Node.js, and npm, run the following commands:
```bash
python --version
node -v
npm -v

## Prerequisites
Before you start, ensure you have:
- Administrative privileges on your system.
- An internet connection to download the installation files.

### Step 1: Checking Existing npm Installation
Before installing npm, check if npm is already installed on your system and its version.

1. **Open a terminal or command prompt.**
2. **Run the following command:**
   ```bash
   npm -v
   sudo apt update
   sudo npm install -g n
   sudo n lts
```
### Updating npm
```npm install -g npm```

To verify the installation of Python, Node.js, and npm, run the following commands:
```bash
python --version
node -v
npm -v
```
# Setup Process
## Step 1: Creating and Activating Python Virtual Environment
``` mkdir ecommerce```
```cd ecommerce```
### Create a virtual environment:
``` python -m venv plp```
### Activate the virtual environment:
``` source plp/bin/activate```
# Step 2: Initializing Node.js Project
```
 npm init -y
 ```
# Step 3: Installing Dependencies
```
    npm install express
```
```
    sudo npm install -g nodemon
```
# Step 4: Configuring Scripts
#### Update the scripts section in your package.json file to include start and development scripts:
```
{
  "name": "ecommerce",
  "version": "1.0.0",
  "description": "Ecommerce Website",
  "main": "app.js",
  "scripts": {
    "start": "node app.js",
    "dev": "nodemon app.js"
  },
  "dependencies": {
    "express": "^4.17.1"
  },
  "devDependencies": {
    "nodemon": "^2.0.0"
  }
}
```
# Step 5: Creating the Server File
- Create app.js file in your project directory:

# Step 6: Starting the Server
**Start the server:**
```
    npm start
```
For development:
```
npm run dev
```
# Step-by-Step Guide to Install and Configure MySQL on Ubuntu

## Step 1: Update Package Repository

First, ensure your package repository is up to date:

```bash
sudo apt update
```
# Step 2: Install MySQL Server
```
sudo apt install mysql-server
```