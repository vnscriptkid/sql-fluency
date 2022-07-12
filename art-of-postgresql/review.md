# Reviewables of art of postgresql

## II Introduction 1
1. Structured Query Language 2
1.1. Some of the Code is Written in SQL 
1.2. A First Use Case 
1.3. Loading the Data Set 
1.4. Application Code and SQL 
1.5. A Word about SQL Injection 
1.6. PostgreSQL protocol: server-side prepared statements 
1.7. Back to Discovering SQL 
1.8. Computing Weekly Changes 
2. Software Architecture 18
2.1. Why PostgreSQL? 
2.2. The PostgreSQL Documentation 
3. Getting Ready to read this Book 23

## III Writing Sql Queries 25
4. Business Logic 27
4.1. Every SQL query embeds some business logic 
4.2. Business Logic Applies to Use Cases 
4.3. Correctness 
4.4. Eஸஹ஭ciency 
4.5. Stored Procedures — a Data Access API 
4.6. Procedural Code and Stored Procedures 
4.7. Where to Implement Business Logic? 
5. A Small Application 41
5.1. Readme First Driven Development 
5.2. Loading the Dataset 
5.3. Chinook Database 
5.4. Music Catalog 
5.5. Albums by Artist 
5.6. Top-N Artists by Genre 
6. The SQL REPL — An Interactive Setup 52
6.1. Intro to psql 
6.2. The psqlrc Setup 
6.3. Transactions and psql Behavior 
6.4. A Reporting Tool 
6.5. Discovering a Schema 
6.6. Interactive Query Editor 
7. SQL is Code 60
7.1. SQL style guidelines 
7.2. Comments 
7.3. Unit Tests 
7.4. Regression Tests 
7.5. A Closer Look 
8. Indexing Strategy 71
8.1. Indexing for Constraints 
8.2. Indexing for Queries 
8.3. Cost of Index Maintenance 
8.4. Choosing Queries to Optimize 
8.5. PostgreSQL Index Access Methods 
8.6. Advanced Indexing 
8.7. Adding Indexes 
9. An Interview with Yohann Gabory 81

## IV SQL Toolbox 86
10. Get Some Data 88
11. Structured Query Language 89
12. Queries, DML, DDL, TCL, DCL 91
13. Select, From, Where 93
13.1. Anatomy of a Select Statement 
13.2. Projection (output): Select 
13.3. Data sources: From 
13.4. Understanding Joins 
13.5. Restrictions: Where 
14. Order By, Limit, No Offset 105
14.1. Ordering with Order By 
14.2. kNN Ordering and GiST indexes 
14.3. Top-N sorts: Limit 
14.4. No Oஸfset, and how to implement pagination 
15. Group By, Having, With, Union All 114
15.1. Aggregates (aka Map/Reduce): Group By 
15.2. Aggregates Without a Group By 
15.3. Restrict Selected Groups: Having 
15.4. Grouping Sets 
15.5. Common Table Expressions: With 
15.6. Distinct On 
15.7. Result Sets Operations 
16. Understanding Nulls 131
16.1. Three-Valued Logic 
16.2. Not Null Constraints 
16.3. Outer Joins Introducing Nulls 
16.4. Using Null in Applications 
17. Understanding Window Functions 137
17.1. Windows and Frames 
17.2. Partitioning into Diஸferent Frames 
17.3. Available Window Functions 
17.4. When to Use Window Functions 
18. Understanding Relations and Joins 143
18.1. Relations 
18.2. SQL Join Types 
19. An Interview with Markus Winand 148

## V Data Types 152
20. Serialization and Deserialization 154
21. Some Relational Theory 156
21.1. Attribute Values, Data Domains and Data Types 
21.2. Consistency and Data Type Behavior 
22. PostgreSQL Data Types 162
22.1. Boolean 
22.2. Character and Text 
22.3. Server Encoding and Client Encoding 
22.4. Numbers 
22.5. Floating Point Numbers 
22.6. Sequences and the Serial Pseudo Data Type 
22.7. Universally Unique Identiஹ஭er: UUID 
22.8. Bytea and Bitstring 
22.9. Date/Time and Time Zones 
22.10. Time Intervals 
22.11. Date/Time Processing and Querying 
22.12. Network Address Types 
22.13. Ranges 
23. Denormalized Data Types 193
23.1. Arrays 
23.2. Composite Types 
23.3. XML 
23.4. JSON 
23.5. Enum 
24. PostgreSQL Extensions 206
25. An interview with Grégoire Hubert 208

## VI Data Modeling 211
26. Object Relational Mapping 213
27. Tooling for Database Modeling 215
27.1. How to Write a Database Model 
27.2. Generating Random Data 
27.3. Modeling Example 
28. Normalization 227
28.1. Data Structures and Algorithms 
28.2. Normal Forms 
28.3. Database Anomalies 
28.4. Modeling an Address Field 
28.5. Primary Keys 
28.6. Surrogate Keys 
28.7. Foreign Keys Constraints 
28.8. Not Null Constraints 
28.9. Check Constraints and Domains 
28.10. Exclusion Constraints 
29. Practical Use Case: Geonames 240
29.1. Features 
29.2. Countries 
29.3. Administrative Zoning 
29.4. Geolocation Data 
29.5. Geolocation GiST Indexing 
29.6. A Sampling of Countries 
30. Modelization Anti-Patterns 258
30.1. Entity Attribute Values 
30.2. Multiple Values per Column 
30.3. UUIDs 
31. Denormalization 265
31.1. Premature Optimization 
31.2. Functional Dependency Trade-Oஸfs 
31.3. Denormalization with PostgreSQL 
31.4. Materialized Views 
31.5. History Tables and Audit Trails 
31.6. Validity Period as a Range 
31.7. Pre-Computed Values 
31.8. Enumerated Types 
31.9. Multiple Values per Attribute 
31.10. The Spare Matrix Model 
31.11. Partitioning 
31.12. Other Denormalization Tools 
31.13. Denormalize wih Care 
32. Not Only SQL 278
32.1. Schemaless Design in PostgreSQL 
32.2. Durability Trade-Oஸfs 
32.3. Scaling Out 
33. An interview with Álvaro Hernández Tortosa 286

## VII Data Manipulation and Concurrency Control 291
34. Another Small Application 293
35. Insert, Update, Delete 297
35.1. Insert Into 
35.2. Insert Into … Select 
35.3. Update 
35.4. Inserting Some Tweets 
35.5. Delete 
35.6. Tuples and Rows 
35.7. Deleting All the Rows: Truncate 
35.8. Delete but Keep a Few Rows 
36. Isolation and Locking 309
36.1. Transactions and Isolation 
36.2. About SSI 
36.3. Concurrent Updates and Isolation 
36.4. Modeling for Concurrency 
36.5. Putting Concurrency to the Test 
37. Computing and Caching in SQL 319
37.1. Views 
37.2. Materialized Views 
38. Triggers 324
38.1. Transactional Event Driven Processing 
38.2. Trigger and Counters Anti-Pattern 
38.3. Fixing the Behavior 
38.4. Event Triggers 
39. Listen and Notify 332
39.1. PostgreSQL Notiஹ஭cations 
39.2. PostgreSQL Event Publication System 
39.3. Notiஹ஭cations and Cache Maintenance 
39.4. Limitations of Listen and Notify 
39.5. Listen and Notify Support in Drivers 
40. Batch Update, MoMA Collection 342
40.1. Updating the Data 
40.2. Concurrency Patterns 
40.3. On Con஺ாict Do Nothing 
41. An Interview with Kris Jenkins 348

## VIII PostgreSQL Extensions 352
42. What’s a PostgreSQL Extension? 354
42.1. Inside PostgreSQL Extensions 
42.2. Installing and Using PostgreSQL Extensions 
42.3. Finding PostgreSQL Extensions 
42.4. A Primer on Authoring PostgreSQL Extensions 
42.5. A Short List of Noteworthy Extensions 
43. Auditing Changes with hstore 365
43.1. Introduction to hstore 
43.2. Comparing hstores 
43.3. Auditing Changes with a Trigger 
43.4. Testing the Audit Trigger 
43.5. From hstore Back to a Regular Record 
44. Last.fm Million Song Dataset 372
45. Using Trigrams For Typos 378
45.1. The pg_trgm PostgreSQL Extension 
45.2. Trigrams, Similarity and Searches 
45.3. Complete and Suggest Song Titles 
45.4. Trigram Indexing 
46. Denormalizing Tags with intarray 386
46.1. Advanced Tag Indexing 
46.2. Searches 
46.3. User-Deஹ஭ned Tags Made Easy 
47. The Most Popular Pub Names 392
47.1. A Pub Names Database 
47.2. Normalizing the Data 
47.3. Geolocating the Nearest Pub (k-NN search) 
47.4. Indexing kNN Search 
48. How far is the nearest pub? 398
48.1. The earthdistance PostgreSQL contrib 
48.2. Pubs and Cities 
48.3. The Most Popular Pub Names by City 
49. Geolocation with PostgreSQL 405
49.1. Geolocation Data Loading 
49.2. Finding an IP Address in the Ranges 
49.3. Geolocation Metadata 
49.4. Emergency Pub 
50. Counting Distinct Users with HyperLogLog 413
50.1. HyperLogLog 
50.2. Installing postgresql-hll 
50.3. Counting Unique Tweet Visitors 
50.4. Lossy Unique Count with HLL 
50.5. Getting the Visits into Unique Counts 
50.6. Scheduling Estimates Computations 
50.7. Combining Unique Visitors 
51. An Interview with Craig Kerstiens 425

## IX Closing Thoughts 428

## X Index