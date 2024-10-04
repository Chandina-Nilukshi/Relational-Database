## Week 05

### Chandina Nilukshi

Question 01<br>
select max(elevation_ft) as "max(elevation_ft)" from airport;
![q1](https://github.com/user-attachments/assets/3bc5c1c6-18b5-4b2e-b381-db675f9558f5)

Question 02<br>
select continent, count(*) <br>
from country <br>
group by continent;<br>
![q2](https://github.com/user-attachments/assets/78eba26e-f774-4b41-948e-09d48a24e94b)

Question 03<br>
select game.screen_name, count(*) <br>
from game, goal_reached where game.id = goal_reached.game_id <br>
group by screen_name;<br>
![q3](https://github.com/user-attachments/assets/8fcc4b48-0506-48ad-b826-c050a8fa9118)

Question 04<br>
select screen_name from game<br>
where co2_consumed in (<br>
select min(co2_consumed) from game);<br>
![q4](https://github.com/user-attachments/assets/4f69b743-c6dc-45c8-8d7c-e63324b3cfb9)

Question 05<br>
select country.name, count(*) from country<br>
join airport on airport.iso_country = country.iso_country<br>
group by country.iso_country order by count(*) desc limit 50;<br>
![q5](https://github.com/user-attachments/assets/c9fb2a78-4073-426a-9e78-9d173fde3ca8)

Question 06<br>
select country.name<br>
from country, airport<br>
where airport.iso_country = country.iso_country<br>
group by country.iso_country<br>
having count(*) >= 1000;<br>
![q6](https://github.com/user-attachments/assets/083fd594-b203-47c1-920f-3c4505531f6f)

Question 07<br>
select name from airport<br>
where elevation_ft in (<br>
select max(elevation_ft) from airport);<br>
![q7](https://github.com/user-attachments/assets/40ca1fe4-4f92-4ea9-ae07-6273ec9264cc)

Quwation 08<br>
select country.name from country, airport<br>
where airport.iso_country = country.iso_country and elevation_ft in (<br>
select max(elevation_ft) from airport);<br>
![q8](https://github.com/user-attachments/assets/29ee6ed6-9047-41f7-9715-207281cc72cd)

Question 09<br>
select count(*) from game, goal_reached <br>
where game.id = goal_reached.game_id <br>
and screen_name = "Vesa" group by game_id;<br>
![q9](https://github.com/user-attachments/assets/d7ece94f-df4f-4893-95c7-0690b1b53064)

Question 10<br>
select name from airport<br>
where latitude_deg in(<br>
select min(latitude_deg) from airport);<br>
![q10](https://github.com/user-attachments/assets/72e77293-ed11-4080-aa31-b186e56bec6d)
