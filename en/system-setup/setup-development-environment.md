---
title: Setup Development Environment
description: Here are some simple steps and tips to setup your development environment to make the best use of RadSystems Studio.
published: true
date: 2026-02-16T09:56:12.059Z
tags: 
editor: markdown
dateCreated: 2023-08-14T07:27:21.581Z
---

# Setup Local Development Environment

To get RadSystems Studio up and running smoothly, we need to set up our local development environment with some essential third-party tools. Since RadSystems Studio supports various Development Stacks, each stack comes with its unique Local Development Environment requirements. First, choose your preferred Development Stack and then follow the instructions tailored specifically for it. This way, you'll have everything you need to start creating amazing apps right away! 

## Setup Backend Framework
## SetupBackendFrameworkTabs {.tabset}

### PHP Laravel

Setting up a local development environment for PHP Laravel app development is essential for building robust and efficient applications. Here's an elaboration of the steps to guide you through the process:

**Step 1: Download and Install Node.js:**
Node.js is a runtime environment that facilitates various development tasks. To install Node.js:

1. Visit the official Node.js website (https://nodejs.org/).
2. Download the recommended version for your operating system (Windows, macOS, or Linux).
3. Run the installer and follow the on-screen instructions to complete the installation.

**Step 2: Download and Install Composer:**
Composer is a dependency management tool for PHP. To install Composer:

1. Visit the official Composer website (https://getcomposer.org/).
2. Download the Composer installer for your operating system.
3. Run the installer and follow the instructions to complete the installation.

**Step 3: Download and Install XAMPP or Any Other LocalHost Server:**
A local server environment is essential for running PHP applications. You can use XAMPP or any other suitable local server software:

1. Download XAMPP from the official website (https://www.apachefriends.org/).
2. Install XAMPP, and during installation, select the necessary components like phpMyAdmin for MySQL etc

Make sure you install XAMPP outside Windows UAC protected folder paths, such as Program Files. Also, it's recommended to avoid spaces in the installation path. 

**Step 4: Setup Environment Variables:**
Configuring environment variables ensures that your development environment is properly recognized by your system:

1. Open your system's Environment Variables settings.
2. Add following paths to your system's PATH variable.
   1. Path to the "bin" directory of your PHP installation, 
   2. Path to the "bin" directory of your Composer installation, and 
   3. Path to the "bin" directory of your Node.js installation 


**Step 5: Check the Setup:**
Once you've completed the setup steps, it's crucial to verify that everything is working as intended:

1. Open a terminal or command prompt.
2. Run the following commands to check installations:
   - To check Node.js installation: `node -v`
   - To check Composer installation: `composer --version`
   - To check XAMPP installation: Access the XAMPP control panel and ensure Apache and MySQL are running.

Remember to refer to Laravel's official documentation (https://laravel.com/docs) for further guidance and resources.

### Python Flask

Setting up a local development environment for Python Flask app development is easy. Here's an elaboration of the steps to guide you through the process:

**Step 1: Download and Install Node.js:**
Node.js is a runtime environment that supports various development tasks. To install Node.js:

1. Visit the official Node.js website (https://nodejs.org/).
2. Download the recommended version for your operating system (Windows, macOS, or Linux).
3. Run the installer and follow the on-screen instructions to complete the installation.

**Step 2: Download and Install Python:**
Python is a fundamental programming language for Flask development. To install Python:

1. Visit the official Python website (https://www.python.org/).
2. Download the latest version compatible with your operating system.
3. Run the installer and follow the instructions, ensuring you select "Add Python to PATH."

**Step 3: Install PIP as Package Manager:**
PIP is a package manager used to install Python packages. To ensure you have PIP:

1. Open a terminal or command prompt.
2. Run the following command:
   ```
   python -m ensurepip --default-pip
   ```

**Step 4: Install Flask:**
Flask is a web framework for Python. To install Flask:

1. Open a terminal or command prompt.

2. Run the following command:

   ```
   pip install flask
   ```

**Step 5: Setup Environment Variables:**
Setting up environment variables is important to ensure your development environment is recognized by your system:

1. Open your system's Environment Variables settings.
2. Add the path to your Python installation directory and PIP installation directory to the PATH variable.

**Step 6: Check the Setup:**
After completing the setup steps, it's crucial to verify that everything is functioning as expected:

1. Open a terminal or command prompt.
2. Run the following commands to check installations:
   - To check Node.js installation: `node -v`
   - To check Python installation: `python --version`
   - To check Flask installation: `flask --version`

Refer to Flask's official documentation (https://flask.palletsprojects.com/) for further guidance and resources.

### ASP .Net Core 

Setting up a local development environment for ASP .NET Core app development is vital to ensure a seamless coding experience. Here's an elaboration of the steps to guide you through the process:

**Step 1: Download and Install ASP .NET Core SDK:**
The ASP .NET Core SDK provides tools and libraries to develop .NET Core applications. To install it:

1. Visit the official ASP .NET Core website (https://dotnet.microsoft.com/).
2. Download the latest version of the ASP .NET Core SDK for your operating system.
3. Run the installer and follow the on-screen instructions to complete the installation.

**Step 2: Setup Environment Variables:**
Configuring environment variables is crucial to ensure your development environment is recognized by your system:

1. Open your system's Environment Variables settings.
2. Add the path to the ASP .NET Core SDK installation directory to the PATH variable.

**Step 4: Check the Setup:**
After completing the setup steps, it's essential to verify that everything is functioning as expected:

1. Open a terminal or command prompt.
2. Run the following commands to check installations:
   - To check ASP .NET Core SDK installation: `dotnet --version`

By following these steps, you establish a solid foundation for ASP .NET Core app development. With the ASP .NET Core SDK, a local server environment, and properly configured environment variables, you're well-equipped to create robust and efficient ASP .NET Core applications. Remember to refer to ASP .NET Core's official documentation (https://docs.microsoft.com/en-us/aspnet/core) for further guidance and resources as you embark on your ASP .NET Core development journey.

## Setup UI Framework
## SetupUIFrameworkTabs {.tabset}

### Quasar Framework

Setting up a local development environment for the Quasar Framework involves a few straightforward steps to ensure a smooth and efficient development process. Here's a breakdown of the steps:

**Step 1: Download and Install Node.js**
Node.js is a crucial component for modern web development, including Quasar applications. To get started, follow these steps:

1. Visit the official Node.js website (https://nodejs.org/).
2. Download the recommended version for your operating system.
3. Run the installer and follow the on-screen instructions to complete the installation.

**Step 2: Install Quasar**
Quasar CLI simplifies Quasar application development by providing a set of commands to create, build, and manage your projects. To install Quasar, open a command-line interface (CLI) and follow these steps:

1. Open your command-line interface (Command Prompt, Terminal, etc.).
2. Install Quasar CLI globally by running the following command:
   ```
   npm install -g @quasar/cli
   ```

**Step 3: Check the Setup**
After installing Node.js and Quasar, it's a good practice to verify that the setup is successful. Here's what you can do:

1. Open your command-line interface again.
2. Check that Node.js and npm (Node Package Manager) are correctly installed by running:
   ```
   node -v
   npm -v
   ```

3. Confirm that Quasar CLI is installed by running:
   ```
   quasar -v
   ```

If all the version numbers are displayed without any errors, it means that your local development environment for Quasar Framework is successfully set up.

By completing these steps, you establish a solid foundation to start creating dynamic and responsive applications using the Quasar Framework. With Node.js, Quasar CLI, and a functional development environment in place, you're well-equipped to dive into the world of Quasar application development.

### Vue.js Framework

Setting up a local development environment for Vue.js development is essential to ensure a smooth and efficient coding experience. Here's an elaboration of the steps to guide you through the process:

**Step 1: Install Node.js and npm:**
Node.js is a runtime environment that allows you to execute JavaScript on the server side, while npm (Node Package Manager) is used to manage and install JavaScript packages. To install them:

1. Visit the official Node.js website (https://nodejs.org/).
2. Download the recommended version for your operating system (Windows, macOS, or Linux).
3. Run the installer and follow the on-screen instructions to complete the installation.

**Step 2: Install a Vue.js cli:**
With Node.js and a code editor in place, you're ready to install VueJS CLI. Follow these steps:

1. Open a terminal or command prompt.

2. Install the Vue CLI globally by running:
   ```
   npm install -g @vue/cli
   ```

## Setup Development Tools
## SetupDevelopmentToolsTabs {.tabset}

### Electron JS for Desktop Apps

Setting up a local development environment for the Electron JS Framework is essential for creating cross-platform desktop applications. RadSystems Studio handles installation of Electron JS Framework (if not already installed) automatically at the time of compiling Desktop Application. For that, you will need to have NodeJS and NPM installed as well as setup properly on your Windows PC.

**Check if Electron JS is already installed**
After completing the setup steps, it's crucial to verify that everything is functioning as intended:

1. Open a terminal or command prompt.

2. Navigate to your project directory.

3. Run the following command to start an Electron application window:

   ```
   npx electron .
   ```

Please refer to Electron's official documentation (https://www.electronjs.org/) for further guidance and resources for your queries related to Electron-specific development.

### Android Studio for Android Apps

Here are the steps to install and set up Android Studio on a Windows PC:

> We recommend to visit https://developer.android.com/studio/install for the most updated instructions. 
> 
{.is-info}

1. **Download Android Studio:**
   - Visit the official Android Studio download page: https://developer.android.com/studio
   - Click on the "Download Android Studio" button.
   - The website should detect your operating system as Windows. If not, select "Windows" from the dropdown.
   - Download the executable installer file.

2. **Run the Installer:**
   
   - Locate the downloaded installer file (it's usually named something like `android-studio-ide-x.x.x.x-windows.exe`).
   - Double-click the installer to run it.
   
   - Wait for the installation to complete.
   
   - After installation, you'll find a shortcut to Android Studio in the Start menu or on your desktop. Double-click it to launch the program.
   
5. **Android Studio Setup:**
   
   - Follow the "Android Studio Setup Wizard" which will appear on first run of the Android Studio.
   - Follow the steps in the wizard to set up Android Studio. This includes choosing a theme, installing the Android SDK components, and configuring the Android Virtual Device (AVD) emulator.
   
7. **SDK Components Installation:**
   
   - The setup wizard will guide you through installing the necessary SDK components. This might take some time, as it downloads various Android SDK versions, tools, and libraries.
   
8. **Emulator Configuration:**
   
   - If you've chosen to install the Android Virtual Device (AVD) emulator, you'll need to create and configure an emulator device. Follow the wizard's steps to create an AVD with the desired specifications.
   
9. **Finish Setup:**
   
   - Once you've completed the setup wizard, Android Studio should be ready to use.
   
10. **Update and Configuration:**
    
    - Android Studio periodically releases updates with new features and bug fixes. Make sure to keep your installation up-to-date by checking for updates in the "Help" menu.
    - You can also configure various settings, including SDK locations, plugins, and more, through the "File" > "Settings" 

That's it! You should now have Android Studio successfully installed and set up on your Windows PC, ready for Android app development.