# IICS_Mapping

An Informatica Intelligent Cloud Services (IICS) sample project containing **Mappings**, **Mapping Tasks**, and a **Taskflow** for a retail sales consolidation use case.

This repository demonstrates how to build an end-to-end ETL pipeline in IICS using reusable mappings and orchestration components.

---

## 📌 Project Overview

The project simulates an **OmniChannel Sales Consolidator** where data from multiple sales sources is processed, transformed, enriched, and summarized.

### Business Scenario

A retail company receives sales data from multiple channels such as:

- Online Store
- Warehouse / Offline Sales
- Product Master Data
- Supplier Data

The goal is to:

✅ Consolidate all incoming sales data  
✅ Clean and standardize records  
✅ Enrich transactions with product/supplier details  
✅ Generate final revenue summary reports  
✅ Automate execution using Taskflow

---

## 📂 Repository Structure

```text
IICS_Mapping-main/
│── Omni_iics.zip          # Exported IICS package
│── README.md

Inside Omni_iics.zip

Explore/Default/
│── Taskflow2.TASKFLOW.xml
│── M_Consolidation_Enrichment.DTEMPLATE.zip
│── M_Final_Summary.DTEMPLATE.zip
│── MCT_Consolidate_Enrich.MTT.zip
│── MCT_Final_Summary.MTT.zip

SYS/
│── hp.AgentGroup.zip
│── conn_flatfile_hcl.Connection.zip
⚙️ Components Included
🔹 Mapping: M_Consolidation_Enrichment

Handles:

Source ingestion
Data cleansing
Null handling
Joining master data
Enrichment logic
Standardization
🔹 Mapping: M_Final_Summary

Handles:

Aggregation
Revenue calculation
Final reporting dataset
🔹 Mapping Tasks
Task Name	Purpose
MCT_Consolidate_Enrich	Executes consolidation mapping
MCT_Final_Summary	Executes summary mapping
🔹 Taskflow
Taskflow	Purpose
Taskflow2	Orchestrates complete ETL process
🚀 How to Import into IICS
Step 1: Login

Login to your Informatica Intelligent Cloud Services organization.

Step 2: Open Data Integration

Navigate to:

Data Integration → Explore
Step 3: Import Package

Upload:

Omni_iics.zip
Step 4: Configure Connections

Update imported connection:

conn_flatfile_hcl

Replace with your:

Flat file path
Database connection
Runtime environment
Secure Agent
Step 5: Run Taskflow

Execute:

Taskflow2
🔄 ETL Flow
Source Files
   ↓
Consolidation Mapping
   ↓
Data Cleansing
   ↓
Master Data Join
   ↓
Enrichment
   ↓
Summary Mapping
   ↓
Final Output
🛠 Technologies Used
Informatica Intelligent Cloud Services (IICS)
Cloud Data Integration
Mapping Designer
Taskflow Designer
Flat File Processing
ETL / ELT Concepts
📈 Learning Objectives

This project is useful for learning:

Real-time IICS project structure
Mapping design best practices
Expression transformations
Aggregator usage
Taskflow orchestration
Reusable ETL architecture
🧠 Use Cases

Suitable for:

IICS Practice Projects
Interview Preparation
Portfolio Showcase
ETL Learning
Data Engineering Basics
📌 Author

Ansh Tiwari

⭐ If you found this useful

Please star the repository and share it with others learning IICS.
