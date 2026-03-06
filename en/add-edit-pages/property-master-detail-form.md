---
title: Master Detail Form Property
description: 
published: true
date: 2026-03-06T08:22:40.580Z
tags: 
editor: markdown
dateCreated: 2026-03-06T08:22:37.721Z
---

# Page Master Detail Form on Add Page

![rs-crud-addpage-pagemasterdetailform.webp](/assets/add-edit-properties/rs-crud-addpage-pagemasterdetailform.webp)

The **Master Detail Form** is one of the most powerful features in RadSystems Studio, enabling the creation of complex, nested forms. This functionality allows you to save a master record and multiple related child records—such as an invoice and its individual line items—simultaneously within a single database transaction. This ensures data integrity and provides a seamless experience for high-volume data entry tasks.

The **Page Master Detail Form** dialog is accessed via the button in the Add or Edit Page properties. The interface is divided into a management toolbar, a list of detail forms, and a relationship configuration panel.

### Detail Forms Management

![rs-crud-addpage-pagemasterdetailform-ui.webp](/assets/add-edit-properties/rs-crud-addpage-pagemasterdetailform-ui.webp)

#### Adding Detail Form

The left panel features a toolbar with four essential buttons for managing your nested forms:

- **Add Detail Form (Green Plus)**: Clicking this adds a new entry to the list of detail forms. Once added, ensure this new entry is selected to begin configuring its specific relationship.
    
- **Reorder Arrows (Up/Down)**: These allow you to change the sequence in which the nested forms appear on your page.
    
- **Remove Detail Form (Red Cross)**: Permanently deletes the selected nested form from the master configuration.
    

#### Master Detail Relation

Once a detail form is selected, you must define the technical link between the master and child records in the right-hand panel:

**Relation Type**: Choose the database relationship logic, typically either **OneToOne** or **OneToMany**. For example, one invoice usually has many invoice items.

**Detail Page**: Select the specific "Add" form for the child table from the dropdown list of available project pages. This tells the system which form structure to embed within the master page.

**Referenced Field**: Select the foreign key field from the child table that links back to the master table's primary key (e.g., `invoice_id`). This ensures that when the master record is created, its new ID is automatically passed and saved into every related child record in the same transaction.

After selecting the referenced field, a text summary of the link (e.g., `Invoices.id = invoiceitems.invoice_id`) will appear at the bottom of the panel. It is crucial to cross-check this summary to confirm the relationship is set properly, as this link is the foundation for the entire master-detail transaction.

---

**Output**

![rs-crud-addpage-pagemasterdetailform-output.webp](/assets/add-edit-properties/rs-crud-addpage-pagemasterdetailform-output.webp)