# Overwatch-SQL-Analytics
A relational database schema for tracking Overwatch match statistics.
# Overwatch Performance Analytics Engine

### Relational Database Schema & KPI Tracking

**Project Status:** Active | **Role:** Data Architect & Analyst

---

## Project Overview
This project is a relational database design aimed at capturing, storing, and analyzing competitive gameplay data from **Overwatch 2**. 

As a **Business Systems Analyst**, I approached this project to demonstrate how complex operational data (game mechanics) can be translated into a structured SQL schema to drive performance insights. The goal is to move beyond basic win/loss tracking and drill down into granular KPIs that influence match outcomes.

## Key Objectives
- **Data Normalization:** Designed a schema (up to 3NF) to efficiently store Heroes, Maps, Game Modes, and Match History without redundancy.
- **Data Integrity:** Utilized Foreign Keys and Constraints to ensure valid relationships between matches and player stats.
- **Performance Analysis:** Structure allows for complex queries, such as:
  - *Win Rate by Map Type (Control vs. Escort)*
  - *Hero Performance Metrics (Damage/10min, Healing/10min)*
  - *Role-based impact analysis*

## Tech Stack
- **Database:** SQL (MySQL / PostgreSQL)
- **Modeling:** Entity-Relationship Diagram (ERD)
- **Tools:** DataGrip / DBeaver / Workbench

## Database Structure (Schema Snapshot)
The database is built around the following core entities:

1.  **`Heroes_Table`**: Static data containing Hero Name, Role (Tank/DPS/Support), and base stats.
2.  **`Maps_Table`**: Stores Map Name and Game Mode type.
3.  **`Matches_Table`**: The central transaction table recording Match ID, Date, Result, and Map played.
4.  **`Performance_Stats`**: The granular fact table linking a specific Match to specific Hero performance (Eliminations, Deaths, Healing, etc.).

## How to Use
*(SQL files will be uploaded soon)*

1.  Clone the repository.
2.  Import the `.sql` schema file into your local SQL environment.
3.  Run the sample queries to view analytics.

---
*© 2025 Jesse Luo. This project is for educational and portfolio purposes.*
