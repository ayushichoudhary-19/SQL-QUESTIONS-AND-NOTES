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


### PROBLEM - 3
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
> A nested variation of two of the above problems



### PROBLEM - 4
https://www.hackerrank.com/challenges/weather-observation-station-9/problem
  
   **Solution:**
```
SELECT DISTINCT CITY
FROM STATION
WHERE (CITY LIKE '%a' OR CITY LIKE '%e' OR CITY LIKE '%i' OR CITY LIKE '%o' OR CITY LIKE '%u')
AND CITY IN (SELECT DISTINCT CITY 
FROM STATION 
WHERE CITY LIKE 'a%' OR CITY LIKE 'e%' OR CITY LIKE 'i%' OR CITY LIKE 'o%' OR CITY LIKE 'u%' );

```


### PROBLEM - 5
https://www.hackerrank.com/challenges/more-than-75-marks/problem
  
   **Solution:**
```
SELECT NAME 
FROM STUDENTS
WHERE MARKS>75 
ORDER BY RIGHT(NAME,3), ID ASC;

```

> There are a lot of takeaways in this problem. Firstly you get to know about using a secondary order and right string function also. Here is more about it.
> In SQL, `RIGHT()` is a string function that is used to extract a specified number of characters from the right end (end of the string) of a given string. The syntax for the `RIGHT()` function is as follows:
```sql
RIGHT(string_expression, number_of_characters)
```

> - `string_expression`: This is the input string from which you want to extract characters. - `number_of_characters`: This is an integer value that specifies how many characters you want to extract from the right end of the input string.

Here's an example of how to use the `RIGHT()` function:

```sql
SELECT RIGHT('Hello, World!', 6); -- This returns 'World!'
```

### PROBLEM - 5
https://www.hackerrank.com/challenges/name-of-employees/problem
  
   **Solution:**
   

```
SELECT NAME 
FROM EMPLOYEE
ORDER BY NAME;
```
> It's written as OREDER <space> BY and not OREDERBY :)
