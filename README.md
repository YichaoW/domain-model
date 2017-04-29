# domain-model
Info 449 Assignment

Make the Unit Tests Pass

- clone the repo at https://TedNeward@bitbucket.org/TedNeward/uwsimpledomainmodel.git (Links to an external site.)Links to an external site.

- this consists of:

SimpleDomainModel: "standard" command-line project
SimpleDomainModelTests: set of unit tests exercising the above
- as written, the tests will not pass; it won't even compile!

- your job: make the tests pass!

WITHOUT changing them!

Create a value type: Money

- Properties:

amount
currency
- Methods:

convert: convert from one currency to another

add, subtract: do the math thing

- Currencies are converted at the following exchange rate:

1 USD = .5 GBP (2 USD = 1 GBP)

1 USD = 1.5 EUR (2 USD = 3 EUR)

1 USD = 1.25 CAN (4 USD = 5 CAN)

you'll have to work out the rest of the math on your own

- If you use a String for currency, make sure that only the four listed are accepted

- Note that it is totally acceptable to add/subtract GBP to EUR or CAN

meaning, you'll need to convert when adding/subtracting

Create a class: Job

- Properties:

title
salary
- Salaries can be either per-hour or per-year

- Methods:

calculateIncome, which should accept a number of hours worked this year
if this is a per-year salary, then ignore the hours

raise, which will bump up the salary by the passed amount
Create a class: Person

- It have the following properties:

firstName
lastName
age
job (Job)
spouse (Person)
- Methods:

display a string representation of Person (toString())
- Note that if the Person is under age 16, they cannot have a job

- Note that if the Person is under age 18, they cannot have a spouse

Create a class: Family

- Properties:

members (a collection of Persons)
- Methods:

initializer: take two Persons, make sure they each have no spouse, set spouse to each other
householdIncome: return the combined income of the entire family
haveChild: add a new Person to the collection of age 0
there must be one Person in the family who is over age 21 to be legal

Rubric
