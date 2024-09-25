## Week 04

# Exercise 04

Question 01 <br>
select country.name as "country name", airport.name as "airport name" <br>
from country inner join airport on country.iso_country=airport.iso_country<br>
where country.name="Finland" <br>
and airport.scheduled_service="yes";<br>
![Question 1](https://github.com/user-attachments/assets/d5fcfcd6-a275-4032-ae60-e7ca99361fb4)

Question 02<br>
select screen_name, airport.name<br>
from game inner join airport on game.location = airport.ident;<br>
![Question 2](https://github.com/user-attachments/assets/a51db2c8-f9f2-4f94-b6bb-4dd56d964c1b)

Question 03<br>
select screen_name, country.name<br>
from game inner join airport on game.location = airport.ident<br>
inner join country on country.iso_country=airport.iso_country;<br>
![Question 3](https://github.com/user-attachments/assets/f5dab7db-5255-4e3f-b805-70508e303e50)

Question 04<br>
select airport.name, screen_name<br>
from airport left join game on airport.ident = game.location<br>
where airport.name like "%Hels%";<br>
![Question 4](https://github.com/user-attachments/assets/506c159c-dc10-4457-8434-bafd9762011e)

Question 05<br>
select name, screen_name<br>
from goal left join goal_reached on goal.id = goal_reached.goal_id<br>
left join game on goal_reached.game_id = game.id;<br>
![Question 5](https://github.com/user-attachments/assets/3b1f35b6-d62f-455b-8119-d964cc7e0aa9)
