# Finals Lab Task 5:SQL Views, Functions, & Stored Procedure
> This repository demonstrates advanced SQL skills by using views, stored procedures, and stored functions in MySQL Workbench through structured tasks on a sample inventory system.
---
##  Tasks Overview
### Task 1: Create a VIEW for 2002+ product entries 🗓
-  View includes: vendors_code, vendors_name, product_description, p_indate
- ** Filter: p_indate ≥ 2002**
  
  ![image]()
---
###  Task 2: Create a VIEW for products priced  between 100–150
- ** Filters products where: p_price BETWEEN 100 AND 150**
![image])
---
###  Task 3: Create a VIEW to compute TOTAL_PRICE 
-  Calculates: P_ONHAND * P_PRICE
-  For vendors: v_code IN (21344, 23119, 24288)
![image]()
---
###  Task 4: Create a STORED PROCEDURE 🛠
-  Task: Takes 1 parameter and updates vendor name
- ✏ From Bryson, Inc. ➡️Bryson and Co
  
![image]()

### 🔹 Task 5: Create a FUNCTION with 2 parameters ⚙️
- 📌 Parameters: v_code, v_state
- 📌 Returns: product_description, price based on parameters
![image]()

---
![image]()
