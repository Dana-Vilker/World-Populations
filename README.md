# World-Populations
SQL practice challenge


-- This is the first query:

SELECT DISTINCT year from population_years;

-- Add your additional queries below:
SELECT population
FROM population_years
WHERE country = 'Gabon' DESC
LIMIT 1;

SELECT country
FROM population_years
WHERE year = 2005 ASC
LIMIT 10;

SELECT DISTINCT country
FROM population_years
WHERE population > 100 AND year = 2010;

SELECT country
FROM population_years
WHERE country LIKE '%Islands%';

SELECT population
FROM population_years
WHERE country = 'Indonesia' AND year = 2000;

SELECT population
FROM population_years
WHERE country = 'Indonesia' AND year = 2010;
