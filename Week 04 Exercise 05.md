## Week 04

# Exercise 05

Question 01<br>
select name from country where iso_country in(<br>
select iso_country from airport where name like 'Satsuma%');<br>
![Screenshot 2024-09-25 231415](https://github.com/user-attachments/assets/d9fab33a-3bab-4693-a126-0bd215328245)

Question 02<br>
select name from airport<br>
where iso_country in(<br>
select iso_country from country<br>
where name = 'Monaco');<br>
![Screenshot 2024-09-25 231440](https://github.com/user-attachments/assets/4f0f6045-8de0-4340-a34a-951b693bd0e0)

Question 03<br>
select screen_name from game<br>
where id in (<br>
select game_id from goal_reached<br>
where goal_id in (<br>
select id from goal<br>
where name = "CLOUDS"));<br>
![Screenshot 2024-09-25 231500](https://github.com/user-attachments/assets/df48621d-2a96-4935-9770-bb5075950cb5)

Question 04<br>
select name from country<br>
where iso_country not in(<br>
select iso_country from airport);<br>
![Screenshot 2024-09-25 231516](https://github.com/user-attachments/assets/508b0c88-f5fb-4896-bdc9-ab2c543c5940)

Question 05<br>
select name from goal<br>
where id not in(<br>
select goal_id from goal_reached<br>
where game_id in (<br>
select id from game<br>
where screen_name = "Heini"));<br>
![Screenshot 2024-09-25 231534](https://github.com/user-attachments/assets/b5d7b47b-dadf-401e-8dec-55c8c8e37a49)

