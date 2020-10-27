# data-science-homework

Assessment for Data / Growth Science role at Eaze.

<br />

Expected completion time: ~1.5 hours. Note that the time next to each question is not a limit but rather a suggestion; feel free to spend more time if you need it.

<br />

How do I take this assessment?
  1. Clone this repo onto your local machine.  
      ```git clone https://github.com/eaze/data-science-homework.git```
  2. Answer the questions below by filling out the files in the solutions folder.  
  3. Zip your solutions folder with your name in the filename.  
      ```zip -r solutions_{first_name}_{last_name}.zip solutions```  
  4. Email ```solutions_{first_name}_{last_name}.zip``` to ```analytics@eaze.com``` (or your recruiter).
      
<br />

What topics are covered?
  - Mathematics / Problem Solving
  - Probability
  - Hypothesis testing
  - Data Science (Modeling, Machine Learning)

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
you the first five cards (which are now removed from the deck), they offer
you the chance to bet on the outcome of the sixth card: if it's a face card, you 
quadruple your money; otherwise, you lose your money. For example, if you bet $1 and 
win you will end with $4 (your $1 + winnings of $3), but if you bet $1 and lose you
will end with $0 (a loss of your $1).

What is the probability that taking this bet will be in your favor?

Write your answer (rounded to 5 decimal points) in question_2.txt.

*Hint: The answer is not simply the probability that the sixth card is a face card. Our question is equivalent to asking: "What is the probability that you will be dealt a 5-card hand such that taking the bet is in your favor?"*

<br />

Question 3. Delivery rate (Statistics) [5 minutes]

A food delivery company averages 100 deliveries in 5 minutes. Find the approximate 95% interval for the number of deliveries per hour. 

Write your answers in question_3.txt; provide two values, each up to 1 digit after decimal point. 

i.e. lower_bound, upper_bound

<br />

Question 4. Hypothesis Testing (Statistics) [5 minutes]

After a new method of quality control was introduced in the packing process of goods in a warehouse,
200 packages were examined and 26 showed some defects. Before this method was implemented,
the defective rate was at most 10%. The warehouse needs to determine whether the new method actually increases the defective rate.

At alpha = 0.05 significance level, what is the test statistics, and is the increase in defective rate of new method statistically significant? 

Write your answers in question_4.txt; test statistic up to 3 digits after decimal point, then boolean value (1 if it is significant, 0 otherwise).

i.e. test_statistics, boolean

<br />

Question 5. Forecasting (Data Science) [60 minutes]

Write a function in Python that takes in a dataset (.csv file; see data/hourly_volume.csv for sample data)
and a number of days forward, and generates predictions for hourly
order volume. Feel free to use any existing libraries/packages.

*Notes: 1) Forecasts should be produced starting at the end of the supplied dataset. E.g. if the dataset contains data up to 2018-01-31 and days_forward is 2, then your function should return predictions for every date in [2018-02-01 00:00:00, 2018-02-02 23:00:00]. 2) Your function should return a data table with only two columns: the first one referring to order hour (formatted like example dates in this comment) and the second one referring to the predicted order volume.*

Write your function in question_5.py.

<br />

<br />
