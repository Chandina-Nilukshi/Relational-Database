## Week 04

# Exercise 04

Question 01
select country.name as "country name", airport.name as "airport name" <br>
from country inner join airport on country.iso_country=airport.iso_country<br>
where country.name="Finland" <br>
and airport.scheduled_service="yes";<br>
