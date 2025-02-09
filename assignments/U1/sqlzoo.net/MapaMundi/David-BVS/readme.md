# ELEBORADO POR VALENZUELA SOTO DAVID BERNABE 
# 23210677

#PROBLEMA 1:
```sql
SELECT name, continent, population FROM world
```
#PROBLEMA 2:
```sql
SELECT name FROM world
WHERE population >= 200000000;
```
#PROBLEMA 3:
```sql
SELECT name, gdp/population AS per_capita_gdp 
FROM world
WHERE population >= 200000000;
```
#PROBLEMA 4:
```sql
SELECT name, population / 1000000 AS population_in_millions
FROM world
WHERE continent = 'South America';
```
#PROBLEMA 5:
```sql
SELECT name, population 
FROM world
WHERE name IN ('France', 'Germany', 'Italy');
```
#PROBLEMA 6:
```sql
SELECT name 
FROM world
WHERE name LIKE '%United%';
```
#PROBLEMA 7:
```sql
SELECT name, population, area 
FROM world
WHERE area > 3000000 OR population > 250000000;
```
#PROBLEMA 8:
```sql
SELECT name, population, area 
FROM world
WHERE (area > 3000000 XOR population > 250000000);
```
#PROBLEMA 9:
```sql
SELECT name, 
       ROUND(population / 1000000, 2) AS population_in_millions, 
       ROUND(gdp / 1000000000, 2) AS gdp_in_billions
FROM world
WHERE continent = 'South America';
```
#PROBLEMA 10:
```sql
SELECT name, 
       ROUND(gdp / population, -3) AS per_capita_gdp
FROM world
WHERE gdp >= 1000000000000;
```
#PROBLEMA 11:
```sql
SELECT name, capital 
FROM world
WHERE LENGTH(name) = LENGTH(capital);
```
#PROBLEMA 12:
```sql
SELECT name, capital
FROM world
WHERE LEFT(name, 1) = LEFT(capital, 1)
AND name <> capital;
```
#PROBLEMA 13:
```sql
SELECT name
FROM world
WHERE name LIKE '%a%'
AND name LIKE '%e%'
AND name LIKE '%i%'
AND name LIKE '%o%'
AND name LIKE '%u%'
AND name NOT LIKE '% %';
```
