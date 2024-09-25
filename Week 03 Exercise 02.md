## Week 03

# Exercise 02

Chandina Nilukshi

Question 1<br/>
SELECT * FROM goal;
![Question 1](https://github.com/user-attachments/assets/8fd43c99-d226-45cd-87a0-10fece517f5f)

Question 2<br/>
SELECT name, type FROM airport WHERE iso_country = 'FI';
![Question 2](https://github.com/user-attachments/assets/2ae08adc-9673-4c00-8d84-b623ed9996f7)

Question 3<br>
SELECT name FROM airport WHERE iso_country = 'FI' ORDER BY name ASC;
![Question 3](https://github.com/user-attachments/assets/fb06d301-4cb3-4066-a229-dc9e4899cada)

Question 4<br/>
select name, type from airport where iso_country = 'FI' order by type, name;
![Question 4](https://github.com/user-attachments/assets/6ea6481d-3e00-4a7d-b94a-47b94f14cbd1)

Question 5<br/>
select name from country where name like 'F%';
![Question 5](https://github.com/user-attachments/assets/7764082d-5627-4179-98fa-032eb215374a)

Question 6<br/>
select name from country where name like "%F%";
![Question 6](https://github.com/user-attachments/assets/b7c33fa0-2c21-415b-bd1d-09af6147675c)

Question 7<br/>
select location from game where screen_name = "Vesa";
![Question 7](https://github.com/user-attachments/assets/d7849f87-8fa4-4cd5-9112-31f5a01d8953)

Question 8<br/>
select co2_consumed from game where screen_name = "Ilkka";
![Question 8](https://github.com/user-attachments/assets/9afb3092-2e66-4593-8cb6-2ffd21bab888)

Question 9<br/>
SELECT DISTINCT co2_budget FROM game;
![Question 9](https://github.com/user-attachments/assets/add76ad0-3823-4ac9-b116-2a599f3ccd0f)

Question 10<br/>
select screen_name, co2_budget, co2_consumed, co2_budget - co2_consumed as co2_left from game;
![Question 10](https://github.com/user-attachments/assets/26822764-b843-4e02-8451-fa0e167d5e70)
