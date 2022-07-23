### 5.9 Write a query to return a count of the number of films that were rented out on the last day of a month

```sql
select
	count(*)
from rental
where date_part('day', rental_date) = date_part('day', date_trunc('month', rental_date + interval '1 month') - interval '1 day');
```

### ⚠️ 5.10 Write a query to list the film titles that have spaces at the beginning or end (we want to flag them so we know to clean them up!)
```sql
select
	title
from film
where length(trim(title)) < length(title);
```

### ⚠️ 5.11 Write a query to sum up, for each customer, the total number of hours they have had films rented out for. Return only the top 3 customers with the most hours.

```sql
select
	customer_id,
	round(sum(date_part('epoch', return_date - rental_date)) / 3600) as hrs_rented
from rental
group by customer_id
order by 2 desc
limit 3;
```

### 5.12 Postgres has a really useful function called generate_series which will come in handy in a few of the coming chapters. 
### Have a look at the examples how to use it here and then write a query to generate a list of timestamps which represent the first day of every month in 2019, at 5pm UTC

```sql
select
	generate_series(
		timestamptz '2019-01-01 17:00 UTC',
		timestamptz '2019-12-01 17:00 UTC',
		interval '1 day'
	)
```

:star: generate_series takes 3 arguments - the start, stop, and step

### 5.14 Write a query to tally up the total amount of money made on weekends (Saturday and Sunday)

```sql
select
	sum(amount)
from payment
where date_part('isodow', payment_date) in (6,7);
```

:star: You can use either the ‘dow’ or ‘isodow’ options with the date_part function to obtain a numerical representation of the day of the week. When using ‘isodow’, 6 represents Saturday and 7 represents Sunday. Handy!


### 5.13 Return a count of the number of occurrences of the letter ‘A’ in each customer’s first name 
### (this is a common interview question for SQL related jobs!). Order the output by the count descending.

```sql
select
	first_name,
	length(first_name) - length(regexp_replace(first_name, 'a', '', 'gi')) as count
from customer
order by count desc;
```

