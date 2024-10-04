## Week 04

# Exercise 05

Question 01<br>
select name from country where iso_country in(<br>
select iso_country from airport where name like 'Satsuma%');<br>
![q1](https://github.com/user-attachments/assets/7602883b-9ff1-4e9e-8125-c4868613bbf2)

Question 02<br>
select name from airport<br>
where iso_country in(<br>
select iso_country from country<br>
where name = 'Monaco');<br>
![q2](https://github.com/user-attachments/assets/7b119c3c-674a-475e-8267-312d0014d891)

Question 03<br>
select screen_name from game<br>
where id in (<br>
select game_id from goal_reached<br>
where goal_id in (<br>
select id from goal<br>
where name = "CLOUDS"));<br>
![q3](https://github.com/user-attachments/assets/61dbbfee-6eab-4793-b64f-b4a9cb569f49)

Question 04<br>
select name from country<br>
where iso_country not in(<br>
select iso_country from airport);<br>
![q4](https://github.com/user-attachments/assets/b1228ad5-1e70-4eb1-ad2c-7a5065763b2d)

Question 05<br>
select name from goal<br>
where id not in(<br>
select goal_id from goal_reached<br>
where game_id in (<br>
select id from game<br>
where screen_name = "Heini"));<br>
![q5](https://github.com/user-attachments/assets/1693e980-71c8-4c61-8538-077186aa99d6)
