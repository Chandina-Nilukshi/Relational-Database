## Week 05

### Chandina Nilukshi

Question 01<br>
select max(elevation_ft) as "max(elevation_ft)" from airport;
![1](https://github.com/user-attachments/assets/f71719a3-222d-4dcc-8c83-c3d14bff4a82)

Question 02<br>
select continent, count(*) <br>
from country <br>
group by continent;<br>
![2](https://github.com/user-attachments/assets/24fe8e58-47f8-42c5-97e7-d47377f0ff8c)

Question 03<br>
select game.screen_name, count(*) <br>
from game, goal_reached where game.id = goal_reached.game_id <br>
group by screen_name;<br>
![3](https://github.com/user-attachments/assets/db1ccea0-3bd1-4041-905d-2f1af6e7155a)

Question 04<br>
select screen_name from game<br>
where co2_consumed in (<br>
select min(co2_consumed) from game);<br>
![4](https://github.com/user-attachments/assets/252745b8-09a3-40d4-aeaf-4a679ce5c740)

Question 05<br>
select country.name, count(*) from country<br>
join airport on airport.iso_country = country.iso_country<br>
group by country.iso_country order by count(*) desc limit 50;<br>
![5](https://github.com/user-attachments/assets/3f96fe1c-74ff-4fe9-8964-4ea61fa73514)

Question 06<br>
select country.name<br>
from country, airport<br>
where airport.iso_country = country.iso_country<br>
group by country.iso_country<br>
having count(*) >= 1000;<br>
![6](https://github.com/user-attachments/assets/80d44a44-be38-4e1a-9794-d0aa064f1c21)

Question 07<br>
select name from airport<br>
where elevation_ft in (<br>
select max(elevation_ft) from airport);<br>
![7](https://github.com/user-attachments/assets/a860e292-12ea-406d-928f-68b5178abb84)

Quwation 08<br>
select country.name from country, airport<br>
where airport.iso_country = country.iso_country and elevation_ft in (<br>
select max(elevation_ft) from airport);<br>
![8](https://github.com/user-attachments/assets/e1d841ed-66fe-4d3a-a147-939a23c1be89)

Question 09<br>
select count(*) from game, goal_reached <br>
where game.id = goal_reached.game_id <br>
and screen_name = "Vesa" group by game_id;<br>
![9](https://github.com/user-attachments/assets/e3774600-5691-4a52-bcc2-152b1987ddad)

Question 10<br>
select name from airport<br>
where latitude_deg in(<br>
select min(latitude_deg) from airport);<br>
![10](https://github.com/user-attachments/assets/99c016c7-fe1b-4f2d-a229-33bb5fe78fba)
