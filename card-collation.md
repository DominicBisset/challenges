# Card Collation

## Background

A normal deck of cards contains 52 cards. Each card has a value and a suit, and there is one card of each possible combination in the deck. The suits are called **Clubs, Hearts, Spades and Diamonds** and the values in each suit are (in ascending order): **Ace, 2, 3, 4, 5, 6, 7, 8, 9, Ten, Jack, Queen and King**. We will refer to the cards using the first letter of the value (or a digit) followed by the first letter of the suit. E.g. `4S` for the "four of spades", `TH` for the "ten of hearts" and `KD` for the "king of diamonds". There are no jokers in this deck.

For this exercise, you are going to write a program in **pseudocode on paper**, to output cards from a standard deck in a certain order.

## A note about Pseudocode

Pseudocode isn't a particular language but can take after any language you are familiar with. Your code will be acceptable as long as the intent of your program is clear and you don't cut corners at the expense of clarity. For example, you could write a `for` or `for each` loop in the style of C, BASIC, or Python and it will be understood. You can write in a functional language style if you want to.

Your language should have consistent characteristics throughout (don't mix `If-Then-EndIf` with `for () {}`). You don't need to use proper language APIs for input and output, you can use anything which is clear, for example `int n = input()` or `writeline(myString)`.

## The Program

Read **all** of the points below before you begin. Write a program which:

 0. Accepts as input a single integer (0 to 52), called `n`
 1. Outputs the first `n` cards from the deck described in "Background", initially **collated by suit**
     + Collation (or grouping) by suit means, for example, that all Clubs are together
	 + Sorted ascending by suit, then value (in the orders given in "Background")
	 + E.g. `AC, 2C, 3C, ... KC, AH, 2H, ...` (one per line)
 2. After `n` cards have been output, the collation changes to **collate by value**
     + For example, cards after the `n`th card will have all like values together (all `2`s together, then all `3`s together)
	 + Output the remaining cards in the deck, sorted ascending by value, then suit (in the orders given in "Background")
     + Any cards which would otherwise be skipped because of the change in collation should be output (see "Example Runs")
	 + Example of the collation: `AC, AH, AS, AD, 2C, 2H, 2S, 2D, 3C, ...` (one per line)
 3. Outputs every card exactly once
 4. Outputs one card per line (see "Example Runs")
 5. Quits after writing all 52 cards to screen
 
Notes:

 * The program should not produce any output other than those described above
 * The program should not accept or require any input other than those described above

## Example Runs

### Run 1

	> 16
	AC
	2C
	3C
	4C
	5C
	6C
	7C
	8C
	9C
	TC
	JC
	QC
	KC
	AH
	2H
	3H
	AS
	AD
	2S
	2D
	3S
	3D
	4H
	4S
	4D
	5H
	5S
	5D
	6H
	6S
	6D
	7H
	7S
	7D
	8H
	8S
	8D
	9H
	9S
	9D
	TH
	TS
	TD
	JH
	JS
	JD
	QH
	QS
	QD
	KH
	KS
	KD
	
### Run 2

	> 30
	AC
	2C
	3C
	4C
	5C
	6C
	7C
	8C
	9C
	TC
	JC
	QC
	KC
	AH
	2H
	3H
	4H
	5H
	6H
	7H
	8H
	9H
	TH
	JH
	QH
	KH
	AS
	2S
	3S
	4S
	AD
	2D
	3D
	4D
	5S
	5D
	6S
	6D
	7S
	7D
	8S
	8D
	9S
	9D
	TS
	TD
	JS
	JD
	QS
	QD
	KS
	KD
	
## End of challenge

Please submit your written program on a piece of paper with your name