Explanation in Words
1️⃣ HTML Structure
<input type="number" id="guess" placeholder="Enter your guess">
This is where the player types their guess.
<button onclick="checkGuess()">Guess</button>
When the player clicks this button, it runs the checkGuess() function.
<p id="message"></p>
This paragraph shows messages like “Too high” or “Correct!”
2️⃣ JavaScript Part
const secretNumber = Math.floor(Math.random() * 100) + 1;
Generates a random number between 1 and 100 that the player has to guess.
function checkGuess() { ... }
This function checks the player’s guess:
const userGuess = Number(document.getElementById('guess').value);
Gets the value typed by the user and converts it to a number.
Compares userGuess with secretNumber:
If equal → display “Correct!”
If lower → display “Too low!”
If higher → display “Too high!”
If invalid → display “Enter a valid number.”# game
