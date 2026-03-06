---
title: RadSystems Studio: Startup Screen Overview
description: 
published: true
date: 2026-02-16T10:03:34.095Z
tags: 
editor: markdown
dateCreated: 2026-02-16T10:03:28.646Z
---

# RadSystems Studio: Startup Screen Overview

Upon launching RadSystems Studio, you are presented with the startup screen, which offers immediate access to your development environment, recent projects, and the options to begin a new application. RadSystems Studio presents a very intuitive user interface, logically divided into different sections for ease of use.

![radsystems-startup.png](/assets/radsystems-startup.png)

## 1. User Interface Sections

### The Menu and Toolbar (1)

The area marked **(1)** contains the main interface controls, including the **Menu Bar** (File, Global Settings, Tools, Help) and the **Button Bar**. This button bar provides quick access to essential actions for managing your project, such as **Save Project**, **Open Project**, **Project Settings**, and tools for managing application components like **Authentication**, **Master Detail Relations**, **Roles and Permissions**, and the final **Publish Project** action.

### Open Recent Projects (2)

The section marked **(2)** is the area where the list of your **recently accessed projects** is displayed.

- To quickly resume work, click the **name of the project** in the list to open it directly in the work area.
- To manage the list, click the **cross button (x)** placed in front of the project title to remove the project from the recent projects list. This does not delete the project files, only the entry from this list.

## 2. Creating a New Application

The central area provides the core options for developing a robust application with just a few clicks.

### Select Backend Framework (3)

The section marked **(3)** lists all the supported **Backend Frameworks** that RadSystems Studio can use to generate your server-side API and logic.

- Options include **PHP - Laravel**, **Node JS - Express**, **Node TS - Express**, **.NET ASP.Net Core**, and **Python - Flask**.
- Click the corresponding button to select the framework you wish to use as the Backend Framework for your new project.

### Select UI Framework (4)

The section marked **(4)** shows all the supported **Front-End (UI) Frameworks** for creating the user interface of your web application.

- Options include **Prime React**, **Prime Vue**, **Quasar Vue**, and **Bootstrap JQuery**.
- Click the corresponding button to select the framework as Frontend Framework to define the look, feel, and functionality of your new project's front-end.

## 3. Starting the Project Creation Process

Once you select your desired frameworks, you have two methods for creating the final project structure:

- **Create Project (5)**: This button starts the new project creation process in **Manual Mode**. Use this option if you already have a **database ready** with a defined schema, which you will connect to in the next step. Clicking this will lead you to the "Create New Project" screen we previously documented.
- **RadAssist (6)**: Click the **RadAssist** button to start an **interactive AI assistant wizard**. This option is ideal if you **do not have a database ready**. RadSystems Studio's RadAssist can help you design your database schema, create the new database, and then automatically create a new project linked to this newly defined database.