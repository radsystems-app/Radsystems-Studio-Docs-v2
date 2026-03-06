---
title: The Main Menu Bar
description: 
published: true
date: 2026-02-16T10:26:21.032Z
tags: 
editor: markdown
dateCreated: 2026-02-16T10:26:18.010Z
---

# The Main Menu Bar

![rs-menubar.png](/assets/radsystems-ui/rs-menubar.png)
The menu bar at the top of the interface provides access to core project management functions, global configurations, and essential developer tools.

## File Menu

![rs-menu-file.png](/assets/radsystems-ui/rs-menu-file.png)

The File menu handles your project-level operations:

- **Open Project (Ctrl+O)**: Browse your system to load an existing RadSystems Studio project file.
    
- **Save Project (Ctrl+S)**: Saves the current state and configurations of your open project.
    
- **Save Project As (Ctrl+Shift+S)**: Creates a duplicate of your current project under a new name or in a different location.
    
- **Exit Application**: Securely closes RadSystems Studio.
    

## Global Settings

This menu allows you to define common configuration settings that are automatically applied to every new project you create. By setting these preferences once, you can standardize your application generation process and save significant time across multiple projects. For a deep dive into available configurations, please refer to the [[Global Settings]] documentation page.

## Tools

![rs-menu-tools.png](/assets/radsystems-ui/rs-menu-tools.png)

RadSystems Studio offers several utility tools to help you manage your local development environment and dependencies:

- **Frameworks Diagnostics**: This tool scans your machine to verify if the required frameworks for your chosen development stack (such as Node.js, PHP, or Python) are properly installed. It displays the current version if a framework is found or notifies you if a required dependency is missing.
    
- **PHP Extensions Manager**: PHP extensions are compiled libraries that extend the core functionality of PHP, such as enabling database drivers or image processing. Certain extensions must be enabled to build PHP Laravel-based applications. While this usually requires finding and manually editing a php.ini file in your localhost environment, RadSystems Studio provides an intuitive interface to manage these with a simple click.
    
- **Edit Environment Variables**: Environment variables are system-wide settings that tell your computer where to find specific software tools. It is often necessary to add certain developer tools to your system PATH to make them available for RadSystems Studio to build applications. This menu gives you direct access to your system's environment variables.

## Help Menu

![rs-menu-help.png](/assets/radsystems-ui/rs-menu-help.png)

The Help menu connects you with support and community resources:

- **Support**: Access official technical support for troubleshooting and advanced queries.
    
- **FaceBook**: Visit the official Facebook page for community updates and news.
    
- **Youtube**: Access a library of video tutorials and walkthroughs.
    
- **Twitter**: Follow the official Twitter account for the latest announcements.
    
- **About**: View the current version information details for your RadSystems Studio installation.