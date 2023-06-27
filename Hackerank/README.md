


> Written with [StackEdit](https://stackedit.io/).

[HackerRank-SQL](https://www.hackerrank.com/domains/sql) my submissions. My account - [sanketghodke03](https://www.hackerrank.com/sanketghodke03)



### 1. [Revising the Select Query I](https://www.hackerrank.com/challenges/revising-the-select-query/problem?isFullScreen=false)

```sql 
select * from city where countrycode= 'USA' and population>100000;
```

### 2. [Revising the Select Query II](https://www.hackerrank.com/challenges/revising-the-select-query-2/problem?isFullScreen=true)

```sql 
select name from city where countrycode='USA' and population>120000;
```
### 3. [Select All](https://www.hackerrank.com/challenges/select-all-sql/problem?isFullScreen=true)

```sql 
select * from city;
```
### 4. [Select by ID](https://www.hackerrank.com/challenges/select-by-id/problem?isFullScreen=true)

```sql 
select * from city where ID=1661;
```
### 5. [Japanese Cities' Attributes](https://www.hackerrank.com/challenges/japanese-cities-attributes?isFullScreen=true)

```sql 
select * from city where COUNTRYCODE='JPN';
```

### 6. [Japanese Cities' Names](https://www.hackerrank.com/challenges/japanese-cities-name/problem?isFullScreen=true)

```sql 
select name from city where COUNTRYCODE ='JPN';
```

### 7. [Weather Observation Station 1](https://www.hackerrank.com/challenges/weather-observation-station-1/problem?isFullScreen=true)

```sql 
select city, state from STATION;
```

### 8. [Weather Observation Station 3](https://www.hackerrank.com/challenges/weather-observation-station-3/problem?isFullScreen=true)

```sql 
select distinct city from station where ID%2=0;
```

### 9. [Weather Observation Station 4](https://www.hackerrank.com/challenges/weather-observation-station-4/problem?isFullScreen=true)

```sql 
select count(city)-count(distinct city) from station;
```
### 10. [Weather Observation Station 5](https://www.hackerrank.com/challenges/weather-observation-station-5/problem?isFullScreen=true)

```sql 
select city, length(city) from STATION order by length(city) asc, city asc limit 1;
select city, length(city) from STATION order by length(city) desc, city asc limit 1;
```

### 11. [Weather Observation Station 6](https://www.hackerrank.com/challenges/weather-observation-station-6/problem?isFullScreen=true)

```sql 
METHOD 1: SELECT DISTINCT CITY FROM Station WHERE Lower(Left(CITY,1)) IN ('a','e','i','o','u');

METHOD 2: select distinct city from STATION where city REGEXP '^[aeiou]';
```
### 12. [Weather Observation Station 7](https://www.hackerrank.com/challenges/weather-observation-station-7/problem?isFullScreen=true)

```sql 
METHOD 1: SELECT DISTINCT CITY FROM Station WHERE Lower(Right(CITY,1)) IN ('a','e','i','o','u');

METHOD 2: SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP '[aeiou]$';
```

### 13. [Weather Observation Station 8](https://www.hackerrank.com/challenges/weather-observation-station-8/problem?isFullScreen=true)

```sql 
METHOD 1: select distinct city from station where left(city,1) in ('a','e','i','o','u') and right(city,1) in ('a','e','i','o','u');

METHOD 2: select distinct city from STATION where city REGEXP '^[aeiou].*[aeiou]$';
```
### 14. [Weather Observation Station 9](https://www.hackerrank.com/challenges/weather-observation-station-9/problem?isFullScreen=true)

```sql 
METHOD 1: select distinct city from station where left(city,1) not in ('a','e','i','o','u');

METHOD 2: select distinct city from STATION where city REGEXP '^[^aeiou]';
```
### 15. [Weather Observation Station 10](https://www.hackerrank.com/challenges/weather-observation-station-10/problem?isFullScreen=true)

```sql 
METHOD 1: select distinct city from station where right(city,1) not in ('a','e','i','o','u');

METHOD 2: select distinct city from STATION where city REGEXP '[^aeiou]$';
```
### 16. [Weather Observation Station 11](https://www.hackerrank.com/challenges/weather-observation-station-11/problem?isFullScreen=true)

```sql 
METHOD 1: select distinct city from station where (left(city,1) not in ('a','e','i','o','u')) or  (right(city,1) not in ('a','e','i','o','u'));

METHOD 2: select distinct city from STATION where city REGEXP '^[^aeiou]|[^aeiou]$';
```
### 17. [Weather Observation Station 12](https://www.hackerrank.com/challenges/weather-observation-station-12/problem?isFullScreen=true)

```sql 
METHOD 1: select distinct city from station where (left(city,1) not in ('a','e','i','o','u')) and  (right(city,1) not in ('a','e','i','o','u'));

METHOD 2: select distinct city from STATION where city REGEXP '^[^aeiou].*[^aeiou]$';
```

### 18. [Higher Than 75 Marks](https://www.hackerrank.com/challenges/more-than-75-marks/problem?isFullScreen=true)

```sql 
select name from students where marks>75 order by right(name,3) asc,id asc; 
```

### 19. [Employee Names](https://www.hackerrank.com/challenges/name-of-employees/problem?isFullScreen=true)

```sql 
select name from employee order by name asc;
```

### 20. [Employee Salaries](https://www.hackerrank.com/challenges/salary-of-employees/problem?isFullScreen=true)

```sql 
select name 
from employee 
where salary>2000 and months<10 
order by employee_id;
```

### 21. [Revising Aggregations - The Count Function](https://www.hackerrank.com/challenges/revising-aggregations-the-count-function/problem?isFullScreen=true)

```sql 
select count(name) from city where population>100000;
```

### 22. [Revising Aggregations - The Sum Function](https://www.hackerrank.com/challenges/revising-aggregations-sum/problem?isFullScreen=true)

```sql 
-- you can use single or double quotes 
METHOD 1:select sum(population) from city where district = "California";

METHOD 2:select sum(population) from city where district = 'California';
```

### 23. [Revising Aggregations - Averages](https://www.hackerrank.com/challenges/revising-aggregations-the-average-function/problem?isFullScreen=true)

```sql 
select avg(population) from city where district = 'California';
```

### 24. [Average Population](https://www.hackerrank.com/challenges/average-population/problem?isFullScreen=true)

```sql 
select round(avg(population)) from city;
```

### 25. [Japan Population](https://www.hackerrank.com/challenges/japan-population/problem?isFullScreen=true)

```sql 
select sum(population) from city where countrycode = 'JPN';
```

### 26. [Population Density Difference](https://www.hackerrank.com/challenges/population-density-difference/problem?isFullScreen=true)

```sql 
select max(population)-min(population) from city;
```

### 27. [The Blunder](https://www.hackerrank.com/challenges/the-blunder/problem?isFullScreen=true)

```sql 
-- Implicit conversion in SQL - geeksforgeeks.org/sql-conversion-function/ 

select ceil((avg(salary)- avg(replace(salary,'0','')))) from employees

```

### 28. [Top Earners](https://www.hackerrank.com/challenges/earnings-of-employees/problem?isFullScreen=true)

```sql 
METHOD 1:
select max(salary*months), count(name) 
from employee 
where salary*months = (
        select max(salary*months) 
        from employee
);

METHOD 2: 
SELECT salary * months AS Earnings, COUNT(*) 
FROM Employee 
GROUP BY Earnings 
ORDER BY Earnings DESC LIMIT 1;
```

### 29. [Weather Observation Station 2](https://www.hackerrank.com/challenges/weather-observation-station-2/problem?isFullScreen=true)

```sql 
select round(sum(lat_n),2), round(sum(long_w),2) 
from station;
```

### 30. [Weather Observation Station 13](https://www.hackerrank.com/challenges/weather-observation-station-13/problem?isFullScreen=true)

```sql 
select truncate(sum(lat_n),4) 
from station 
where lat_n between 38.7880 and 137.2345;
```

### 31. [Weather Observation Station 14](https://www.hackerrank.com/challenges/weather-observation-station-14/problem?isFullScreen=true)

```sql 
select truncate(max(lat_n),4) from station where lat_n<137.2345;
```

### 32. [Weather Observation Station 15](https://www.hackerrank.com/challenges/weather-observation-station-15/problem?isFullScreen=true)

```sql 
METHOD 1:
select round(long_w,4) 
from station 
where lat_n= (
    select max(lat_n) 
    from station 
    where lat_n<137.2345)
;

METHOD 2:
select round(long_w, 4)
FROM station
WHERE lat_n < 137.2345
ORDER BY lat_n DESC
LIMIT 1;
```


### 33. [Weather Observation Station 16](https://www.hackerrank.com/challenges/weather-observation-station-16/problem?isFullScreen=true)

```sql 
select round(min(lat_n),4)
from station
where lat_n>38.7780;
```

### 34. [Weather Observation Station 17](https://www.hackerrank.com/challenges/weather-observation-station-17/problem?isFullScreen=true)

```sql 
select round(long_w,4)
from station
where lat_n>38.7780
order by lat_n asc limit 1;
```

### 35. [Population Census](https://www.hackerrank.com/challenges/asian-population/problem?isFullScreen=true)

```sql 
select sum(city.population)
from city 
inner join country
on city.countrycode = country.code
where continent = 'asia';
```

### 36. [African Cities](https://www.hackerrank.com/challenges/african-cities/problem?isFullScreen=true)

```sql 
select city.name
from city
inner join country
on city.countrycode = country.code
where continent ='africa';
```

### 37. [Average Population of Each Continent](https://www.hackerrank.com/challenges/average-population-of-each-continent/problem?isFullScreen=true)

```sql 
--rounded down to nearest integer - floor function

select continent, floor(avg(city.population))
from country
inner join city
on country.code = city.countrycode
group by continent;
```

### 38. [Weather Observation Station 18](https://www.hackerrank.com/challenges/weather-observation-station-18/problem?isFullScreen=true)

```sql 
select round(abs((max(lat_n)-min(lat_n))+abs(max(long_w)-min(long_w))),4) 
from station;
```

### 39. [Weather Observation Station 19](https://www.hackerrank.com/challenges/weather-observation-station-19/problem?isFullScreen=true)

```sql 
METHOD 1:
select round(
    sqrt(
        (
            (max(lat_n)-min(lat_n))
            *
            (max(lat_n)-min(lat_n))
        )
        +(
            (max(long_w)-min(long_w))
            *
            (max(long_w)-min(long_w))
        )
    )
    ,4
) 
from station;

METHOD 2:
select round(
    sqrt(
        power(
            (max(lat_n)-min(lat_n)),2
        )
        +power(
            (max(long_w)-min(long_w)),2
        )
    )
    ,4
) 
from station;
```

### 40. [The PADS](https://www.hackerrank.com/challenges/the-pads/problem?isFullScreen=true)

```sql 
select concat(name,'(',left(occupation,1),')')
from occupations
order by name asc;

select concat('There are a total of ',count(*),' ',lower(occupation),'s.')
from occupations 
group by occupation
order by count(*),occupation;
```

### 41. [Type of Triangle](https://www.hackerrank.com/challenges/what-type-of-triangle/problem?isFullScreen=true)

```sql 
select 
    case 
        when A=B and A=C then 'Equilateral'
        when (A=B and (A+B)>C) or (B=C and (C+B)>A) or (A=C and (A+C)>B) then 'Isosceles'
        when (A+B)>C and (A+C)>B and (C+B)>A then 'Scalene'
        else 'Not A Triangle'
    end as output
from triangles;
```
