# SQL-Learning
Learning the basics of Structure Query Language, creating databases, tables, as well as navigating and searching databases.

## Learning SQL on Ubuntu

This repository documents my journey learning SQL on Ubuntu. It covers everything from creating databases to manipulating and querying data. Below are the key concepts and commands I learned.

# Learning SQL on Ubuntu

This repository documents my journey learning **<span style="color:blue">SQL</span>** on **<span style="color:green">Ubuntu</span>**. It covers everything from creating databases to manipulating and querying data. Below are the key concepts and commands I learned.

---

## 📂 <span style="color:purple">Setting Up SQL on Ubuntu</span>

1. **Update System and Install MySQL:**
   ```bash
   sudo apt update
   sudo apt install mysql-server -y
   sudo systemctl start mysql
   sudo systemctl enable mysql
   ```

2. **Access MySQL:**
   ```bash
   sudo mysql
   ```

---

## 🔢 <span style="color:purple">Creating Databases and Tables</span>

1. **Create a Database:**
   ```sql
   CREATE DATABASE <span style="color:orange">my_database</span>;
   ```

2. **Use the Database:**
   ```sql
   USE <span style="color:orange">my_database</span>;
   ```

3. **Create a Table with TRUE/FALSE (BOOLEAN) Column:**
   ```sql
   CREATE TABLE <span style="color:orange">users</span> (
       id INT AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(100),
       is_active BOOLEAN
   );
   ```

---

## 🔄 <span style="color:purple">Inserting and Updating Data</span>

1. **Insert Data into Table:**
   ```sql
   INSERT INTO <span style="color:orange">users</span> (name, is_active) VALUES ('Alice', TRUE);
   INSERT INTO <span style="color:orange">users</span> (name, is_active) VALUES ('Bob', FALSE);
   ```

2. **Update a Column:**
   ```sql
   UPDATE <span style="color:orange">users</span> SET is_active = TRUE WHERE name = 'Bob';
   ```

---

## 🔍 <span style="color:purple">Querying Data</span>

1. **Select Specific Columns:**
   ```sql
   SELECT name FROM <span style="color:orange">users</span>;
   ```

2. **Search for Specific Values:**
   ```sql
   SELECT * FROM <span style="color:orange">users</span> WHERE is_active = TRUE;
   ```

3. **Show All Databases:**
   ```sql
   SHOW DATABASES;
   ```

4. **Show All Tables in Current Database:**
   ```sql
   SHOW TABLES;
   ```

5. **Describe Table Structure:**
   ```sql
   DESCRIBE <span style="color:orange">users</span>;
   ```

---

## 🔎 <span style="color:purple">Deleting Data</span>

1. **Delete a Column from a Table:**
   ```sql
   ALTER TABLE <span style="color:orange">users</span> DROP COLUMN is_active;
   ```

2. **Delete Data from a Table:**
   ```sql
   DELETE FROM <span style="color:orange">users</span> WHERE name = 'Alice';
   ```

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

