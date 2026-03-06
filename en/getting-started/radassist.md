---
title: RadAssist: AI-Powered Project Creation
description: 
published: true
date: 2026-02-16T10:15:58.298Z
tags: 
editor: markdown
dateCreated: 2026-02-16T10:15:55.297Z
---

# RadAssist: AI-Powered Project Creation

RadAssist is an intelligent, step-by-step wizard that integrates Artificial Intelligence into your development workflow. Designing a normalized, efficient database schema is the most critical part of any application; an improper design can lead to unforeseen issues later.

RadAssist acts as your **AI Assistant**, helping you transform a simple concept into a professional database structure. While the AI does the heavy lifting, you maintain complete control at every step, allowing you to fine-tune the results before any code is generated.

## Getting Started

![radassist-select-frameworks.png](/assets/radassist/radassist-select-frameworks.png)

To begin, go to the startup screen and perform the following:

1. **Select Backend Framework**: Choose your preferred server-side technology.
    
2. **Select UI Framework**: Choose your preferred frontend technology.
    
3. **RadAssist AI**: Click this button to launch the wizard.
    

---

## Step 1: Enter Your Prompt

![radassist-prompt.png](/assets/radassist/radassist-prompt.png)

The first step is to describe your application concept to the AI.

- **Select Database (1)**: Choose the database engine you wish to use (e.g., **MARIADB**, **MSSQL**, **POSTGRE**, or **SQLITE**).
    
- **Describe your application concept (2)**: In the text area, provide a brief description of what your app does. You don't need a detailed technical document; a simple sentence like _"Create a dental clinic management system"_ is enough for the AI to start.
    
- **Status Bar (3)**: Displays the current readiness of the AI and the tokens used for the request.
    
- **Next (4)**: Click this to allow the AI to suggest a list of tables based on your description.
    
- **Cancel**: 
	
  ![radassist-cancel-prompt.png](/assets/radassist/radassist-cancel-prompt.png)
  
  If you click Cancel, a confirmation prompt will appear warning that **all AI-generated content will be lost** if you quit the wizard.

---

## Step 2: Select Tables to Generate Fields

![radassist-tablelist.png](/assets/radassist/radassist-tablelist.png)

Based on your prompt, RadAssist will propose a list of database tables.

- **Table Configuration Area (1)**: This area allows you to manually influence the schema.
    
    - **Table Name**: Specify a name for a new custom table.
        
    - **Table Description (Context)**: Describe the purpose of the table. You can also mention specific field names you want included here.
        
    - **Add to List**: Click this to add your custom-defined table to the existing AI suggestions.
        
- **Table List Toolbar (2)**:
    
    - **Edit (Pencil Icon)**: Select a table from the list and click this icon to load its details back into the Configuration Area (1). Once you've made changes, click **Update** to save them.
        
    - **Delete (Red X Icon)**: Select a table and click this to remove it from the list. **Warning:** This action cannot be undone; ensure the table is truly unnecessary before deleting.
        
- **Table List (3)**: This grid displays all tables that will be generated. You can uncheck the box next to a table name to exclude it from the final generation without deleting it.
    

---

## Step 3: Review Fields and Relationships

![radassist-tablefields.png](/assets/radassist/radassist-tablefields.png)

RadAssist now generates the specific fields for each table, including data types and relationships.

- **List of Tables**: Located on the far left, click any table name to view its specific fields in the main grid.
    
- **Fields Management Toolbar**: Use these buttons to manually override the AI's suggestions:
    
    - **Delete (Red X)**: Remove the selected field from the table.
        
    - **Move Up/Down (Arrows)**: Change the visual order of the fields within the table.
        
- **List of Table Fields**: This grid allows you to review technical details for every field:
    
    - **Field Name**: The actual column name in the database.
        
    - **Type & Length**: The data type (e.g., INT, VARCHAR, TEXT) and its maximum character length.
        
    - **Nullable**: Defines if the field can be left empty (True/False).
        
    - **Default**: Sets a default value (e.g., CURRENT_TIMESTAMP for dates).
        
    - **PK (Primary Key)**: Indicates if this field is the unique identifier for the table.
        
    - **Foreign Key**: Shows relationships between tables (e.g., `patients(patient_id)`), ensuring data integrity across your app.
        

---

## Step 4: Project Configuration & Database Creation

![radassist-project-config.png](/assets/radassist/radassist-project-config.png)

The final step defines your project properties and prepares the physical database.

- **Project Name**: Enter the name for your new RadSystems project.
    
- **Project Location**: Choose the directory on your computer where the source code will be saved.
    
- **Site Address**: Define the local development URL (e.g., `http://localhost:8050/`).
    
- **Enable Multi Language**: Check this to enable localization support and select your **Default Language**.
    
- **Project Icon**: Choose the icon set for your UI components.
    
- **Database Server Configuration**:
    
    - **Server/User/Password**: Enter your local database credentials (e.g., `localhost` and `root`).
        
    - **Database**: You can select an existing database or **type a new name**. If the name doesn't exist, RadAssist will create it for you.
        
- **Finish**: Click this to finalize the process.
    

### **Database Conflicts**

If a table name already exists in your database, RadAssist will display an error message asking you to rectify the conflict. You can use your favorite database management tool to rename or delete the conflicting tables, then return to RadAssist and click **Finish** again. All your configurations and AI-generated fields are retained during this process.

Once complete, your project is fully scaffolded and ready for you to start building advanced logic in RadSystems Studio!