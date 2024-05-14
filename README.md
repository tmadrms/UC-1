# Coupon Acceptance Rates

## Context

Imagine driving through town and a coupon is delivered to your cell phone for a restaurant near where you are driving. Would you accept that coupon and take a short detour to the restaurant? Would you accept the coupon but use it on a subsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaurant? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

## Overview

The goal of this project is to use visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

## Data

This data comes from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then asks the person whether they will accept the coupon if they are the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20 - $50).

## Bar Coupon Acceptance Rates

### Overall Acceptance Rate
- **Acceptance rate for bar coupons:** 41.00%

### Acceptance Rates Based on Bar Visit Frequency
- **Acceptance rate for those who went to a bar 3 or fewer times a month:** 37.06%
- **Acceptance rate for those who went to a bar more than 3 times a month:** 76.88%
- **Acceptance rate for those with 'NotSpecified' in 'Bar' column:** 38.10%

### Acceptance Rates Based on Age and Frequency
- **Acceptance rate for drivers who go to a bar more than once a month and are over the age of 25:** 77.21%
- **Acceptance rate for all other drivers:** 38.38%
- **Acceptance rate for drivers who go to bars more than once a month:** 68.79%
- **Acceptance rate for drivers that go to bars more than once a month, had passengers that were not a kid, and were not widowed:** 71.79%
- **Acceptance rate for drivers that go to bars more than once a month and are under the age of 30:** 80.88%

### Acceptance Rates Based on Occupation and Passenger
- **Acceptance rate for drivers that had passengers who are not kids, and have occupations other than farming, fishing, or forestry:** 48.36%
- **Acceptance rate for drivers that go to cheap restaurants more than 4 times a month and income is less than 50K:** 45.35%

### Detailed Acceptance Rates for Specific Groups
- **Acceptance rate for drivers that go to bars more than once a month, had passengers that were not a kid, and were not widowed:** 71.79%
- **Acceptance rate for drivers that go to bars more than once a month and are under the age of 30:** 80.88%
- **Acceptance rate for drivers that go to cheap restaurants more than 4 times a month and income is less than 50K:** 45.35%

### Detailed Acceptance Rates for Drivers with Passengers
- **Acceptance rate for drivers that had passengers who are not kids, and have occupations other than farming, fishing, or forestry:** 48.36%

### Observations
- **Those without urgent destinations are more likely to accept.**
- **Having a friend as a passenger raises probability.**
- **Younger individuals (30 and under) are more likely to use the coupon.**
- **Those who go to bars are far more likely, especially those who go more than 3 times per month.**




## Coffee House Coupon Acceptance Rates

### Overall Acceptance Rate
- **Acceptance rate for Coffee House coupons:** 49.92%

### Acceptance Rates Based on Coffee House Visit Frequency
- **Acceptance rate for those who went to a Coffee House 3 or fewer times a month:** 44.94%
- **Acceptance rate for those who went to a Coffee House more than 3 times a month:** 67.50%
- **Acceptance rate for those with 'NotSpecified' in 'Coffee House' column:** 45.83%

### Acceptance Rates Based on Age and Frequency
- **Acceptance rate for drivers who go to a Coffee House more than once a month and are over the age of 25:** 64.34%
- **Acceptance rate for all other drivers:** 47.29%

### Observations from Graphs
- **Destination:**
  - Those without urgent destinations are more likely to accept.
- **Passenger:**
  - Having a friend as a passenger raises the probability of acceptance.
- **Weather and Temperature:**
  - Weather and temperature have no bearing on acceptance.
- **Time of Day:**
  - 10 AM and 2 PM have the highest acceptance rates.
- **Expiration Time:**
  - 1-day expirations work best.
- **Age:**
  - While not enormous, those that are younger (26 and under) are more likely to use the coupon.
- **Other Factors:**
  - Marital status, income level, having children, and education level have little bearing.
  - Those who go to coffee houses are far more likely, especially those who go 1-3 times per week.

### Detailed Acceptance Rates for Frequent Coffee House Visitors by Time of Day
- **10 AM:** 81.29%
- **10 PM:** 49.65%
- **2 PM:** 73.35%
- **6 PM:** 58.68%
- **7 AM:** 59.09%

### Acceptance Rate for Younger Individuals (26 and under)
- **Acceptance Rate:** 53.43%

### Detailed Acceptance Rates by Time of Day and Expiration Time
- **10 AM - 1 Day Expiration:** 65.58%
- **10 AM - 2 Hours Expiration:** 63.17%
- **10 PM - 1 Day Expiration:** 66.93%
- **10 PM - 2 Hours Expiration:** 24.12%
- **2 PM - 1 Day Expiration:** 59.22%
- **2 PM - 2 Hours Expiration:** 49.44%
- **6 PM - 1 Day Expiration:** 50.09%
- **6 PM - 2 Hours Expiration:** 32.35%
- **7 AM - 1 Day Expiration:** 60.56%
- **7 AM - 2 Hours Expiration:** 35.87%

## Summary
The analysis shows that bar coupons are generally more accepted by individuals without urgent destinations, those with friends as passengers, and are frequent visitors of bars. 

Similarly, coffee house coupons are more accepted by those without urgent destinations and frequent visitors of coffee houses. Acceptance rates vary significantly based on time of day and expiration time, with younger individuals also showing higher acceptance rates. These insights can be used to tailor marketing strategies and increase the effectiveness of both bar and coffee house coupons.
