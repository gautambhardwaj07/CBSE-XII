## Commands
**1. SELECT →** This command is used to print column, values from specified table.
<br>
<br>

**2. FROM →** It will extract values from column from specified table.
<br>
<br>

**3. WHERE →** This command is used to give condition in a query.
<br>
<br>

**4. ORDER BY →** This command is used to arrange the table in ascending or descending order on the basis of a prticular column.

(i) `SELECT NAME FROM TUITION WHERE PERCENT > 40 ORDER BY NAME;`

This command will print student's name from the table 'TUITION' whose percentage is more than 40 in alphabetically order.

(ii) `SELECT NAME FROM TUITION WHERE PERCENT > 40 ORDER BY NAME DESC;`

This command will print student's name from the table 'TUITION' whose percentage is more than 40 in reverse alphabetically order.
<br>
<br>

**5. GROUP BY →** This command will make groups of different types of same element.

e.g., `SELECT SUM(AMOUNT), COMPANY FROM SHOWROOM GROUP BY COMPANY;`
<br>
<br>

**6. DISTINCT →** This command will not consider any repeated value from same column.

e.g., `SELECT DISTINCT GAME FROM SCHOOL;`
<br>
<br>

**7. LIKE →** This command is used to compare a string with sub string.

(i) "%" → This is known as unlimited. In this, there is no boundation for number of characters.

e.g., `SELECT NAME FROM CLASS WHERE NAME LIKE "A%";`

(ii) "_" → In this, there is boundation for number of characters.

e.g., `SELECT NAME FROM CLASS WHERE NAME LIKE "A_ _ _ _ _";`
<br>
<br>

**8. INSERT INTO →** This command is used to add a new record(row) in any existing table. It is used with 'VALUES' command.

e.g., `INSERT INTO TUITION VALUES();`
<br>
<br>

**9. UPDATE →** This command is used to change value of the particular column of a table. It is used with set command.

e.g., `UPDATE FLIGHT SET FARE=6000 WHERE ENO="F104";`
<br>
<br>

**10. DELETE →** This command is used to delete record(s) from a table.

e.g., `DELETE FROM FLIGHT WHERE END="MUMBAI";`
<br>
<br>
<br>

## Functions
**1. MAX() →** It will find maximum value of a column.
<br>
<br>

**2. MIN() →** It will find minimum value of a column.
<br>
<br>

**3. SUM() →** It will add values of a column.
<br>
<br>

**4. AVE() →** It will find average of a column.
<br>
<br>

**5. COUNT(COLUMN_NAME) →** It will count total number of rows of a particular column, but only used rows.
<br>
<br>

**6. COUNT(*) →** It will count total number of rows of a particular table.
<br>
<br>
<br>

## Note
**1. '*' →** It is known as all.

When we have to extract all column values, then we use this symbol.

e.g., `SELECT * FROM TUITION WHERE AGE>15;`
<br>
<br>

**2. IS →** It is used to check if column is NULL.
