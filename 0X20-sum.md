# SUM

Perform addition of a data set.

lets `sum` the total price of every car that we have in our table.

```sql
SELECT SUM(price) FROM car;
```

It will give the total price.

Lets aggregate this and see the total sum by the actual car make.

```sql
SELECT make, SUM(price) FROM car GROUP BY make;
```

You will see the total sum of all makes.
