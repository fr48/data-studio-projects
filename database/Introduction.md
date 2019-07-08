# So Your Email Has Been Stolen...

We hear a lot about data breaches, about a company exposing our email addresses or IP addresses. We heave a sigh of relief that it was "just" email addresses or IP addresses. Our passwords and financial data wasn't in danger. This project starts off with a very basic form of OSINT: what kind of information can attackers find just starting off with the humble email address?

## Research Questions

* I randomly grabbed the dumps off the internet without much searching. Where are these people located?

* I know what kind of social media accounts these people have. Which is the most common social media account they are using?

* Most of these people have been involved in at least one breach. What is the largest data breach for this data set? What was stolen in that breach?

## Database Schema

I am using DataFrames to conceptualize my "tables" for my database

There are  tables (using the filenames as my table names):

* maintable: email address, ip address, longitude and latitude

* breaches: name of site breached, domain, date of breach, number of records stolen, and a list of all stolen items

* pwned: email address, breached site the address was in
(correlates to both maintable and breaches)

* reputation: email address, and all social media accounts (youtube, spotify, pinterest, etc)

* profiles: email addres, social media 

The primary keys, but not enforced, is the email address.
