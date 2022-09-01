# Repetition tracking

1. select from
2. derived columns
- lecture
    - `film`.`rental_duration`: display in hours
    - duration: date - date = interval
    - concat: fn, ||
    - initcap (capitalize)
- 3.5 🚩 **23/07/22** 🍏
- 3.6 🚩 **23/07/22** 🍏
- 3.7 🚩 **23/07/22** 🍏

3. filter with where
- lecture
    - =, >, <, >=, <=, <>, !=
    - quote: single for literal, double for table, column, identifier
    - timestamp = date + time
- 3.8 🚩 **23/07/22** 🍏
- 3.9 🚩 **23/07/22** 🍏
- 3.10 🚩 **23/07/22** 🍏
- 3.11 🚩 **23/07/22** 🍏

4. and, or, not
- lecture
- 3.12 🚩 **24/07/22** 🍏
- 3.13 🚩 **24/07/22** 🍏
- 3.14 🚩 **24/07/22** 🍏
- 3.15 🚩 **24/07/22** 🍏

5. null handling
- lecture
    - 3-value logic (true, false, unknown)
    - use `not null` as much as possible
- 3.16 🚩 **24/07/22** 🍏
- 3.17 🚩 **24/07/22** 🍏

6. in, between, like
- lecture
    - `__A%` matches str with `A` as third char (`_` * 2)
    - ilike: sql way for in-case-sensitive
    - `similar to 'M%L{2}%'`
- 3.18 🚩 **26/07/22** 🍏
- 3.19 🚩 **26/07/22** 🍏
- 3.20 🚩 **26/07/22** 🍏
- 3.21 🚩 **26/07/22** 🔴

7. order by
- lecture
    - nulls first, nulls last
- 3.22 🚩 **26/07/22** 🍏
- 3.23 🚩 **26/07/22** 🍏
- 3.24 🚩 **26/07/22** 🍏
- 3.25 🚩 **26/07/22** 🍏

8. order of execution
- lecture
    - order mnemonic: `from` the place `where` the `group` `has` been `select`ed and `order`ed there's a `limit`
- 3.26 🚩 **30/07/22** 🍏

9. limit and offset
- lecture
- 3.27 🚩 **30/07/22** 🍏
- 3.28 🚩 **30/07/22** 🔴
- 3.29 🚩 **30/07/22** 🍏
- 3.30 🚩 **30/07/22** 🍏

9. distinct
- lecture
    - multiple fields => distinct combinations
- 3.31 🚩 **31/07/22** 🍏
- 3.32 🚩 **31/07/22** 🍏
- 3.33 🚩 **31/07/22** 🍏
- 3.34 🚩 **31/07/22** 🍏

10. case exp
- lecture
    - in: select, where, order by
    - forms: search, simple
- 3.35 🚩 **31/07/22** 🍏
- 3.36 🚩 **31/07/22** 🍏
- 3.37 🚩 **31/07/22** 🔴

11. challenge
- 3.38 🚩 **01/08/22** 🔴
- 3.39 🚩 **01/08/22** 🍏
- 3.40 🚩 **01/08/22** 🔴
- 3.41 🚩 **01/08/22** 🍏
- 3.42 🚩 **01/08/22** 🔴
- 3.43 🚩 **01/08/22** 🍏

11. Common aggregate functions
- lecture
- 4.1 🚩 **01/08/22** 🍏
- 4.2 🚩 **01/08/22** 🍏
- 4.3 🚩 **01/08/22** 🍏
- 4.4 🚩 **01/08/22** 🍏
- 4.5 🚩 **01/08/22** 🍏

12. group by, having
- lecture
- 4.6 🚩 **01/08/22** 🍏
- 4.7 🚩 **01/08/22** 🍏
- 4.8 🚩 **01/08/22** 🍏

13. CASE expressions and aggregations
- lecture
    - sum(case when ... then 1 else then 0)
    - sum(case when ... then 1)
    - count(case when ... then 1 else then null)
    - count(case when ... then 1)
    - count(*) filter (where ...)
- 4.9 🚩 **02/08/22** 🍏
- 4.10 🚩 **02/08/22** 🔴

14. Challenge exercises
- 4.11 🚩 **02/08/22** 🍏
- 4.12 🚩 **02/08/22** 🍏
- 4.13 🚩 **02/08/22** 🔴
- 4.14 🚩 **02/08/22** 🍏

15. Character data types
- lecture
    - varchar vs text
    - concat vs ||
    - coercion
    - coalesce
    - trim, length + trim
    - lower, upper, left, right
    - substr (1-based index)
- 5.1 🚩 **02/08/22** 🍏
- 5.2 🚩 **02/08/22** 🍏

16. Number data types
- lecture
    - int2 (smallint), int4 (int), int8 (bigint)
    - pg_typeof
    - type coersion
    - explicit casting (3 ways): int '10', '10'::int, cast('10' as int)
    - count(*) returns bigint, bigint/int => bigint
    - categoties:
        - exact type: numeric === decimal, numeric(precision, scale) -> fixed
        - approximate type (floating-point type): real, double precision
- 5.3 🚩 **06/08/22** 🍏
- 5.4 🚩 **06/08/22** 🔴

17. Date and time data types
- lecture
    - 'YYYY-MM-DD'
    - date - date = num of days (int)
    - ts - ts = interval
    - justify_hours
    - date_part('epoch', interval)
    - date_trunc => when grouping
    - current_date, current_time, current_timestamp
- 5.5 🚩 **06/08/22** 🍏
- 5.6 🚩 **06/08/22** 🍏
- 5.7 🚩 **06/08/22** 🍏
- 5.8 🚩 **06/08/22** 🍏

18. Challenge exercises
- 5.9 🚩 **07/08/22** 🔴
- 5.10 🚩 **07/08/22** 🍏
- 5.11 🚩 **07/08/22** 🍏
- 5.12 🚩 **07/08/22** 🍏
- 5.13 🚩 **07/08/22** 🍏
- 5.14 🚩 **07/08/22** 🍏

19. Cross join
- lecture
    - cartesian product

20. Inner join
- lecture
- 6.1 🚩 **07/08/22** 🍏
- 6.2 🚩 **07/08/22** 🍏
- 6.3 🚩 **07/08/22** 🔴  
- 6.4 🚩 **07/08/22** 🍏
- 6.5 🚩 **07/08/22** 🍏

21. Outer join
- lecture
    - left join use cases: find posts that do not have comments, count comments of all posts
    - `left join`, followed by `inner join`
- 6.6 🚩 **08/08/22** 🍏
- 6.7 🚩 **08/08/22** 🍏

22. advanced join
- lecture
    - self-join: pair up diff combination within one column
- 6.8 🚩 **08/08/22** 🔴

23. Challenge exercises
- 6.9 🚩 **10/08/22** 🍏
- 6.10 🚩 **10/08/22** 🍏
- 6.11 🚩 **10/08/22** 🔴

24. Exercises - Uncorrelated subqueries
- 7.1 🚩 **28/08/22** 🍏
- 7.2 🚩 **28/08/22** 🍏
- 7.3 🚩 **28/08/22** 🔴

25. Exercises - Correlated subqueries
- 7.4 🚩 **30/08/22** 🍏
- 7.5 🚩 **30/08/22** 🔴
- 7.6 🚩 **30/08/22** 🔴

26. Exercises - Table subqueries
- 7.7 🚩 **30/08/22** 🍏
- 7.8 🚩 **30/08/22** 🔴

27. Exercises - Lateral subqueries
- 7.9 🚩 **31/08/22** 🍏

28. Exercises - Common table expressions
- 7.10 🚩 **31/08/22** 🍏
- 7.11 🚩 **31/08/22** 🔴

29. Challenge exercises
- 7.12 🚩 **01/09/22** 🔴
- 7.13 🚩 **01/09/22** 🍏
- 7.14 🚩 **01/09/22** 🔴
- 7.15 🚩 **01/09/22** 🔴
- 7.16 🚩 **01/09/22** 🍏

29. Ranking window functions
- lect
    - row_number(), rank(), dense_rank()
- 8.1 🚩 **01/09/22** 🍏
- 8.2 🚩 **01/09/22** 🔴
- 8.3 🚩 **01/09/22** 🔴

29. Aggregate window functions
- lect
- 8.4 🚩 **01/09/22** 
- 8.5 🚩 **01/09/22**