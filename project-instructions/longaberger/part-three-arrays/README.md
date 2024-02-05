# Longaberger Project Part 3 - Arrays
This is the final update to your longaberger project that will add arrays to store correct data for input validations and calculations.

## Longberger class updates
1. Add a loop to the main method that asks the user if they have another basket to process (Y/N).
2. Create Hard-Coded Arrays for the following information.
    - Basket Type
    - Accessory Code
3. Validate user input for the Basket Type using the hard-coded array
4. Validate user input for the Accessory Code using the hard-coded array

## BasketBuild class updates

1. Create Hard-Coded Arrays for the following information:
    - Literal values are the display values to the user, whereas type and code are the values we use internally. Example, "C" is the Basket Type, and "Cracker" is the Basket Literal
    - Basket Type
    - Basket Literal
    - Basket Cost
    - Accessory Code
    - Accessory Literal
    - Accessory Cost
    - Customer Type Literal
    - Discount Percentage
2. Search the basket type array for a match to the user input to find the array index for the basket type. Use this array index to access the basket literal and the basket cost arrays.
3. Search the accessory code array for a match to the user input to find the array index for the accessory code. Use this array index to access the accessory literal and accessory cost arrays.
4. Use the customer type as the array index to access the customer type literal and discount percentage arrays. (Remember arrays start with 0! Adjust accordingly)
5. Calculation methods should use the cost array values.
6. Display method should use the literal array values.

## Rubric

This project is graded on features and functionality added for this revision.

|Topic| Task| Points|
|-----|-----|------|
|**Hard-coded arrays Longaberger class** | Hard-coded arrays added for Basket Type and Accessory Code inside the Longaberger class| 10 |
|| Only one array was added and/or arrays not setup correctly | 5|
|| Basket Type and Accessory Code arrays missing inside Longaberger class | 0|
|**Input is validated against arrays**| Basket type and accessory code inputs are now validated against the values inside the hard-coded arrays | 10|
| | Only one input is validated against values in the arrays and/or the validation is not reading from the array correctly | 5|
| |  Arrays are not being used for basket type and accessory code validations | 0|
|**Hard-coded arrays BasketBuild class** | All eight hard-coded arrays are created in the BasketBuild class| 10 |
|| Some arrays are missing inside BasketBuild and/or arrays are not setup correctly | 5|
|| Arrays are missing from BasketBuild class | 0|
|**Array usage** | Arrays inside the BasketBuild class are being used correctly to determine cost for calculations, and literal values for display using the indexes | 10 |
|| Some arrays are being utilized for either calculations or displaying and/or the arrays are not being utilized correctly | 5|
|| Arrays are not utilized to lookup values to calculate costs or display literals | 0|
| **Total** | | 40|
