# MySQL
create database db1;
use db1;
create table Project(id int,name varchar(255),tech varchar(255),startdate date,no_of_stud int);
insert into Project(id,name,tech,startdate,no_of_stud) values(01,"Gautami","AI","2018-02-2",5);
insert into Project(id,name,tech,startdate,no_of_stud) values(02,"Sahil","DS","2018-02-4",10);
insert into Project(id,name,tech,startdate,no_of_stud) values(03,"Navya","ML","2018-02-2",8);
insert into Project(id,name,tech,startdate,no_of_stud) values(04,"Pranav","AI","2018-02-4",15);
insert into Project(id,name,tech,startdate,no_of_stud) values(05,"Ninad","DL","2018-02-3",2);

select * from Project;

select max(no_of_stud) from Project;
select min(no_of_stud) from Project;
select count(no_of_stud) from Project;

alter table Project add guide varchar(255);

select * from Project;

update Project set guide = "abc" where id = 01;
select * from Project;
update Project set guide = "abc" where id = 02;
update Project set guide = "pqr" where id = 03;
update Project set guide = "abc" where id = 04;
update Project set guide = "lmn" where id = 05;

select * from Project;

select * from Project where guide="abc";

select name from Project order by name asc;
