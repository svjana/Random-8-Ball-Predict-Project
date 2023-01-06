# Random-8-Ball-Predict-Project
This code creates a "magic 8 ball" program that will ask a user for their name, and then ask them a question. It will then generate a random number between 0 and 7 (inclusive), and use that number to determine a response from the magic 8 ball. The response will be printed to the console.


// Random 8 Ball Predict Project //

let userName = "Babai"; // Create a variable to store the user's name

// Print "Hello, [userName]!" if the user's name is provided, or "Hello!" if not
userName ? console.log(`Hello, ${userName}!`) : console.log("Hello!");

let userQuestion = "Today's day?"; // Create a variable to store the user's question

// Print "${userName} has asked - ${userQuestion}"
console.log(`${userName} has asked - ${userQuestion}`);

// Generate a random number between 0 and 7 (inclusive) using Math.random() and store it in a variable
let randomNumber = Math.floor(Math.random() * 8);

// Print the value of randomNumber
console.log(randomNumber);

let eightBall = " "; // Create a variable to store the magic 8 ball's response

// Use a switch statement to determine the magic 8 ball's response based on the value of randomNumber
switch (randomNumber) {
  case 0:
    eightBall = "It is certain.";
    break;
  case 1:
    eightBall = "It is decidedly so.";
    break;
  case 2:
    eightBall = "Reply hazy, try again.";
    break;
  case 3:
    eightBall = "Cannot predict now.";
    break;
  case 4:
    eightBall = "Do not count on it.";
    break;
  case 5:
    eightBall = "My sources say no.";
    break;
  case 6:
    eightBall = "Outlook not so good.";
    break;
  case 7:
    eightBall = "Signs point to yes.";
    break;
}

// Print the magic 8 ball's response
console.log(`The magic 8 ball's answer: ${eightBall}`);
