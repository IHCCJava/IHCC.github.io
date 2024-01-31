# Longaberger Project Part 2 - Validations
This is an update to your Longaberger project that will add validations to all of the inputs and error handling to all your parse methods.

For an example of input validations, if the user tries to select "X" as the basket type, the program should prompt that X is not one of the accepted values for basket type, and prompt for the basket type again. This will require if/else or switch statements, and loops. You will do this for ALL inputs.

## Longberger class updates
1. Validate all user input (Order Type, Basket Type, Accessory Type, State, Customer Type and
further processing of Y/N).
2. Create a loop for each user input validation requiring the user to input valid data. Display an
error message each time invalid data is entered.
3. Every parse method you use should be wrapped in a try/catch statement for error handling.

## BasketBuild class has no updates this time

## Rubric

This project is graded on features and functionality added for this revision.

|Topic| Task| Points|
|-----|-----|------|
|**Input Validations**| All user inputs are validated for correct values. If an incorrect value is provided, an error is displayed and the program asks for the input again. | 15|
| | Some user inputs are validated, but not all and/or not using looping structure to reprompt the user | 8|
| |  User inputs are not being validated | 0|
|**Error Handling** | All parse methods are wrapped in a try/catch statement to catch any potentional runtime errors and display an error to the user | 15 |
|| Some parse methods have try/catch statements, but not all and/or try/catch was attempted but not working all the way | 8|
|| Try/catch error handling was not used, or used incorrectly | 0|
| **Total** | | 30|