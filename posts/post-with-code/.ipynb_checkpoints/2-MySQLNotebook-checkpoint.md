---
jupytext:
  formats: ipynb,md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.14.5
kernelspec:
  display_name: Python 3 (ipykernel)
  language: python
  name: python3
---

# MySQL Check (Sample Notebook for preview ipynb)
> A tutorial of SQL Basics Scripting.

- toc: true 
- badges: true
- comments: true
- categories: [SQL]

# **Resources:**  
+ https://www.educba.com/data-science/data-science-tutorials/mysql-tutorial/  
+ https://www.w3schools.com/mysql/default.asp

```{code-cell} ipython3
:azdata_cell_guid: 3440b9ca-03e9-4fc9-b924-ed383519f471
:language: sql

USE world;
SELECT * from city limit 5;
```

```{code-cell} ipython3
:azdata_cell_guid: c7da93ac-bb67-4b9a-a319-ea701d1bce57
:language: sql

# LECTURE: Creating a Database - Part I here we are creating Sales Database

CREATE DATABASE IF NOT EXISTS Sales;

CREATE SCHEMA IF NOT EXISTS Sales;
```

```{code-cell} ipython3
:azdata_cell_guid: c0fa8df0-88ef-4a27-bd65-407157246b4f
:language: sql

#  use Sales database
USE Sales;
```

```{code-cell} ipython3
:azdata_cell_guid: 3d64b7a9-3d2e-4690-b4fc-13df3d47c860
:language: sql

CREATE TABLE sales
(
    purchase_number INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    date_of_purchase DATE NOT NULL,
    customer_id INT,
    item_code VARCHAR(10) NOT NULL

);
```
