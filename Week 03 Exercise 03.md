## Week 03

# Exercise 03

Question 01<br>
SELECT country.name as "country name", airport.name as "airport name"<br>
FROM country, airport<br>
WHERE country.iso_country = airport.iso_country and country.name = "Iceland";<br>
![Screenshot 2024-09-25 224602](https://github.com/user-attachments/assets/c208aba1-af49-4009-919a-fde6ee750076)

Question 02<br>
SELECT airport.name as "airport name"<br>
FROM airport, country<br>
where airport.iso_country=country.iso_country and country.name = "France" AND airport.type = "large_airport";<br>
![Screenshot 2024-09-25 224644](https://github.com/user-attachments/assets/6b0df97d-1caa-4d37-ae6b-cf245d08a2c0)

Question 03<br>
select country.name as "country_name", airport.name as "airport_name"<br>
from airport, country<br>
where airport.iso_country = country.iso_country and country.continent = "AN";<br>
![Screenshot 2024-09-25 224701](https://github.com/user-attachments/assets/64253995-2a6a-4c90-b274-caf1589bde79)

Question 04<br>
SELECT elevation_ft<br>
from airport, game<br>
where location = ident and screen_name="Heini";<br>
![Screenshot 2024-09-25 224817](https://github.com/user-attachments/assets/fec0896b-cfe5-40d0-9b23-10bb68055482)

Questoin 05<br>
select elevation_ft * 0.3048 as "elevation_m"<br>
from airport, game<br>
where location = ident and screen_name="Heini";<br>
![Screenshot 2024-09-25 224837](https://github.com/user-attachments/assets/7f7afe5c-8731-4d7c-8c9c-4b03b4ab1d0c)

Question 06<br>
select airport.name as "name"<br>
from airport, game<br>
where location = ident and screen_name = "Ilkka";<br>
![Screenshot 2024-09-25 224855](https://github.com/user-attachments/assets/db272b92-14cb-455a-894b-38f6ecf588bd)

Question 07<br>
select country.name as "name"<br>
from country, airport, game<br>
where location = ident and airport.iso_country = country.iso_country and screen_name = "Ilkka";<br>
![Screenshot 2024-09-25 224924](https://github.com/user-attachments/assets/6471f1db-a42c-4e35-a36e-911a964f5be6)

Question 08<br>
select name from goal, game, goal_reached where game.id=game_id and goal.id=goal_id and screen_name="Heini";<br>
![Screenshot 2024-09-25 225005](https://github.com/user-attachments/assets/d325953c-9f8b-421e-879b-28f2d1c37221)

Question 09<br>
select airport.name from airport, goal_reached, goal, game<br>
where ident = location and goal.id = goal_reached.goal_id and game.id = goal_reached.game_id and screen_name = "Ilkka" and goal.name = "CLOUDS";<br>
![Screenshot 2024-09-25 225042](https://github.com/user-attachments/assets/2ea4cfc1-cad5-4ce1-bd7e-75d20495f27a)

Question 10<br>
select country.name<br>
from country, game, goal, goal_reached, airport<br>
where airport.iso_country = country.iso_country and ident=location AND<br> game_id=game.id AND goal_id=goal.id and screen_name = "Ilkka" and goal.name = "CLOUDS";<br>
![Screenshot 2024-09-25 225103](https://github.com/user-attachments/assets/37efefa2-454a-4522-9325-c93700e2cb61)
