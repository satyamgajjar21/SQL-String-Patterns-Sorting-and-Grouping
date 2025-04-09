## **Hands-on Lab: String Patterns, Sorting and Grouping**

**Estimated time needed**: 35 minutes

In this lab, you will go through some **SQL practice problems** that provide hands-on experience with **string patterns, sorting result sets, and grouping result sets**.

---

## **Software Used in this Lab**

You will use an **IBM Db2 Database**.  
Db2 is a **Relational Database Management System (RDBMS)** from IBM, designed to store, analyze, and retrieve data efficiently.

To complete this lab, you will utilize a **Db2 database service on IBM Cloud**.

> ⚠️ If you haven’t yet completed the earlier lab to set up the Db2 service, please do that first:  
**Hands-on Lab: Sign up for IBM Cloud, Create Db2 service instance and Get started with the Db2 console**

---

## **Database Used in this Lab**

This lab uses a sample **HR database** consisting of five tables:

- **EMPLOYEES**
- **JOB_HISTORY**
- **JOBS**
- **DEPARTMENTS**
- **LOCATIONS**

> ⚠️ These tables must be populated with sample data. If not already done, please complete the lab:  
**Hands-on Lab: Create tables using SQL scripts and Load data into tables**

---

## **Objectives**

After completing this lab, you will be able to:

- Simplify a **SELECT** statement using **string patterns**, **ranges**, or **sets of values**
- **Sort** result sets in ascending/descending order and specify sort columns
- **Eliminate duplicates** and apply additional filters to result sets

> 💡 Make sure you are using the **CSV file and datasets** from the instruction file.

---

## **Instructions**

1. Go to the **Resource List** on IBM Cloud and locate your **Db2 service instance**.
2. Click **Open Console**.
3. Click the 3-bar menu icon (☰) and navigate to **Run SQL**.
4. Use the **Run SQL** tool to execute queries.

> If needed, refer to the lab:  
**Hands-on Lab: Sign up for IBM Cloud, Create Db2 service instance and Get started with the Db2 console**

---

## **Exercise 1: String Patterns**

### **1. Retrieve all employees whose address is in Elgin, IL**

**Solution:**
```sql
SELECT F_NAME, L_NAME
FROM EMPLOYEES
WHERE ADDRESS LIKE '%Elgin,IL%';
