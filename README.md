Download Link: https://assignmentchef.com/product/solved-number-guessing-game-computer-as-guessing-role
<br>
<h1>OVERVIEW</h1>

In this assignment, you are going to design and develop an interactive number-guessing game.  One participant (as host) is asked to pick a fixed length number (as secret number) and another participant (as game-player) is to guess the chosen number repeatedly.  In the beginning of each game, a secret number is first picked by the host with no repeated digits, then repeatedly prompt the “game-player” for a “guess” of the secret number, without repeated digits.  In return after each guess, the game-player will be given some feedbacks about the guess.  Based on the feedback, the game-player continues to guess until the secret number is correctly guessed or the maximum number of attempts is reached.




The feedback provided to the game-player by the host contains 2 pieces of information as follows:

<ol>

 <li>How many of the digits in the “guess” also appear in the “secret number” (as Correct)</li>

 <li>How many of the digits from “Correct” appear in the same position as secret number’s (as Exact)</li>

</ol>




For instances, say the chosen secret number is “2468”, the following table shows the feedback as a result of each guess provided by the game-player:




<table width="534">

 <tbody>

  <tr>

   <td width="60">Guess</td>

   <td width="66">Correct</td>

   <td width="60">Exact</td>

   <td width="348">Remark</td>

  </tr>

  <tr>

   <td width="60">1357</td>

   <td width="66">0</td>

   <td width="60">0</td>

   <td width="348">None of the digits (1,3,5 &amp; 7) are from 2468</td>

  </tr>

  <tr>

   <td width="60">2890</td>

   <td width="66">2</td>

   <td width="60">1</td>

   <td width="348">Only digits 2 &amp; 8 appear in 2468 and digit 2 is in the exact position</td>

  </tr>

  <tr>

   <td width="60">8294</td>

   <td width="66">3</td>

   <td width="60">0</td>

   <td width="348">Only digits 2, 4 &amp; 8 appear in 2468 and none of 3 digits appear in the exact position</td>

  </tr>

  <tr>

   <td width="60">2486</td>

   <td width="66">4</td>

   <td width="60">2</td>

   <td width="348">All digits from “guess” also from 2468 and only digits 2 &amp; 4 appear in the exact position</td>

  </tr>

  <tr>

   <td width="60">2468</td>

   <td width="66">4</td>

   <td width="60">4</td>

   <td width="348">Guess matches secret number</td>

  </tr>

 </tbody>

</table>




You are asked to design and develop a program to be the guessing role.   In other words, the computer program as “game player” makes the guess and you as “host” provides the computer program with the feedback interactively.







<strong>              </strong>

<h1>SCOPE</h1>




<ol>

 <li>You are free to implement your program for 3-digit or 4-digit guessing, in python.</li>

 <li>In the beginning of each game, indicate to the host the number of digits your program is designed to guess.</li>

 <li>Inform the host to choose a “secret number” with no repeated digits and have it written down somewhere.</li>

 <li>Prompt “host” to start the game</li>

 <li>Your program as “game-player” starts to guess, after each guess, prompt “host” for feedback as described in the “Overview” session:

  <ol>

   <li>How many correct digits?</li>

   <li>How many exact digits? (skip this question if Correct is 0)</li>

  </ol></li>

 <li>Your program is required to verify the responses returned by the “host”. If needed, repeatedly prompt “host” to re-enter the correct information, such examples as:

  <ol>

   <li>Non-numeric responses</li>

   <li>Value of “Exact” is greater than that of “Correct”</li>

   <li>Value of either “Correct” or “Exact” should be less than the length of the secret number</li>

  </ol></li>

</ol>

(3 or 4)

<ol>

 <li>Inconsistent responses</li>

</ol>

<ol start="7">

 <li>Feedback History

  <ol>

   <li>Keep a list of history of all guesses including corresponding feedback, and then display the entire list after each guess in chronological order</li>

  </ol></li>

 <li>Termination

  <ol>

   <li>the current guess matches the secret number</li>

   <li>In this case, display a congratulation message</li>

   <li>the number of guess attempts reaches the limit</li>

   <li>Display a game-over message</li>

   <li>the host enters “x” on any of the 2 feedback (Correct or Exact)</li>

  </ol></li>

 <li>Termination Prompt

  <ol>

   <li>After termination, prompt “host” to quit or to continue a new game.</li>

  </ol></li>

 <li>Game Startup

  <ol>

   <li>Show a welcome message to briefly describe what your program does</li>

   <li>Then prompt “host” for the secret number prior to starting the game</li>

  </ol></li>

 <li>For 3-digit number implementation, your program MJST successfully guessed the secret number within 20 attempts.</li>

 <li>For 4-digit number implementation, your program MJST successfully guessed the secret number within 40 attempts.</li>

</ol>

<u>TARTUP </u><u>O</u><u>PTIONS</u>




Not applicable




<h1>SKILLS</h1>




In this assignment, you will be trained on the use of the followings:




<ul>

 <li>Use input() to prompt user for information</li>

 <li>Use standard objects (strings, numbers &amp; lists)</li>

 <li>Control statements to interact with users</li>

 <li>Variable Scope</li>

 <li>String formatting (method style)</li>

 <li>Functions for program structure and decomposition</li>

</ul>







<h1>DELIVERABLES</h1>




<ol>

 <li>Design documentation (A1_School_StudentID_Design.doc)</li>

 <li>Program source code (A1_School_StudentID_Source.py)</li>

 <li>Output (A1_School_StudentID_Output.doc)</li>

</ol>




Zip all files above in a single file (A1_School_StudentID.zip) and submit the zip file by due date to the corresponding assignment folder under “Assignment (submission)”

For instances, a SME student with student ID “119010001”:

    A1_SME_119010001.zip:

o A1_SME_119010001_Design.doc o A1_SME_119010001_Source.py o A1_SME_119010001_Output.doc

5% will be deducted if any files are incorrectly named!!!

<strong>              </strong>

<h1>DESIGN DOCUMENTATION</h1>




For the design document provide write-up for the following 2 chapters:

<ol>

 <li>Design:</li>

 <li>Describe your strategy for guessing</li>

 <li>Describe the core data structures used for tracking the guess history and feedback</li>

 <li>Describe the structure of the program (functions, variables and program flow) 2. Test Strategy:</li>

 <li>How to verify that your program works as per “Scope” – create a test plan</li>

 <li>Describe different plans for different scenarios</li>

</ol>




<h1>TIPS &amp; HINTS</h1>




<ul>

 <li>Format the feedback for each guess using format() (number guessed, correct : xx, position: xx)</li>

 <li>Use a list to keep all previous guesses &amp; feedback as strings</li>

 <li>Beware of variable scope as you might keep a few variables as global such as guess results and guess count.</li>

 <li>Refer to python website for program styles and naming convention (PEP 8)</li>

 <li>Try a guessing algorithm (solution) with a simple strategy in 2 parts. The first part is to determine all the correct digits (not concerning the position); then the second part simply takes the digits form part I and reorders them to match the secret number.</li>

 <li>Split up the digits in logical groups and make first guess attempt for each group. Based on different feedback, identify the digit(s) that is part of the secret number or not.  Use the result discovered to sequentially determine the remaining digits one by one.  Once all required digits are discovered, simply shuffle the digits until a correct guess is achieved.</li>

 <li>Gradually optimize your guessing solution with results from “part I” to make “part II” more efficient.</li>

</ul>




<strong>              </strong>




<h1>OUTPUT SUCCESSFUL GUESS</h1>

<strong> </strong>

<h2>SECRET NUMBER = 487</h2>

Guess 1/15: 123

How many correct digits? 0




Guess 1/15: 123 Correct=0 Exact=0




Guess 2/15: 490

How many correct digits? 1

How many exact digits? 1




Guess 1/15: 123 Correct=0 Exact=0

Guess 2/15: 490 Correct=1 Exact=1




Guess 3/15: 478

How many correct digits? 3

How many exact digits? 1




Guess 1/15: 123 Correct=0 Exact=0

Guess 2/15: 490 Correct=1 Exact=1

Guess 3/15: 478 Correct=3 Exact=1




Guess 4/15: 487

How many correct digits? 3

How many exact digits? 3




Congratulations!! Start a new game (y/n)?




<strong>               </strong>

<h1>OUTPUT INCORRECT FEEDBACK</h1>




<h2>SECRET NUMBER = 487</h2>

Guess 1/15: 123

How many correct digits? 4

Incorrect feedback, must be &lt; 4 How many correct digits?







<h2>SECRET NUMBER = 487</h2>

Guess 1/15: 123

How many correct digits? 1

How many exact digits? 2

Incorrect feedback, exact digit must be &lt;= 1!

How many exact digits?







<strong>              </strong>

<h1>OUTPUT EXCEEDING GUESS LIMIT</h1>




<h2>SECRET NUMBER = 487</h2>

Guess 1/15: 123

How many correct digits? 0




Guess 1/15: 123 Correct=0 Exact=0




Guess 2/15: 490

How many correct digits? 1

How many exact digits? 1




Guess 1/15: 123 Correct=0 Exact=0

Guess 2/15: 490 Correct=1 Exact=1




Guess 3/15: 491

How many correct digits? 1

How many exact digits? 1




Guess 1/15: 123 Correct=0 Exact=0

Guess 2/15: 490 Correct=1 Exact=1

Guess 3/15: 491 Correct=1 Exact=1

Guess 4/15: 431

How many correct digits? 1

How many exact digits? 1




.

.

.

.

.

.




Guess 15/15: 413




Game Over!! Exceeded max. attempts! Start a new game (y/n)?




<strong>       </strong>