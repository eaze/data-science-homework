# data-science-homework

Assessment for Data / Growth Science role at Eaze.

<br />

Expected completion time: 3 hours.

<br />

How do I take this assessment?
  1. Clone this repo onto your local machine.  
      ```git clone https://github.com/eaze/data-science-homework.git```
  2. Create (and switch to) a new branch with your email address. (Note you must
     be in the directory for this to work).
      ```git checkout -b address@email.com```
  3. Answer the questions below by filling out the files in the solutions folder.  
  4. Zip your solutions folder.  
      ```zip -r solutions.zip solutions```  
  5. Email ```solutions.zip``` to ```atilley@eaze.com```.
  6. Your assessment will be scored, and you will receive an email with your
     results.
      
*Important Note: Questions 4 and 5 can be completed in either R or Python (doesn't
have to be the same for 4 and 5). If you fill out both the R and Python 
function files for a question, we will score both and give you the best result.

<br />

What topics are covered?
  - Math / Problem Solving
  - Probability
  - SQL
  - Data Science (Modeling, Machine Learning)
  - Applied Mathematics

<br />

Question 1. Positive Fractions (Math / Problem Solving) [5 minutes]

The numerator and denumerator of Juan’s fraction are positive integers whose 
sum is 2011. The value of this fraction is less than 1 / 3. Find the greatest
such fraction.

Write your answer in question_1.txt in the following format:  
numerator  
denominator

<br />

Question 2. Counting Cards (Probability) [10 minutes]

A standard deck of 52 cards has 12 "face cards" (Jack, Queen, King of each suit).
Suppose you're playing a game where you're given six cards. After the dealer gives
you the first five cards (which are now removed from the deck), he offers 
you the chance to bet on the outcome of the sixth card: if it's a face card, you 
quadruple your money; otherwise, you lose your money.

What is the probability that taking this bet will be in your favor?

Write your answer (rounded to 5 decimal points) in question_2.txt.

<br />

Question 3. Order Query (SQL) [15 minutes]

Write a SQL query (using ANSI/universal sql) on the user_orders table (data/user_orders.csv)
that returns the following table:

user first_28_day_orders

which contains one row for every user along with how many orders they had in
their first 28 days.

*Important Note: An order is considered to be in the user's first 28 days if
it happened before OR on first_date + days(28). E.g. if the user's first order
was on 1/1/2018, an order on 1/29/18 would still count as a first_28_day_order.

Write your query in question_3.sql.

<br />

Question 4. Forecasting (Data Science) [60 minutes]

Write a function in R or Python that takes in a dataset (.csv file)
and a number of days forward, and generates predictions for hourly
order volume.

Write your function in question_4.r or question_4.py.

<br />

Question 5. Referral Chain (Applied Mathematics) [90 minutes]

Suppose your business has a network of users who are all either Active (1) or
Inactive (0) (we call this the user's state). Each user was referred by an existing
user, except for the first user. At any given time, each user's likelihood of being 
Active is a function of their referrer's state along with some threshold t_i.

Specifically, we can define the state of each user with the following equation:

(docs/equation 1.jpg),

where user 1 referred user 2, user 2 referred user 3, user 3 referred user 4, etc.

In this system, each user except for user N has referred exactly one person.

While there are N users, the state vector s has length (N + 1) and is indexed at
0. The threshold vector t is unknown but distributed uniformly with support on
[0.5, 1].

Write a function which takes in N (the number of users) and s_N (the state 
probability for the last user in the chain) and returns the maximum likelihood estimate 
of s_0 (rounded to 2 decimal places).

*Important Note: In order to receive a score, your function must finish running
in under 30 minutes for N <= 5.

Write your function in question_5.r or question_5.py.

<br />

<br />

If anything on this assessment is unclear, please email questions to ```atilley@eaze.com```.

