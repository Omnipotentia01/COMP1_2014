#Task Sheet 1
##Task 3a Questions
###Question One:
1. Which function is responsible for getting the name from the user?
2. The function responsible for this is the GetPlayerName() function. 
###Question Two:
1. How will you ensure that the user is asked for the name repeatedly?
2. I will add a Validity loop that will not end until a correct input is recieved.
###Question Three:
1. What additional variable will you need and what will its datatype be?
2. A variable named Valid; it will be a boolean.

###Write the function metioned in PsudoCode;
  
Try Then
Function GetPlayerName()
ValidName < Boolean
PlayerName < String
While ValidName == FALSE Then
    OUTPUT "Enter Your Name"
    INPUT PlayerName
    IF PlayerName >= 2 AND <= 16 THEN
        ValidName = True
    Except TypeError Then
        OUTPUT "Invalid Name, Please Try Again!"
call GetPlayerName()
Return PlayerName
END Function

##Task 3b Questions
###Question One:
1. Which function is responsible for adding scores to the table?
2. The function responsible is UpdateRecentScores(RecentScores, Score)

##Task 5 Questions
###Question One:
1. Which Module needs to be added?
2. datetime (import datetime)
###Question Two:
1. Identify the four functions that will require changes.
2. 
###Question Three:
1. How do you convert a string in the format DD/MM/YY (e.g. 14/08/93) to a date type in Python?
2. 