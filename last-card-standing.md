# Last Card Standing

**Difficulty: Medium**

## Background

A normal deck of cards contains 52 cards. Each card has a value and a suit, and there is one card of each possible combination in the deck. The suits are called Clubs, Hearts, Spades and Diamonds and the values in each suit are (in ascending order): Ace, 2, 3, 4, 5, 6, 7, 8, 9, Ten, Jack, Queen and King. We will refer to the cards using the first letter of the value (or a digit) followed by the first letter of the suit. E.g. 4S for the "four of spades", TH for the "ten of hearts" and KD for the "king of diamonds".

Imagine a deck of 52 cards which is initially grouped by suit (i.e. all Clubs together) and sorted ascending in the orders of suit and value given above.

E.g.
AC, 2C, 3C, ... KC, AH, 2H, ...

For this exercise, you are going to write a program to "throw away" cards from the deck according to a sequence, until only one card remains. 

## The Program

Read **all** of the points below before you begin. Write a program which:

 0. Accepts as input a single integer (1 to 999), `n`
 1. Takes, initially, the sorted deck from above as the "pile"
 2. Iterates through the cards in the pile
 3. Discards `n` cards, keeps 1, and proceeds until it reaches the end of the pile
 4. Takes as its new pile the cards which were **kept** in the previous iteration
 5. Repeats from Step 2 (using the same value of `n`)
 6. Continues until only one card remains
 7. Outputs the name of the last remaining card using the notation given in the "Background" section
 
Notes:

 * When the number `n` is greater than the number of cards left to process in the deck, then `n` should "fold over" back to the start of the deck as many times as necessary until a card can be selected
 * The output in step 7 should be the only output of the program
 * Your program may or may not loop in its entirety (up to you)
 * You may wish to add a pause (or keypress) after the final output to stop the program from exiting immediately
 
## Example Runs