## Week 03

# Exercise 02

Chandina Nilukshi

Question 1<br/>
SELECT * FROM goal;
![q1](https://github.com/user-attachments/assets/a2c375ec-0e67-4b56-9181-17c83e75bddc)

Question 2<br/>
SELECT name, type FROM airport WHERE iso_country = 'FI';
![q2](https://github.com/user-attachments/assets/0b4ae2df-6f1b-446b-834b-ea9824478bc1)

Question 3<br>
SELECT name FROM airport WHERE iso_country = 'FI' ORDER BY name ASC;
![q3](https://github.com/user-attachments/assets/0c61c801-6c37-4e88-9b3e-29d87b2c07aa)

Question 4<br/>
select name, type from airport where iso_country = 'FI' order by type, name;
![q4](https://github.com/user-attachments/assets/602f0456-dcca-4d0d-8b18-bc30f2123edd)

Question 5<br/>
select name from country where name like 'F%';
![q5](https://github.com/user-attachments/assets/250665f6-bd3e-4da7-9c9a-06c2d8431d9e)

Question 6<br/>
select name from country where name like "%F%";
![q6](https://github.com/user-attachments/assets/7914324a-cd94-472f-abeb-65e168564b5f)

Question 7<br/>
select location from game where screen_name = "Vesa";
![q7](https://github.com/user-attachments/assets/e8044bdb-ed12-439e-8a3c-c7d66edbb8cd)

Question 8<br/>
select co2_consumed from game where screen_name = "Ilkka";
![q8](https://github.com/user-attachments/assets/799480c3-db37-4a73-86d4-760e3dd56d80)

Question 9<br/>
SELECT DISTINCT co2_budget FROM game;
![q9](https://github.com/user-attachments/assets/b1a1ffa2-54d7-4746-805d-bef0b524ea97)

Question 10<br/>
select screen_name, co2_budget, co2_consumed, co2_budget - co2_consumed as co2_left from game;
![q10](https://github.com/user-attachments/assets/f16d37f5-5cc0-4660-bd53-fdee1671f465)
