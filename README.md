# World-Populations
SQL practice challenge


-- This is the first query, checks for the years covered by the database:

SELECT DISTINCT year from population_years;

-- Checks for the year with the largest population in Gabon:
SELECT population
FROM population_years
WHERE country = 'Gabon' DESC
LIMIT 1;

-- Checks for the 10 countries with largest population in 2005:
SELECT country
FROM population_years
WHERE year = 2005 ASC
LIMIT 10;

-- Finds countries with populations larger than 100M in 2010:
SELECT DISTINCT country
FROM population_years
WHERE population > 100 AND year = 2010;

-- Finds all countries that have the word "Islands" in their name:
SELECT country
FROM population_years
WHERE country LIKE '%Islands%';

-- Last two commends are used to compare population growth in Indonesia between 2000 and 2010:
SELECT population
FROM population_years
WHERE country = 'Indonesia' AND year = 2000;

SELECT population
FROM population_years
WHERE country = 'Indonesia' AND year = 2010;
