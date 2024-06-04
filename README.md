# goit-rdb-hw-04 Relationship Databases Topic IV DML and DDL commands. Complex SQL expressions

1. Структура БД
   a. Назва схеми — “LibraryManagement”
   b. Таблиця "authors":

![screenshot](./assets/Screenshot%20rdb-hw-04-test-01.1.jpg)

c. Таблиця "genres":

![screenshot](./assets/Screenshot%20rdb-hw-04-test-01.2.jpg)

d. Таблиця "books":

![screenshot](./assets/Screenshot%20rdb-hw-04-test-01.3.jpg)

e. Таблиця "users":

![screenshot](./assets/Screenshot%20rdb-hw-04-test-01.4.jpg)

f. Таблиця "borrowed_books":

![screenshot](./assets/Screenshot%20rdb-hw-04-test-01.5.jpg)

2. Tables filled with test data rows:

![screenshot](./assets/Screenshot%20rdb-hw-04-test-02.1.jpg)
![screenshot](./assets/Screenshot%20rdb-hw-04-test-02.2.jpg)

![screenshot](./assets/Screenshot%20rdb-hw-04-test-02.3.jpg)
![screenshot](./assets/Screenshot%20rdb-hw-04-test-02.4.jpg)
![screenshot](./assets/Screenshot%20rdb-hw-04-test-02.5.jpg)
![screenshot](./assets/Screenshot%20rdb-hw-04-test-02.6.jpg)
![screenshot](./assets/Screenshot%20rdb-hw-04-test-02.7.jpg)

3. A query using FROM and INNER JOIN statements that joins all the data tables from the files: order_details, orders, customers, products, categories, employees, shippers, suppliers with shared keys:

![screenshot](./assets/Screenshot%20rdb-hw-04-test-03.jpeg)
![screenshot](./assets/Screenshot%20rdb-hw-04-test-03.1.jpg)
![screenshot](./assets/Screenshot%20rdb-hw-04-test-03.2.jpg)

4. Let's determine how many rows we got (using the COUNT statement):

![screenshot](./assets/Screenshot%20rdb-hw-04-test-04.1.jpg)

a. Let's change several INNER statements to LEFT or RIGHT and determine what happens to the number of rows and why:

![screenshot](./assets/Screenshot%20rdb-hw-04-test-04.2.1.jpg)
![screenshot](./assets/Screenshot%20rdb-hw-04-test-04.2.2.jpg)
![screenshot](./assets/Screenshot%20rdb-hw-04-test-04.2.3.jpg)

-- Кількість рядків змінюється тому, що INNER JOINs включають лише рядки, які мають співпадіючі значення в обох таблицях. LEFT і RIGHT JOINs, навпаки, включають всі рядки з однієї таблиці та лише співпадіючі рядки з іншої таблиці. Це може привести до збільшення кількості рядків, якщо є рядки, які не співпадають у якійсь таблиці, або зменшення, якщо є рядки, які не співпадають у обох таблицях. У нашому випадку кількість рядків залишається незмінною, 518.

b. Select only those rows where employee_id > 3 and ≤ 10:

![screenshot](./assets/Screenshot%20rdb-hw-04-test-04.3.jpg)

c. Group by category name, count number of rows in group, average product quantity (product quantity is in order_details.quantity):

![screenshot](./assets/Screenshot%20rdb-hw-04-test-04.4.jpg)

d. Filter out rows where the average number of items is greater than 21:

![screenshot](./assets/Screenshot%20rdb-hw-04-test-04.5.jpg)

e. Sort the rows in descending order of number of rows:

![screenshot](./assets/Screenshot%20rdb-hw-04-test-04.6.jpg)

f. Display (select) four lines with the first line omitted:

![screenshot](./assets/Screenshot%20rdb-hw-04-test-04.7.jpg)
