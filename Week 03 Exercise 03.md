## Week 03

# Exercise 03

Question 01<br>
SELECT country.name as "country name", airport.name as "airport name"<br>
FROM country, airport<br>
WHERE country.iso_country = airport.iso_country and country.name = "Iceland";<br>
![q1](https://github.com/user-attachments/assets/7801101c-eb44-4d70-9b59-edeac40ec405)

Question 02<br>
SELECT airport.name as "airport name"<br>
FROM airport, country<br>
where airport.iso_country=country.iso_country and country.name = "France" AND airport.type = "large_airport";<br>
![q2](https://github.com/user-attachments/assets/1eb9e3f6-b9cb-405f-af3c-660ae622e4b6)

Question 03<br>
select country.name as "country_name", airport.name as "airport_name"<br>
from airport, country<br>
where airport.iso_country = country.iso_country and country.continent = "AN";<br>
![q3](https://github.com/user-attachments/assets/c3e82da0-ad66-4196-81bd-8b89109e5967)

Question 04<br>
SELECT elevation_ft<br>
from airport, game<br>
where location = ident and screen_name="Heini";<br>
![q4](https://github.com/user-attachments/assets/ad80fefc-7563-432f-8c16-c32fe742a05c)

Questoin 05<br>
select elevation_ft * 0.3048 as "elevation_m"<br>
from airport, game<br>
where location = ident and screen_name="Heini";<br>
![q5](https://github.com/user-attachments/assets/3eadea45-7e1b-4dc2-bfa7-c9e0e78dbbb0)

Question 06<br>
select airport.name as "name"<br>
from airport, game<br>
where location = ident and screen_name = "Ilkka";<br>
![q6](https://github.com/user-attachments/assets/ee1224a0-60cb-4132-acab-251d4b58bbba)

Question 07<br>
select country.name as "name"<br>
from country, airport, game<br>
where location = ident and airport.iso_country = country.iso_country and screen_name = "Ilkka";<br>
![q7](https://github.com/user-attachments/assets/55889b09-90a9-4ba2-8cb0-e95af4b05339)

Question 08<br>
select name from goal, game, goal_reached where game.id=game_id and goal.id=goal_id and screen_name="Heini";<br>
![q8](https://github.com/user-attachments/assets/5b289a4c-91f5-47b1-9edc-d8b8c67f67e7)


Question 09<br>
select airport.name from airport, goal_reached, goal, game<br>
where ident = location and goal.id = goal_reached.goal_id and game.id = goal_reached.game_id and screen_name = "Ilkka" and goal.name = "CLOUDS";<br>
![q9](https://github.com/user-attachments/assets/4bdde0f7-410c-4e0e-998a-b2ea8b3e89af)

Question 10<br>
select country.name<br>
from country, game, goal, goal_reached, airport<br>
where airport.iso_country = country.iso_country and ident=location AND<br> game_id=game.id AND goal_id=goal.id and screen_name = "Ilkka" and goal.name = "CLOUDS";<br>
![q10](https://github.com/user-attachments/assets/701d4721-c514-4bf1-9cdd-6dcc2ac41393)
