To install:
-----------

1.> git clone https://github.com/grkrthk/SQLITE3_PROJECT_CS411

2.> cd SQLITE3_PROJECT_CS411

3.> ./configure

4.> make

5.> ./sqlite3


OUTPUT SNIPPET:
--------------

sqlite> create table employee (age char);

sqlite> alter table employee add constraint constr1 check (age>30);

Warning: This will have no effect on the existing tuples

sqlite> insert into employee (age) values (70);

sqlite> insert into employee (age) values (28);

Error: constraint constr1 failed

sqlite> select * from employee;
70

