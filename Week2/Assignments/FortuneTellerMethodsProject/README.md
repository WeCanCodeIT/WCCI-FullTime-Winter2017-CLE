# FortuneTellerMethod
## Due: Tuesday, January 17th by 9:30 AM

## Overview
Develop a console application that will tell the user’s fortune based on data received from the user, using Methods to 
process the user's input.

## Tasks

### Part 1 - This is the same as your last FortuneTeller, so this part of the project should already be done.
- [ ] Ask the user for the user’s first name
- [ ] Ask the user for the user’s last name
- [ ] GREET the user (see Part 2)
- [ ] Ask the user for the user’s age
- [ ] Ask the user for the user’s birth month (as an 'int')
- [ ] Ask the user for the user’s favorite ROYGBIV color
  - [ ] If the user does not know what ROYGBIV is, ask them to enter “Help” to get a list of the ROYGBIV colors
- [ ] Ask the user for the number of siblings the user has

### Part 2
- [ ] Create a Method that greets the user
  - [ ] This user should take two 'string' parameters (such as first name and last name)
  - [ ] This Method should return a 'string'
  - [ ] When this method is used, it should print to the console "Greetings, ______ _______. I will tell you your fortune!"
   - [ ] example: "Greetings, Daniel Vivacqua. I will tell you your fortune!"
- [ ] Create a Method that calculates the number of years before the user retires
  - [ ] If the user’s age is an odd number, then they will retire in ____ years, or ___ years if their age is an even number.
  - [ ] This method must have an 'int' as a parameter (such as the user's age) and must return an 'int' representing the number of years before retirement to the Main method
- [ ] Create a Method that determines the vacation home of the user.
  - [ ] If the user’s number of siblings is 0, then they will have a vacation home in ___(location), or 1 then they will have a vacation home in ___(location), or 2 then they will have a vacation home in ___ (location), or 3 then they will have a vacation home in ___ (location), or more than 3 then they will have a vacation home in ____ (location). If the user enters anything other than a number greater than or equal to 0, they should get a bad vacation home!
  - [ ] This method must take an 'int' as a parameter (such as the user's number of siblings) and return a 'string' of the vacation home's location.
- [ ] Create a Method that determines the user's future mode of transportation
  - [ ] Depending on which ROYGBIV color is the user’s favorite, they will have a specific mode of transportation (i.e. car, boat, plane, etc.) 
  - [ ] If the user enters anything other than a ROYGBIV color, their mode of transportation should be a squeaky shopping cart.
  - [ ] This method should take a 'string' as a parameter (such as the user's favorite color) and return a 'string' of the mode of transportation.
- [ ] Create a Method that determines how much money the user will have when they retire.
  - [ ] If the user’s birth month is 1-4, they will have $____ in the bank; if the user's birth month is 5-8, they will have $____ in the bank; and if it is 9-12, then they will have $____ in the bank. If the user enters something other than 1-12 as their birth month, they will have $0.00 in the bank.
  - [ ] This method should take an 'int' as a parameter (such as birth month) and return a 'double' of their bank account amount.
- [ ] Create a Method that judges how good the fortune is.
 - [ ] This method should take no parameters.
 - [ ] This method should be return type 'void'.
 - [ ] This method should tell the user what the fortune teller thinks of the fortune. Pick a phrase of your choosing.
  - [ ] example: "Oooh! That's a good fortune!" or "Well, I think that was the weirdest fortune I've ever told!"
  - [ ] hint: Don't overthink it.
- [ ] Allow the user to quit the program at any point where the program is looking for user input.
- [ ] Allow the user to restart the program at any point where the program is looking for user input.

### Part 3
- [ ] The user should be greeted after entering their name.
- [ ] The user’s fortune should be written as such:
  - [ ] [First Name] [Last Name] will retire in [# of Years] with [Amount of Money] in the bank, a vacation home in [Location] and a [Mode of Transportation].
- [ ] The user should then receive a judgment on their fortune printed to the console.
- [ ] Program should be able to handle whether or not a user inputs capital or lowercase letters.

### Optional Extension Challenge:
- [ ] Create a single Method that allows the user to either quit or restart the program at any point where the program is looking for user input.
- [ ] Create an overloaded Method that allows the user to pick their two favorite colors, and give them a special mode of transportation based on color combinations.
- [ ] Determine which of the methods in this project could be converted to 'void' methods, and write out those 'void' methods below the rest of your code, commented out with "//"


### Project Submission
[GitHub Submission Link](https://docs.google.com/forms/d/e/1FAIpQLSflEACBLrqMgfuHadVrfQtk7GSDyThJ-J0oHMPjFZjQg1Vcpw/viewform)
