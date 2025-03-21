# GROUP BY HAVING

- Group by having allows performance of an extra filtering after you perform the aggregation.

- We have `count` summing up everyone from each country. 

<img src="./img/co.png" alt="cb">


We can find all countries that have at least 5 people using `HAVING`.

- It takes the COUNT(*) function and then specify the count. For instance at least 5 will be `>5`.

```sql
SELECT country_of_birth, COUNT(*) FROM person GROUP BY country_of_birth HAVING COUNT(*) > 5 ORDER BY country_of_birth;
```

We will getting countries where there is at least 5 people.
 We can also use  `>=5`.

 <a href="https://www.postgresql.org/docs/9.5/functions-aggregate.html">Aggregate Functions</a>

 COUNT(*) is an aggregate function.

 





