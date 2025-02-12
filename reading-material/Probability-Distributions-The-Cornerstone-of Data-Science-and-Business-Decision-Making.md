# Probability Distributions in Data Science and Business Decision-Making

Source: [Main Tweet](https://x.com/mdancho84/status/1889292944814846424)

![Main Tweet Image](https://pbs.twimg.com/media/Gjgd68LX0AAAuIi?format=png&name=small)


## 1. Probability Distribution Fundamentals
In statistics, a probability distribution is a mathematical function that provides the probabilities of occurrence of different possible outcomes in an experiment. It's a way to describe how likely different outcomes will occur. There are two main types of probability distributions: Discrete and Uniform.

## 2. Discrete Distribution
These are used when the set of possible outcomes is discrete (i.e., can be counted). For example, the number of customers that convert in a time period (which can only take on the values 1, 2, 3, 4, 5, 6, etc).

## 3. Continuous Distribution
These are used when the set of possible outcomes can take on any value in a range. For example, the conversion rate of customers in a given time period is N_conv / N_total, which divides customers (discrete) by the total number of website visits. The resulting conversion rate is continuous.

## 4. Probability Functions (PDF and PMF)
This is how we calculate the probability of an event occurring. Discrete probabilities have a Probability Mass Function (PMF), while continuous probabilities have a Probability Density Function (PDF).

## 5. Expected Value
**IMPORTANT, THIS IS WHAT I USE TO MAKE DECISIONS:**  
Arguably the most important concept in my opinion is the concept of Expected Value (EV). The expected value is like the long-run average or most typical outcome. I use this to make business decisions. Here's an example.

## 6. Application: Lead Scoring Model
I made a basic logistic regression model that helped my team know which quotes to work on. The model predicted a class probability from 0 to 1, with 0 being not likely to buy and 1 being 100% likely to buy. But to decide whether or not to spend days working on the time-intensive quote, I need to know the Expected Value.

## 7. Business Decision Making
The $15,000,000 question was, which quote (lead) to work on?  

A routine example:

- **Option 1:** $3,000,000 Quote Value x 0.02 Predicted Probability of Buying = $60,000 EV  
- **Option 2:** $100,000 Quote Value x 0.90 Predicted Probability of Buying = $90,000 EV  

The choice is easy: We work on the latter all day every day. We only work on the larger when EV exceeds the smaller higher probability quotes.  
Doing this helped us grow revenue from $3M to $15,000,000 in under 2 years.
