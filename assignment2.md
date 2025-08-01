Mysql 
DDL
1.	create database hotwax;
2.	use hotwax;
3.	create table employee (id int ,name varchar(20));
4.	alter table employee modify  id int   primary key auto_increment;
5.	insert into employee (name)values ("ankit"),("rahul");
6.	alter table employee rename to staff;
7.	alter table staff add column gender varchar(20) after name; 
8.	alter table staff drop column id ;
9.	create table students (id int primary key,name varchar(50),marks varchar(50));
10.	alter table students add column pid int;
11.	alter table students rename column pid to Pid;
12.	ALTER TABLE staff ADD FOREIGN KEY (id) REFERENCES students(id);
13.	alter table staff add column email varchar(50) unique;
14.	alter table staff add column  mode varchar(50) default"active";
15.	truncate students;
16.	alter table students drop column name;
17.	alter table students rename to std;
18.	select * from staff;
19.	truncate table staff;
20.	drop table std;

 




DML
1.	show tables;
2.	select * from staff;
3.	select * from staff order by name asc;
4.	select * from staff limit 2;
5.	select * from staff top ;
6.	select * from staff fetchfirst ;

7.	insert into staff values (4,"amit","amit@gmail.com","active"),(2,"aniket","anikit@gmail.com","not active"),(6,"anki","anki@gmail.com","active");
8.	delete from staff where name = 4;
9.	insert into staff values (1, 'ravi', 'ravi@gmail.com', 'active');
10.	insert into staff values (4, 'amit', 'amit@gmail.com', 'inactive');
11.	insert into staff values 
12.	(5, 'anu', 'anu@gmail.com', 'active'), 
13.	(6, 'raj', 'raj@gmail.com', 'not active');
14.	update staff set status = 'inactive' where id = 2;
15.	update staff set name = 'ankit sharma' where id = 3;
16.	delete from staff where id > 4;
17.	select * from staff;
18.	select name, email from staff;
19.	select * from staff where status = 'active';
20.	select * from staff order by name asc;
21.	select * from staff where email like '%gmail.com';

git hub 
cherry picking 
cherry picking is used in GitHub to solve the merge conflict 
when two or more people work on same issue or file and they make changes in it then this arises the conflict to the code base and owner needs to select the changes he wants to keep in file using cherry picking 
syntax
git cherry-pick <commit-hash>

example
 git checkout main
git cherry-pick a1b2c3d4
