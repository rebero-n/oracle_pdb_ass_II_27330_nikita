# Oracle Pluggable Database Assignment II

## Overview
This assignment demonstrates practical management of Oracle Multitenant Architecture. It covers the creation and deletion of Pluggable Databases (PDBs), user management within a PDB, and verification of the environment using Oracle Enterprise Manager (OEM) and SQL Developer. The goal is to show hands-on experience with Oracle database administration in a controlled environment.

---

## Oracle Environment
- Oracle Database 21c Express Edition (XE)  
- SQL*Plus for command-line operations  
- Oracle SQL Developer (GUI tool)  
- Oracle Enterprise Manager Database Express (OEM) via `https://localhost:5500/em`  
- Windows 11 operating system  

---

## Task Explanations

### Task 1 – Create a New Pluggable Database
- Created the main PDB `NI_PDB_27330`.  
- Created the user `NIKITA_PLSQLAUCA_27330` inside this PDB.  
- Verified the PDB was open and the user exists.  
- **Screenshot:** pdbs_creation.png 

---

### Task 2 – Create and Delete a Temporary PDB
- Created a temporary PDB `NI_TO_DELETE_PDB_27330`.  
- Verified that it existed.  
- Closed and completely dropped the temporary PDB.  
- **Screenshot:** pdbs_to_delete_deleted.png

---

### Task 3 – Oracle Enterprise Manager (OEM) and SQL Developer
- Logged in to OEM using the `SYSTEM` administrative user.  
- Selected container `NI_PDB_27330` to display the dashboard for the PDB.  
- Verified the database version, PDB name, and dashboard panels (Performance, Storage).  
- Opened SQL Developer and connected using the custom user `NIKITA_PLSQLAUCA_27330` to confirm it exists and can be used for running SQL/PLSQL commands.  
- **Screenshots:**  
  - OEM dashboard: oem_dashboard.png
  - User proof: username_proof.png  
  - SQL Developer showing the custom user: user_in_sql_dev.png  

---

## Challenges Faced
- Initial confusion with OEM login: attempted to log in using my custom user (`NIKITA_PLSQLAUCA_27330`), but Oracle XE does not allow non-administrative users to access OEM.  
- Issue resolved by logging in with `SYSTEM` as the administrative user and selecting the correct PDB container (`NI_PDB_27330`).  
- Localhost URL initially returned search results instead of the OEM page; resolved by typing the URL directly in the browser address bar (`https://localhost:5500/em`).  

---

## Integrity Statement
I confirm that this assignment was completed individually, and all screenshots and results reflect my personal Oracle database environment. No work was copied from other students or external sources.
