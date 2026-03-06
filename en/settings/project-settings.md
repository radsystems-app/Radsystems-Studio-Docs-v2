---
title: Project Settings
description: 
published: true
date: 2026-02-16T10:41:01.387Z
tags: 
editor: markdown
dateCreated: 2026-02-16T10:40:58.238Z
---

# Project Settings

![rs-projectsettings.png](/assets/settings/rs-projectsettings.png)

The **Project Settings** dialog is the central location for configuring application-wide behavior, publishing control, branding, deployment parameters, and system-level integrations. It defines how RadSystems generates your project and how the final application behaves at runtime.

This window contains two major areas: **Publish File Selection** and **Project Information Settings**.

---

## Publish File Selection

This section determines which files are included when the project is generated during the **Publish** process.

![rs-projectsettings-filelist.png](/assets/settings/rs-projectsettings-filelist.png)

The **File List** shows all files involved in the generation routine. Files with a check mark are included in publishing, while unchecked files are skipped. **This is particularly important if you have manually modified generated files outside RadSystems Studio. By removing the check mark, you prevent those files from being overwritten, protecting your customizations.**

The **Search** field filters the file list dynamically as you type, allowing quick location of specific files.

The **Toggle Selection** option selects or deselects all files at once, making bulk changes faster.

---

## Project Information Settings

This section defines global configuration that affects system identity, UI behavior, deployment targets, and runtime behavior.

![rs-projectsettings-projectinfo.png](/assets/settings/rs-projectsettings-projectinfo.png)

### System Info

**Project Name** defines the internal name of the application project.

**Navbar Title Display Mode** controls branding in the application header. You can display both logo and text, only the logo, or only the text.

**Include Footer** determines whether the application footer appears across pages.

**SiteAddr** specifies the base URL where the application is hosted.

**ApiAddr** defines the backend API endpoint used by the frontend for server communication.

**Project Directory** shows the local file system path where project files are stored.

---

### Meta Information

**Meta Keywords** allows you to define keywords describing the application for search engines.

**Meta Site Author** identifies the author or organization behind the application.

**Meta Description** provides a summary of the application used by browsers and search engines.

**Meta Viewport** controls responsive display behavior on different devices and is typically left at its default value.

**Meta Theme Color** defines the browser interface color on supported devices.

---

### Production Info

**Publish To Production** enables production-ready optimizations when activated. This is typically enabled before deploying to a live environment.

---

### System Files

**Project Favicon** defines the icon shown in browser tabs.

**Project Logo** sets the main branding logo used in the application header.

---

### AWS S3 Upload

These settings configure cloud storage integration.

**Access Key** and **Secret Key** provide AWS authentication credentials.

**Bucket Name** specifies the S3 storage bucket.

**Region Name** defines the AWS region where the bucket is hosted.

---

### Misc Settings

**Email Settings** opens the email configuration window used to set up outgoing system mail.  

![rs-projectsettings-projectinfo-emailsettings.png](/assets/settings/rs-projectsettings-projectinfo-emailsettings.png)

Here you define the **Sender Name** and **Sender Email**, along with SMTP server details including **SMTP Host Server**, **SMTP Server Port**, **SMTP Username**, and **SMTP Password**. These settings enable features such as password recovery, notifications, and system alerts.

**Database CharSet** defines the database character encoding.

**Page Encoding** sets the encoding used in generated pages, typically UTF-8.

**Enable Axios Request Cache** improves performance by enabling client-side request caching.

**Default Locale** sets the default language of the application.

**Github Repositories** allows linking repositories for integration or deployment workflows.