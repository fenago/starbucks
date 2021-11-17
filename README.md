# starbucks

## Introduction:
This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. Not all users receive the same offer, and that is the challenge to solve with this data set.
<br />
## Data Sets:
The data is contained in three files:
<br />
portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.) <br />
profile.json - demographic data for each customer <br />
transcript.json - records for transactions, offers received, offers viewed, and offers completed<br />
<br />
## Data understanding:
<br />
### portfolio.json:
id (string) - offer id<br />
offer_type (string) - type of offer ie BOGO, discount, informational<br />
difficulty (int) - minimum required spend to complete an offer<br />
reward (int) - reward given for completing an offer<br />
duration (int) - time for offer to be open, in days<br />
channels (list of strings)<br />
<br />
### profile.json:<br />
age (int) - age of the customer<br />
became_member_on (int) - date when customer created an app account<br />
gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)<br />
id (str) - customer id<br />
income (float) - customer's income<br />
<br />
### transcript.json:<br />
event (str) - record description (ie transaction, offer received, offer viewed, etc.)<br />
person (str) - customer id<br />
time (int) - time in hours since start of test. The data begins at time t=0<br />
value - (dict of strings) - either an offer id or transaction amount depending on the record<br />
<br />
## Problem Statement:<br />
What is the Gender Distribution of Starbucks Customers?<br />
What is the Age Distribution of Starbucks Customers?<br />
What is the Income Distribution of Starbucks Customers?<br />
How many customers enrolled yearly?<br />
Which gender has the highest yearly membership?<br />
Which gender has the highest Annual income?<br />
What is the distribution of event in transcripts?<br />
What is the percent of trasactions and offers in the event?<br />
What is the Income Distribution for the Offer Events?<br />
What are the Offer types amongst ages, gender and income groups?<br />
