---
title: View Page - Properties Overview
description: 
published: true
date: 2026-03-05T11:14:04.286Z
tags: 
editor: markdown
dateCreated: 2026-03-05T11:13:58.898Z
---

# View Page Properties

The **View Page** (often referred to as the **Details Page**) is the dedicated interface where the full details of a single record are displayed. While the List Page provides a broad overview of many records, the View Page allows the user to focus on a specific entry—such as a single invoice or a complete customer profile—displaying all relevant data fields, including those from joined tables.

![rs-crud-viewpage-properties.webp](/assets/list-view-properties/rs-crud-viewpage-properties.webp)

When you select the **View Page** from the List of Pages, the properties panel updates to show settings specifically relevant to displaying individual records. Many properties overlap with the List Page, while others are unique to this detailed view.

### Page Design

**RoutePath**: Defines the unique URL endpoint used to access a specific record (e.g., `invoices/view`).

**PageTitle**: The text displayed at the top of the browser and the page header (e.g., **Invoice Details**).

**DisplayTemplate**: Sets the visual layout for the details. For View Pages, this is set to **Grid** by default to display fields in a structured card format.

**PageSkeletonTemplate**: Defines the visual "placeholder" or shimmer effect shown while the record data is being fetched from the server.

**RecordNavigation**: When enabled, this adds "Previous" and "Next" buttons to the page, allowing the user to cycle through individual record details without returning to the main list.

**Master Detail Display**: Set this to **True** to show nested child records (such as line items) related to this specific master record. Please set up Master Detail Relationship before you enable this option.

**ReloadOnNavigation**: Ensures the record data is refreshed every time the user navigates to this page.

### Default Query Configuration

**Join Tables**: Opens the collection window to link related tables, allowing you to display data from multiple sources on a single details page (e.g., showing the Client's name and address on an Invoice view).

### Record Events

The **Mail Action Settings** allow you to trigger an automated email notification whenever a user views a specific record. This is useful for tracking high-value data access or sending automatic confirmations.

![rs-crud-viewpage-sendmail.webp](/assets/list-view-properties/rs-crud-viewpage-sendmail.webp)

#### Send Mail After Record View

**SendMail**: The master toggle to enable or disable the automated email trigger for this page.

**Mail Title**: The subject line of the email to be sent.

**Mail Body**: The content of the message.

**RecipientEmail**: The email address that will receive the notification.

#### Project Email Setting Configuration

Clicking the **Mail Setting** button opens the global SMTP configuration required for the system to send emails.

**Sender Detail**: Includes the **Sender Name** and **Sender Email** that will appear in the "From" field of the sent messages.

**To Use SMTP Server**: These fields must be filled with your mail provider's credentials, including the **SMTP Host Server**, **SMTP Server Port**, **SMTP Username**, and **SMTP Password**.

### Page Components

**ExportSetting**: Enables the user to export the details of this single record into formats like PDF, allowing for the generation of "Printable" versions of the data.

### Action Buttons

**ActionButtons**: A collection of buttons specifically for this record, such as **Edit** or **Delete**.

**ActionButtonsPosition**: Determines where these buttons are placed on the page, typically at the **Bottom** or top of the detail card.

**ActionButtonsType**: Sets the visual style for these buttons, such as **IconButtons** for a compact look.

**ActionButtonRowClass**: Allows you to apply specific layout classes (e.g., `justify-end`) to the container holding the action buttons, depending on your selected **Frontend Framework**.
