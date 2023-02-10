#1
Query all columns for all American cities in the CITY table with populations larger than 100000. The CountryCode for America is USA.

```sql
SELECT
    *
FROM 
    CITY AS c
WHERE
    c.POPULATION > 100000 AND c. COUNTRYCODE = 'USA'

```
#2
Query the NAME field for all American cities in the CITY table with populations larger than 120000. The CountryCode for America is USA.

```sql
SELECT
    c.NAME
FROM 
    CITY AS c
WHERE
    c.POPULATION > 120000 AND c. COUNTRYCODE = 'USA'

```

#3
Query all columns (attributes) for every row in the CITY table.

```sql
SELECT
    *
FROM 
    CITY AS c
```

# 4

Query all columns for a city in CITY with the ID 1661.

```sql
SELECT
    *
FROM 
    CITY AS c
WHERE
    c.ID = 1661
```

# 5
Query all attributes of every Japanese city in the CITY table. The COUNTRYCODE for Japan is JPN.

```
SELECT
    *
FROM 
    CITY AS c
WHERE
    c.COUNTRYCODE = 'JPN'
```

#6

Query the names of all the Japanese cities in the CITY table. The COUNTRYCODE for Japan is JPN.

```sql
SELECT
    c.NAME
FROM 
    CITY AS c
WHERE
    c.COUNTRYCODE = 'JPN'
```

#7
Query a list of CITY and STATE from the STATION table.
```sql
SELECT
    a.CITY
    ,A.STATE
FROM
    STATION AS a
```
# 8

Query a list of CITY names from STATION for cities that have an even ID number. Print the results in any order, but exclude duplicates from the answer.
```
SELECT DISTINCT
    CITY
FROM
    STATION
WHERE   
    ID%2=0
```

