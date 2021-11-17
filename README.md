# starbucks

## Introduction:
This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. Not all users receive the same offer, and that is the challenge to solve with this data set.
<br />
## Data Sets:
The data is contained in three files:
<br />
portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
profile.json - demographic data for each customer
transcript.json - records for transactions, offers received, offers viewed, and offers completed
<br />
## Data understanding:
<br />
### portfolio.json:
id (string) - offer id
offer_type (string) - type of offer ie BOGO, discount, informational
difficulty (int) - minimum required spend to complete an offer
reward (int) - reward given for completing an offer
duration (int) - time for offer to be open, in days
channels (list of strings)
<br />
### profile.json:
age (int) - age of the customer
became_member_on (int) - date when customer created an app account
gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
id (str) - customer id
income (float) - customer's income
<br />
### transcript.json:
event (str) - record description (ie transaction, offer received, offer viewed, etc.)
person (str) - customer id
time (int) - time in hours since start of test. The data begins at time t=0
value - (dict of strings) - either an offer id or transaction amount depending on the record
<br />
## Problem Statement:
What is the Gender Distribution of Starbucks Customers?
What is the Age Distribution of Starbucks Customers?
What is the Income Distribution of Starbucks Customers?
How many customers enrolled yearly?
Which gender has the highest yearly membership?
Which gender has the highest Annual income?
What is the distribution of event in transcripts?
What is the percent of trasactions and offers in the event?
What is the Income Distribution for the Offer Events?
What are the Offer types amongst ages, gender and income groups?
