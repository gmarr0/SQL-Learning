# SQL-Learning
Learning the basics of Structure Query Language, creating databases, tables, as well as navigating and searching databases.

## Learning SQL on Ubuntu

This repository documents my journey learning SQL on an Ubuntu Virtual machine. It covers everything from creating databases to manipulating and querying data. Below are the key concepts and commands I learned.

---

## Setting Up SQL on Ubuntu

1. **Update System and Install MySQL:**
   ```bash
   ubuntu@ubuntu:~$ sudo apt update
   ubuntu@ubuntu:~$ sudo apt install mysql-server -y
   ```

---

2. **Access MySQL:**
   ```bash
   ubuntu@ubuntu:~$ sudo mysql
   ```
![opening mysql requires root access](https://github.com/user-attachments/assets/477b935b-a91b-47c5-8345-b9c7b6dff6c9)

---

## Creating Databases and Tables

1. **Create a Database:**
   ```sql
   mysql> create database; 
   ```
   -In SQL a ";" is always needed at the end of the command to let it know your finished with your request.
   
   -When you enter a successful query you should get a message saying "Query OK, 1 row affected (0.01 sec)"
   
![creating   showing databases](https://github.com/user-attachments/assets/ba67f207-6cdd-4da0-bbb2-c63e77f15237)

---

2. **Use the Database:**
   ```sql
   mysql> use; 
   ```
   -If successful should say : "Database Changed"

![creating first mysql table 2](https://github.com/user-attachments/assets/22fa53a2-2cae-4f9a-8c67-34738a8031ed)

---

3. **Altering a table to add a TRUE/FALSE (BOOLEAN) Column:**
   ```sql
   mysql> alter table yourtable_name add newcolumn_name boolean;  
   ```
-use "alter" to alter the table and "add" to a new column and "boolean" for true or false 

![BOOLEAN](https://github.com/user-attachments/assets/fc24e0bc-3e00-4246-add4-91135250f3c1)

-use "update" to update a column and "where" to specify which column your updating.

![adding TRUE and FALSE stayments to multiple columns at once](https://github.com/user-attachments/assets/e36af45d-217b-4da8-9c6b-dc98b908565b)

---

## 🔄 Inserting and Updating Data

1. **Insert Data into Table:**
   ```sql
   mysql> insert into yourtable_name values (1, "default route", "location", "item");
   ```

![inserting data into our table](https://github.com/user-attachments/assets/b4412f65-cf16-4f9e-bb78-bc7ad01ba337)

![adding multiple lines columns at once inside our table](https://github.com/user-attachments/assets/9eff248d-26b7-4da9-8c09-80097576389b)


-  **The " , " is to let sql know we're not done with our columns yet letting us add multiple lines at once**
---

2. **Update a Column:**
   ```sql
   mysql> update yourtable_name set id = 5 where id = 6;
   ```

![update a column](https://github.com/user-attachments/assets/7112fae7-49f9-44c1-b2cb-659b6ee5562f)

---

## 🔍 Querying Data

1. **Select Specific Columns:**
   ```sql
   mysql> select column_name from table_name;
   ```

- select = we want to select data  
   
![specifying a specific category inside our database](https://github.com/user-attachments/assets/4b20401e-eb35-44a2-ad82-195103399c1e)
```sql
mysql select * from yourtable_name where column =  "the column name" or column = "the column name";
```

- can use "or" when querying specific data to specifically search for multiple types of data

![specifiying columns in data base with WHERE and choosing between two with OR](https://github.com/user-attachments/assets/a1bdc4c3-ac97-4813-af18-63b32caa606a)

![selecting everything from a table using asterisk](https://github.com/user-attachments/assets/91a2c089-24bc-478f-b1b9-f4ea33dfe952)

- using an Asterisk (*) asks to output all the contents inside.
  
2. **Search for Specific Values:**
   ```sql
   SELECT * FROM <span style="color:orange">users</span> WHERE is_active = TRUE;
   ```

```sql
mysql> select device from jparo_gadgets where price < 500;
```

![searching for gadgets below 500 dollars with the LESS THAN symbol](https://github.com/user-attachments/assets/8a2c7551-f259-4ad4-b7f0-5ad56a9a9fdb)

- you can use " < " less than or " > " more than to deep dive even further to specify data with numbers or values
3. **Show All Databases:**
   ```sql
   mysql> show databases;
   ```
![showing data bases](https://github.com/user-attachments/assets/5f25a083-b9c3-4bd1-8388-7499d86c7d9e)

4. **Show All Tables in Current Database:**
   ```sql
   SHOW TABLES;
   ```

5. **Describe Table Structure:**
   ```sql
   mysql> describe table_name;
   ```
![describing table to see contents inside](https://github.com/user-attachments/assets/85aed634-3cfd-4751-8230-e51c11cfe2de)

---

## 🔎 <span style="color:purple">Deleting Data</span>

1. **Delete a Column from a Table:**
   ```sql
   ALTER TABLE <span style="color:orange">users</span> DROP COLUMN is_active;
   ```

2. **Delete Data from a Table:**
   ```sql
   mysql> delete from yourtable_name where column =  "column item";
   ```
![deleting columns from database](https://github.com/user-attachments/assets/23d94232-5c8d-4823-b8d6-221fe2a42251)

- To delete items from tables
3. **Drop a Table:**
   ```sql
   DROP TABLE <span style="color:orange">users</span>;
   ```

4. **Drop a Database:**
   ```sql
   DROP DATABASE <span style="color:orange">my_database</span>;
   ```

---

## 🌟 <span style="color:purple">Conclusion</span>

Learning **<span style="color:blue">SQL</span>** on **<span style="color:green">Ubuntu</span>** has been an essential step in building my IT skills. This repository serves as a reference for basic **<span style="color:blue">SQL</span>** operations and will be updated as I continue to learn more advanced **<span style="color:blue">SQL</span>** concepts.

Feel free to explore the commands and modify them to fit your own projects!

