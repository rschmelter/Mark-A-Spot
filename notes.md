steps

1. A user can sign up and select and add countries and cities they've been to.
2. A user can also add cities to certain countries. 
3. A user can add cool spots that they've found in the cities they've visited
4. A user can select a category for the cities they've visited


A user has_many counties
A user has_many cities through countries 
A user has_many spots through cities

A category has_many spots
A spot has_many categories 
A user has_many categories through spots
A city has_many categories


Models:

Users
Countries
Cities
Spots
Categories

Users:
Name
password_digest

Countries:
Name:

Cities:
Name
user_id
Country_id

Spots:
Name
Description
Rating

Category:
Name:
