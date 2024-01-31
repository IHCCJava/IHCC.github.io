# Longaberger Project
This program will ask for order type, basket specifications, customer type and customer information. It will calculate the total cost which includes sales tax. Output will be displayed on the console.

## The Longaberger class should contain the following

1. Comments should be at the top of this and all programs. Should have a description of the program’s purpose, your name and date. Also place additional comments on lines to clarify what you are doing if needed.
2. Use descriptive names for variables.
3. Use the Scanner or JOptionPane classes for input and/or display.
4. Request the order type from the user. Order type of (S)tandard should use the default constructor. Order type of (C)ustom should request user input for basket type, accessory type, state and customer type
5. All invalid entries should be assigned the default values given for the default constructor
6. Place entered data into a Basket object, based on the order type
7. Call the calculate method in your BasketType object to get the total
8. After calculations, display all input and calculated data in a receipt format with the current date

## The BasketBuild class should contain the following

1. Create a class called BasketBuild.java inside src/main/java/com.longaberger
2. Use private instance variables for input and calculated values.
3. Create getters and setters for the basket type, accessory type, customer type and state
4. Write a default constructor that sets the following values:
    - char Basket Type – U
    - String Accessory Type – A4
    - int Customer Type – 1
    - String State - IA
5. Write a parameterized constructor that takes all the values for basket type, accessory type, customer type and state
6. Write an instance method to calculate the basket amount, subtotal, discount, sales tax and total bill
    - Basket Amount = Basket Cost + Accessory Cost
    - Discount = Basket Amount * Customer Discount Rate
    - Subtotal = Basket Amount – Discount
    - Tax = Subtotal * Tax Rate
    - Total Cost = Subtotal + Tax
        - Dealers DO NOT pay sales tax.
7. Write an instance method to return a formatted string for the receipt

## The BasketBuildTests class should contain the following

1. Under the src directory, create a test/java directory
2. In the test/java folder create the com.longaberger package
3. Inside the test/java/com.longaberger create a class called BasketBuildTests.java
4. Write at least three unit tests to test the calculation method inside BasketBuild
  - Test scenarios should include variations in basket type, accessories, type of customer, etc

## Data for calculations

You'll need the following information to take your inputs and run your calculations.

| Basket Type    | Basket Cost | 
|----------------|-------------|
| C = Cracker    | $15.00      |
| W = Wildflower | $53.25      |
| K = Key        | $23.15      |
| M = Magazine   | $34.20      |
| U = Umbrella   | $112.77     |

| Accessory      | Accessory Cost |
|----------------|----------------|
| A1 = Protector | $4.75          |
| A2 = Liner     | $8.00          | 
| A3 = Combo     | $10.55         |
| A4 = None      | $0.00          |

| State | State Tax Rate |
|-------|----------------|
| IA    | 6%             |
| IL    | 6.25%          |
| MO    | 4.225%         |

| Customer Type | Customer Discount |
|---------------|-------------------|
| 1             | Dealer 50%        |
| 2             | Walk In 0%        |
| 3             | Bus 10%           |

## Rubric

This project is graded on functionality (does it compile, can the user create a basket and get the correct cost). It is also graded on features added in the instructions, like including the correct methods, constructors, data conversions, and tests.

|Topic| Task| Points|
|-----|-----|------|
|**Longaberger class**| Longaberger class includes a logic branch for Standard vs Custom order, input methods, creates a BasketBuild object, and calls instance methods on the object to display proper values | 12|
| | Longaberger class includes only some of the required features and/or features are not working | 5|
| |  Longaberger class does not compile | 0|
|**BasketBuild class** | BasketBuild class includes both constructors, getters/setters, calculation and output methods | 12 |
|| BasketBuild class missing some of the required features and/or features are not working | 5|
|| BasketBuild class does not compile | 0|
|**Calculations** | Calculation method is inside the BasketBuild class. Calculations take into account all the variations of cost based on user input, and outputs the correct cost | 11 |
|| Calculation method is included, but is in the wrong class and/or missing code to produce correct calculations | 5|
|| Calculation method is not implemented | 0|
| **Total** | | 35|