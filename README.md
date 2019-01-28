# data-science-homework

Assessment for Data / Growth Science role at Eaze.

<br />

Expected completion time: 3 hours.

<br />

How do I take this assessment?
  1. Clone this repo onto your local machine.  
      ```git clone https://github.com/eaze/data-science-homework.git```
  2. Answer the questions below by filling out the files in the solutions folder.  
  3. Zip your solutions folder.  
      ```zip -r solutions.zip solutions```  
  4. Email ```solutions.zip``` to ```atilley@eaze.com``` and ```shri@eaze.com``` (or your recruiter).
  5. You'll receive an email with your results.
      
*Important Note: Questions 4 and 5 can both be completed in either R or Python. If you fill out both the R and Python 
function files for a question, we will score both and give you the best result.

<br />

What topics are covered?
  - Mathematics / Problem Solving
  - Probability
  - SQL
  - Data Science (Modeling, Machine Learning)
  - Applied Mathematics

<br />

Question 1. Positive Fractions (Math / Problem Solving) [5 minutes]

The numerator and denominator of Juan’s fraction are positive integers whose 
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

*Hint: The answer is not simply the probability that the sixth card is a face card. Imagine that the dealer is asking you to place your bet before handing you any cards; what is the probability that doing so will result in a monetary gain for you?*

<br />

Question 3. Order Query (SQL) [15 minutes]

Write a SQL query (using SQLite syntax - http://www.sqlite.org/index.html) on the user_orders table (data/user_orders.csv)
that returns the following table:

user first_29_day_orders

which contains one row for every user along with how many orders they had in
their first 29 days.

Write your query in the format of a SELECT statement.

*Note: An order is considered to be in the user's first 29 days if
it happened before OR on first_date + days(28). E.g. if the user's first order
was on 1/1/2018, an order on 1/29/18 would still count as a first_29_day_order but an order on 1/30/18 would not.*

Write your query in question_3.sql.

<br />

Question 4. Forecasting (Data Science) [60 minutes]

Write a function in R or Python that takes in a dataset (.csv file; see data/hourly_volume.csv for sample data)
and a number of days forward, and generates predictions for hourly
order volume. Feel free to use any existing libraries/packages.

*Note: Forecasts should be produced starting at the end of the supplied dataset. E.g. if the dataset contains data up to 2018-01-31 and days_forward is 2, then your function should return predictions for every date in [2018-02-01 00:00:00, 2018-02-02 23:00:00].*

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

While there are N users, the binary state vector s has cardinality (N + 1) and is 
indexed at 0. The threshold vector t is a random variable distributed uniformly 
with support on [0.5, 1].

Write a function which takes in N (the number of users) and s_N (the sample 
expectation for the last user in the chain; this can also be interpreted as
the probability the last user in the chain is Active) and returns the maximum 
likelihood estimate of the state probability of s_0 (i.e. the probability 
that s_0 is 1). Please round your answer to 2 decimal places.

*Important Note: In order to receive a score, your function must finish running
in under 30 minutes for N <= 5.

Write your function in question_5.r or question_5.py.

<br />

<br />

If anything on this assessment is unclear, please email questions to ```atilley@eaze.com```.

