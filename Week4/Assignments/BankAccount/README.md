#Bank Account Project
##Directions
You will be designing a console application to manage a client’s bank account. For now, the application will have only one client that is hard-coded into the system.

##Tasks
###Menu Items
- [ ] View Client Information
- [ ] View Account Balance
  - [ ] Checking Account Balance
  - [ ] Reserve Account Balance
  - [ ] Savings Account Balance
- [ ] Deposit Funds
- [ ] Withdraw Funds
- [ ] Exit

###Checking Account Class
- [ ] Inherits Account base class
- [ ] Minimum 2 fields
- [ ] Minimum 2 properties
- [ ] Minimum 1 constructor

###Reserve Account Class
- [ ] Inherits Account base class
- [ ] Minimum 2 fields
- [ ] Minimum 2 properties
- [ ] Minimum 1 constructor

###Savings Account Class
- [ ] Inherits Account base class
- [ ] Minimum 2 fields
- [ ] Minimum 2 properties
- [ ] Minimum 1 constructor

###Objects
- [ ] Minimum 1 object instantiated from the Checking Account Class
- [ ] Minimum 1 object instantiated from the Reserve Account Class
- [ ] Minimum 1 object instantiated from the Savings Account Class

###Other Required Tasks
- [ ] Use StreamWriter to create account summary files that track transactions **for each account type (each type has its own text file)**. Files should be located in the Debug Folder and should include:
  - [ ] Name of Client
  - [ ] Client Account Number
  - [ ] Account Type (Checking, Reserve, or Savings)
  - [ ] Each transaction should be on its own line
  - [ ] Each transaction should show date and time of transaction (must use DateTime Class)
  - [ ] Each transaction should show a “+” for deposit and a “-” for withdrawal
  - [ ] Each transaction should show the transaction amount
  - [ ] Each transaction should show the new current balance after the transaction

### Stretch Tasks

With the current tasks persistence is not a requirement. Implementing persistence with FileWriter would make the program reusable for tracking balances.

Right now this program is designed for one user. Giving the ability to enter a user name when the program begins would make the program useful for multiple users. At this point do not worry about trying to add passwords. That is outside of the scope of what we know at this point. Letting the users log in with only their names _is_ less secure, but we're focused on functionality right now.

## Hints

Persistence is not required. Meaning each time you run the program all of the values can reset.

You can choose any starting balance to begin the program with.



-  * [Submission Link](https://docs.google.com/forms/d/e/1FAIpQLSdoPHuQpvwxiBW2dVW8_nTOqvKDP8OfqZ87hn2fz4QKDcRjTg/viewform)
