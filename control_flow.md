#Javascript Control Flow Exercises

###1. Nightclub Bouncer

Using an if/else expression, create a script that prompts the user for their age, then:

  * If the user is older than 18, he/she should receive a message that he/she may enter.
  * If the user is younger than 18, then he/she can't enter and should receive a message telling him/her that he/she's too young.
  * If the user is between 18 and 21, he/she should receive a message that he/she can enter, but not drink.
  * If the user is older than 21, he/she should receive a message that he/she can both enter and drink.

var age = 14;

if(age < 18) {
      bouncer = "You gotta go home, kid";
  } else if(age >= 21) {
      bouncer = "C'mon In!";
  } else {
      bouncer = "No Drinking";
  }

bouncer

###2. Grade.js
Output the following letter grade from a variable with a test score. 

Based on the user input, display either "A", "B", "C", "D", or "F", for a score that is an integer between 0 and 100. Try and use a `switch` statement.

var testScore = 60;

switch(testScore) {
  case 100:
    grade = "A";
    break;
  case 90:
    grade = "B";
    break;
  case 80:
    grade = "C";
    break;
  case 70:
    grade = "D";
    break;
  case 60:
    grade = "F";
    break;
  default:
    grade = "null";
}

###3. Fizz Buzz (Bonus, uses loops)
Write a small program that asks a user for a number. If it's a multiple of 3, output 'fizz.' If it's a multiple of 5, output 'buzz.' If it's a multiple of 3 and 5, output 'Fizzbuzz.' 


for (var i = 0; i < 100; i++) {
  if((i % 3 === 0) && (i % 5 === 0)) {
    console.log("Fizzbuzz");
  } else if(i % 3 === 0) {
    console.log("Fizz");
  } else if(i % 5 === 0) {
    console.log("Buzz");
  } else {
    console.log(i);
  }
}

###4. EXTRA BONUS! (Not required, but give it the college try!)

- There is an event where guests will be sitting in three sections based on their names: "left," "middle," and "right." If they have a premium ticket, they can sit in first `3` rows in their section; otherwise they can take any seat behind row 3. Using hardcoded variables for `name` and `ticketType`, print out appropriate seating instructions.

- There is an event with ticket prices that are `$50,' `$65,' `$85` for standard, premier, and premier plus (for drinks) seating. Seniors, veterans, and students receive a `$10` discount, while standard patrons receive no discount. Based on hardcoded variables for `ticketType` and `discountType,' print out a patron's `ticketPrice.'
