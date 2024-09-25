## Week 03

# Exercise 02

Chandina Nilukshi

Question 1<br/>
SELECT * FROM goal;
![Question 1](https://github.com/user-attachments/assets/f96fef8c-8833-4d13-a87c-96aa4e70ede9)


Question 2<br/>
SELECT name, type FROM airport WHERE iso_country = 'FI';
![Question 2](https://github.com/user-attachments/assets/bd9a3cc0-e63b-4331-980b-66a21e08cd19)


Question 3<br>
SELECT name FROM airport WHERE iso_country = 'FI' ORDER BY name ASC;
![Question 3](https://github.com/user-attachments/assets/cc640cf1-fa2b-4f23-bcbd-3bd98e796da3)


Question 4<br/>
select name, type from airport where iso_country = 'FI' order by type, name;
![Question 4](https://github.com/user-attachments/assets/d6ded1d3-bd22-4535-abda-6383d7c58db2)


Question 5<br/>
select name from country where name like 'F%';
![Question 5](https://github.com/user-attachments/assets/311c7289-b8fa-40d7-b30f-c4a21f7679e0)


Question 6<br/>
select name from country where name like "%F%";
![Question 6](https://github.com/user-attachments/assets/af2480e1-5970-4a1f-ba9d-68970c168af2)


Question 7<br/>
select location from game where screen_name = "Vesa";
![Question 7](https://github.com/user-attachments/assets/c9b51ab6-a0cd-4e2d-8f28-0116d0b4a193)


Question 8<br/>
select co2_consumed from game where screen_name = "Ilkka";
![Question 8](https://github.com/user-attachments/assets/1b6fb2c2-1a69-472d-9a50-e50862f831ad)


Question 9<br/>
SELECT DISTINCT co2_budget FROM game;
![Question 9](https://github.com/user-attachments/assets/c0a7d7b6-6e0c-4fed-aa4a-0c3853d44bf0)


Question 10<br/>
select screen_name, co2_budget, co2_consumed, co2_budget - co2_consumed as co2_left from game;
![Question 10](https://github.com/user-attachments/assets/de445a10-b049-4a27-98d3-0624fef945b5)

