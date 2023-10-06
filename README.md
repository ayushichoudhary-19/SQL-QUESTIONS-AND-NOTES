# SQL Practice Repository

Welcome to my SQL practice repository! 📊📚

This repository contains SQL solutions to various questions from LeetCode and HackerRank. It serves as a personal learning resource where I store my solutions and jot down key takeaways and notes as a beginner in SQL.

## Contents

- **LeetCode Solutions:** SQL solutions to LeetCode questions.
- **HackerRank Solutions:** SQL solutions to HackerRank questions.

I hope you find these solutions and notes helpful in your own SQL learning journey. Feel free to explore the content, and if you have any suggestions or improvements, please let me know. Happy coding! 😄📖

# SQL Basics and Prerequisites

Before diving into SQL problem-solving on platforms like LeetCode and HackerRank, it's essential to have a good grasp of the basics. This guide provides a quick overview of some fundamental SQL concepts and common query functions:  [PREREQUISITED.MD](https://github.com/ayushichoudhary-19/SQL-QUESTIONS-AND-NOTES/blob/main/PREREQUISITES.MD))


---

**Now, that you're ready:**
# LET'S GO!
### PROBLEM - 1
https://www.hackerrank.com/challenges/weather-observation-station-6/problem
  
   **Solution:**
```
SELECT DISTINCT CITY 
FROM STATION 
WHERE CITY LIKE 'a%' OR CITY LIKE 'e%' OR CITY LIKE 'i%' OR CITY LIKE 'o%' OR CITY LIKE 'u%';
```
> 💡 I initialy did a mistake in using `=` sign as in `WHERE CITY LIKE = 'a%'` But we aren't suppoed to use `=` with `LIKE` 

### PROBLEM - 2
https://www.hackerrank.com/challenges/weather-observation-station-7/problem
  
   **Solution:**
```
SELECT DISTINCT CITY
FROM STATION
WHERE CITY LIKE '%a' OR CITY LIKE '%e' OR CITY LIKE '%i' OR CITY LIKE '%o' OR CITY LIKE '%u' 
```
> Same as above one


### PROBLEM - 2
https://www.hackerrank.com/challenges/weather-observation-station-8/problem
  
   **Solution:**
```
SELECT DISTINCT CITY
FROM STATION
WHERE (CITY LIKE '%a' OR CITY LIKE '%e' OR CITY LIKE '%i' OR CITY LIKE '%o' OR CITY LIKE '%u')
AND CITY IN (SELECT DISTINCT CITY 
FROM STATION 
WHERE CITY LIKE 'a%' OR CITY LIKE 'e%' OR CITY LIKE 'i%' OR CITY LIKE 'o%' OR CITY LIKE 'u%' );

```
> Same as above one




