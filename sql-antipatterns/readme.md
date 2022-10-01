# sql anti-patterns

## 1 Introduction 13
1.1 Who This Book Is For 
1.2 What’s in This Book 
1.3 What’s Not in This Book 
1.4 Conventions 
1.5 Example Database 
1.6 Acknowledgments 

## I Logical Database Design Antipatterns 24

2 Jaywalking 25
2.1 Objective: Store Multivalue Attributes 
2.2 Antipattern: Format Comma-Separated Lists 
2.3 How to Recognize the Antipattern 
2.4 Legitimate Uses of the Antipattern 
2.5 Solution: Create an Intersection Table 

3 Naive Trees 34
3.1 Objective: Store and Query Hierarchies 
3.2 Antipattern: Always Depend on One’s Parent 
3.3 How to Recognize the Antipattern 
3.4 Legitimate Uses of the Antipattern 
3.5 Solution: Use Alternative Tree Models 

4 ID Required 54
4.1 Objective: Establish Primary Key Conventions 
4.2 Antipattern: One Size Fits All 
4.3 How to Recognize the Antipattern 
4.4 Legitimate Uses of the Antipattern 
4.5 Solution: Tailored to Fit 

5 Keyless Entry 65
5.1 Objective: Simplify Database Architecture 
5.2 Antipattern: Leave Out the Constraints 
5.3 How to Recognize the Antipattern 
5.4 Legitimate Uses of the Antipattern 
5.5 Solution: Declare Constraints 

6 Entity-Attribute-Value 73
6.1 Objective: Support Variable Attributes 
6.2 Antipattern: Use a Generic Attribute Table 
6.3 How to Recognize the Antipattern 
6.4 Legitimate Uses of the Antipattern 
6.5 Solution: Model the Subtypes 

7 Polymorphic Associations 89
7.1 Objective: Reference Multiple Parents 
7.2 Antipattern: Use Dual-Purpose Foreign Key 
7.3 How to Recognize the Antipattern 
7.4 Legitimate Uses of the Antipattern 
7.5 Solution: Simplify the Relationship 

8 Multicolumn Attributes 102
8.1 Objective: Store Multivalue Attributes 
8.2 Antipattern: Create Multiple Columns 
8.3 How to Recognize the Antipattern 
8.4 Legitimate Uses of the Antipattern 
8.5 Solution: Create Dependent Table 

9 Metadata Tribbles 110
9.1 Objective: Support Scalability 
9.2 Antipattern: Clone Tables or Columns 
9.3 How to Recognize the Antipattern 
9.4 Legitimate Uses of the Antipattern 
9.5 Solution: Partition and Normalize 

## II Physical Database Design Antipatterns 122

10 Rounding Errors 123
10.1 Objective: Use Fractional Numbers Instead of Integers 124
10.2 Antipattern: Use FLOAT Data Type 
10.3 How to Recognize the Antipattern 
10.4 Legitimate Uses of the Antipattern 
10.5 Solution: Use NUMERIC Data Type 

11 31 Flavors 131
11.1 Objective: Restrict a Column to Specific Values 
11.2 Antipattern: Specify Values in the Column Definition . 132
11.3 How to Recognize the Antipattern 
11.4 Legitimate Uses of the Antipattern 
11.5 Solution: Specify Values in Data 

12 Phantom Files 139
12.1 Objective: Store Images or Other Bulky Media 
12.2 Antipattern: Assume You Must Use Files 
12.3 How to Recognize the Antipattern 
12.4 Legitimate Uses of the Antipattern 
12.5 Solution: Use BLOB Data Types As Needed 

13 Index Shotgun 148
13.1 Objective: Optimize Performance 
13.2 Antipattern: Using Indexes Without a Plan 
13.3 How to Recognize the Antipattern 
13.4 Legitimate Uses of the Antipattern 
13.5 Solution: MENTOR Your Indexes 

III Query Antipatterns 161
14 Fear of the Unknown 162
14.1 Objective: Distinguish Missing Values 
14.2 Antipattern: Use Null as an Ordinary Value, or Vice Versa163
14.3 How to Recognize the Antipattern 
14.4 Legitimate Uses of the Antipattern 
14.5 Solution: Use Null as a Unique Value 

15 Ambiguous Groups 173
15.1 Objective: Get Row with Greatest Value per Group 
15.2 Antipattern: Reference Nongrouped Columns 
15.3 How to Recognize the Antipattern 
15.4 Legitimate Uses of the Antipattern 
15.5 Solution: Use Columns Unambiguously 

16 Random Selection 183
16.1 Objective: Fetch a Sample Row 
16.2 Antipattern: Sort Data Randomly 
16.3 How to Recognize the Antipattern 
16.4 Legitimate Uses of the Antipattern 
16.5 Solution: In No Particular Order

17 Poor Man’s Search Engine 190
17.1 Objective: Full-Text Search 
17.2 Antipattern: Pattern Matching Predicates 
17.3 How to Recognize the Antipattern 
17.4 Legitimate Uses of the Antipattern 
17.5 Solution: Use the Right Tool for the Job 

18 Spaghetti Query 204
18.1 Objective: Decrease SQL Queries 
18.2 Antipattern: Solve a Complex Problem in One Step 
18.3 How to Recognize the Antipattern 
18.4 Legitimate Uses of the Antipattern 
18.5 Solution: Divide and Conquer 

19 Implicit Columns 214
19.1 Objective: Reduce Typing 
19.2 Antipattern: a Shortcut That Gets You Lost 
19.3 How to Recognize the Antipattern 
19.4 Legitimate Uses of the Antipattern 
19.5 Solution: Name Columns Explicitly 

## IV Application Development Antipatterns 221

20 Readable Passwords 222
20.1 Objective: Recover or Reset Passwords 
20.2 Antipattern: Store Password in Plain Text 
20.3 How to Recognize the Antipattern 
20.4 Legitimate Uses of the Antipattern 
20.5 Solution: Store a Salted Hash of the Password 

21 SQL Injection 234
21.1 Objective: Write Dynamic SQL Queries 
21.2 Antipattern: Execute Unverified Input As Code 
21.3 How to Recognize the Antipattern 
21.4 Legitimate Uses of the Antipattern 
21.5 Solution: Trust No One 

22 Pseudokey Neat-Freak 250
22.1 Objective: Tidy Up the Data 
22.2 Antipattern: Filling in the Corners 
22.3 How to Recognize the Antipattern 
22.4 Legitimate Uses of the Antipattern 
22.5 Solution: Get Over It 

23 See No Evil 259
23.1 Objective: Write Less Code 
23.2 Antipattern: Making Bricks Without Straw 
23.3 How to Recognize the Antipattern 
23.4 Legitimate Uses of the Antipattern 
23.5 Solution: Recover from Errors Gracefully 

24 Diplomatic Immunity 266
24.1 Objective: Employ Best Practices 
24.2 Antipattern: Make SQL a Second-Class Citizen 
24.3 How to Recognize the Antipattern 
24.4 Legitimate Uses of the Antipattern 
24.5 Solution: Establish a Big-Tent Culture of Quality 

25 Magic Beans 278
25.1 Objective: Simplify Models in MVC 
25.2 Antipattern: The Model Is an Active Record 
25.3 How to Recognize the Antipattern 
25.4 Legitimate Uses of the Antipattern 
25.5 Solution: The Model Has an Active Record 

V Appendixes 293
A Rules of Normalization 294
A.1 What Does Relational Mean? 
A.2 Myths About Normalization 
A.3 What Is Normalization? 
A.4 Common Sense 
B Bibliography 309
Index 311
