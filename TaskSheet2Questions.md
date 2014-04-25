#Task Sheet 2
##Task 6 Questions
###Question One:
1. Where would be a good place in the program to keep track of whether the ace is high or not? Remember that the aces' value will be set before a game is started and it will not change for the duration of the game.
2. This should be set as a global variable at the beginning of the program. It should be written in all capitals so that it is clear later on and other programmers that it is a global variable.
###Question Two:
1. Name the function that will need to be altered so that `5. Options` is part of the main menu.
2. The `DisplayMenu()` function.
###Question Three:
1. Name the function that will need to be modified so that card value comparisons will work correctly now that aces can be either high or low.
2. The function is `GetRank(RankNo)`

##Pseudo-Code
	FUNCTION DisplayOptions()
		Ace <- Options.Ace
		OUTPUT ''
		OUTPUT 'OPTIONS'
		OUTPUT ''
		OUTPUT '1. Ace: ', Ace
		OUTPUT ''
		OUTPUT 'Select an option or press q to quit: '
	END FUNCTION

	FUNCTION GetOptionChoice()
		Choice <- INPUT ''
		Choice <- CALL lower(Choice)
		OUTPUT ''
		Choice <- Choice[1]
		RETURN Choice
	END FUNCTION

	FUNCTION SetOptions(OptionChoice):
		IF OptionChoice = '1' THEN
			CALL SetAceHighOrLow()
		END IF
	END FUNCTION

	FUNCTION SetAceHighOrLow():
		OUTPUT ''
		OUTPUT 'Would you like the ace to be high or low? '
		Finished = False
		WHILE NOT Finished DO
			Choice <- INPUT ''
			OUTPUT ''
			Choice <- CALL lower(Choice)
			Choice <- Choice[1]
			IF Choice = 'h' THEN
				Options.Ace <- 'high'
				Finished = TRUE
			ELSE IF Choice <- 'l' THEN
				Options.Ace <- 'low'
				Finished = TRUE
			ELSE
				OUTPUT 'Please input a valid choice'
			END IF
		END WHILE
	END FUNCTION
