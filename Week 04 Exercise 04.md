## Week 04

# Exercise 04

Question 01 <br>
select country.name as "country name", airport.name as "airport name" <br>
from country inner join airport on country.iso_country=airport.iso_country<br>
where country.name="Finland" <br>
and airport.scheduled_service="yes";<br>
![q1](https://github.com/user-attachments/assets/948562f7-528f-42a3-833c-e82b2b136423)

Question 02<br>
select screen_name, airport.name<br>
from game inner join airport on game.location = airport.ident;<br>
![q2](https://github.com/user-attachments/assets/76a6298c-829d-455e-a7f2-76ee91f18825)

Question 03<br>
select screen_name, country.name<br>
from game inner join airport on game.location = airport.ident<br>
inner join country on country.iso_country=airport.iso_country;<br>
![q3](https://github.com/user-attachments/assets/071f22fc-b367-4ab4-babc-a3851ae2f0ec)

Question 04<br>
select airport.name, screen_name<br>
from airport left join game on airport.ident = game.location<br>
where airport.name like "%Hels%";<br>
![q4](https://github.com/user-attachments/assets/79c39c11-7319-4975-a62e-29375a9f20c3)

Question 05<br>
select name, screen_name<br>
from goal left join goal_reached on goal.id = goal_reached.goal_id<br>
left join game on goal_reached.game_id = game.id;<br>
![q5](https://github.com/user-attachments/assets/6cb5336c-a009-4c3a-9086-c35f70055d59)
