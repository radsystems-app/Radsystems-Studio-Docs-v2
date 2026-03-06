---
title: List Pagination Property
description: 
published: true
date: 2026-03-05T06:25:58.882Z
tags: 
editor: markdown
dateCreated: 2026-03-05T06:25:55.970Z
---

# List Pagination Settings

![rs-crud-listpage-pagination.webp](/assets/list-view-properties/rs-crud-listpage-pagination.webp)

Pagination is a crucial feature for managing large datasets, as it breaks down content into smaller, manageable chunks. RadSystems Studio offers a comprehensive **Page Load Indicator Settings** window to customize how users navigate through your record lists.

While the functional properties vary by style, the visual properties such as **Button Design** and **Spinner** logic remain consistent across all types. These design classes (like colors and button shapes) automatically adapt to the **Frontend Framework** (Bootstrap or Quasar) you selected during project setup.

The **Pagination** property allows you to choose from several distinct navigation styles. Each style is designed to cater to different user experiences, from traditional numbered pages to modern "infinite" scrolling.

## Common Visual Properties

![rs-crud-listpage-pagination-commonproperties.webp](/assets/list-view-properties/rs-crud-listpage-pagination-commonproperties.webp)

These settings appear across most pagination styles to maintain a consistent look for your navigation controls:

- **ButtonColor**: Sets the theme color for navigation buttons (e.g., `primary`).
    
- **ButtonTextColor**: Defines the color of the text within the buttons.
    
- **ButtonOutline**: When enabled, buttons appear with a transparent background and a colored border.
    
- **ButtonFlat**: Removes all borders and background colors, leaving only the text/icon.
    
- **ButtonGlossy**: Applies a reflective gradient effect.
    
- **ButtonPush**: Simulates a physical button press when clicked.
    
- **ButtonUnelevated**: Removes the drop-shadow from the buttons.
    
- **Loading Text**: The text displayed inside the **Spinner** while new data is being fetched (e.g., `Loading...`).
    

---

## 1. NumericPrevNext Style

![rs-crud-listpage-pagination-numeric.webp](/assets/list-view-properties/rs-crud-listpage-pagination-numeric.webp)

This is the most common pagination style, providing numbered buttons along with "Previous" and "Next" controls.

- **EnablePagination**: Master toggle to turn pagination on or off.
    
- **RecordCount**: Displays the total number of records available in the database.
    
- **UseInputNav**: Adds a text input field where users can type a specific page number to jump to.
    
- **PageCount**: Shows the total number of pages available.
    
- **LimitCount**: Displays the current number of records being shown out of the total.
    
- **LinkRangeLimit**: Sets the number of page buttons to show in the range (e.g., setting it to `5` shows buttons for the next five pages).
    

## 2. PrevNextOnly Style

![rs-crud-listpage-pagination-prevnext.webp](/assets/list-view-properties/rs-crud-listpage-pagination-prevnext.webp)

A simplified navigation style that only offers buttons to move to the immediate next or previous page.

- **NextButtonText**: Allows you to customize the label for the forward button (e.g., `Next`).
    
- **PrevButtonText**: Allows you to customize the label for the backward button (e.g., `Previous`).
    
- **ButtonRowClass**: Lets you apply custom layout classes to the button container.
    

## 3. LoadMore Style

![rs-crud-listpage-pagination-loadmore.webp](/assets/list-view-properties/rs-crud-listpage-pagination-loadmore.webp)

Instead of numbered pages, this style provides a single button at the bottom of the list to fetch the next set of records.

- **LoadmoreButtonText**: Customizes the text on the trigger button (e.g., `Load More`).
    
- **Finished Loading Text**: The message shown when there are no more records to display (e.g., `No more content to load`).
    

## 4. InfiniteScroll Style

![rs-crud-listpage-pagination-infinite.webp](/assets/list-view-properties/rs-crud-listpage-pagination-infinite.webp)

Ideal for modern social or news-style feeds, this style automatically loads the next set of records as the user scrolls to the bottom of the page.

- **LoadmoreButtonText**: While it usually triggers automatically, this text is used if a manual fetch is required.
    
- **Finished Loading Text**: The message displayed at the bottom of the feed once the end of the data is reached.
    

---

## Apply to other pages

At the bottom of the configuration window, you will find the **Apply to other pages** checkbox. Enabling this allows you to synchronize your chosen pagination style and design across all other list pages in your project with a single click.