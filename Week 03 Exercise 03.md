## Week 03

# Exercise 03

Question 01<br>
SELECT country.name as "country name", airport.name as "airport name"<br>
FROM country, airport<br>
WHERE country.iso_country = airport.iso_country and country.name = "Iceland";<br>
