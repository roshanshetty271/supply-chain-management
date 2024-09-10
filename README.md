# Supply Chain Management Project

## Overview

The Supply Chain Management project is aimed at optimizing workflows from product design to production. It focuses on:

- Regulating internal departmental structures and roles.
- Enhancing the management of materials from diverse vendors.
- Streamlining the invoice handling process with clear sender identification.

## Purpose

The primary objectives of this project include:

- **Managing Departments and Staff:** Ensuring clear assignments and responsibilities across departments, warehouses, and production lines.
- **Overseeing Product Lifecycle:** Managing the entire product lifecycle from design conceptualization to manufacturing.
- **Vendor and Invoice Management:** Efficiently tracking and processing vendor-supplied invoices to ensure seamless financial operations.

## Features

### Entity Relationship Diagram (ERD)

Provides a clear visualization of the relationships between various entities within the supply chain, including products, raw materials, vendors, warehouses, and supply schedules.

### Views

- **Product Supply Chain View**
  - **Data Source:** Product, ProductMaterial, RawMaterial, Warehouse, SupplySchedule, and Vendor.
  - **Purpose:** Offers a consolidated snapshot of the supply chain, tracking the flow of raw materials from vendors to warehouses and ultimately to products.

- **Product Warehouse View**
  - **Data Source:** Product, ProductMaterial, RawMaterial, and Warehouse.
  - **Purpose:** Provides a simplified representation of the relationship between products and the warehouses where their raw materials are located.

### Triggers

- **AuditEmployeeSalaryChange:** Monitors updates to the salary column in the "Employee" table and logs changes.
- **AuditProductCostChange:** Monitors updates to the cost column in the "Product" table and logs changes.

### Indexes and Functions

- **Non-clustered Index:** Created for employee last name, department name, and product name for faster data retrieval.
- **User-Defined Functions:** Custom functions to support specific database operations.

### Stored Procedures

- **Assign Employee to Department:** Checks for the existence of both employee and department, then inserts the assignment into the DepartmentEmployee table.
- **Update Product Price:** Updates the price of a product in the "Product" table and communicates the success or failure of the update operation.

### Power BI Dashboards

- **Dashboards:** Provide visual insights into the supply chain management, facilitating data-driven decisions.

### Graphical User Interface (GUI)

- **Home Screen:** Each screen contains records of specific entities with options to create new records, update, or delete existing ones.

## Authors

- **Roshan Shetty**
- **Vrishab Loknath Shetty**
- **Vamsi Naradasu**
- **Shobaraajeswar Elango**


