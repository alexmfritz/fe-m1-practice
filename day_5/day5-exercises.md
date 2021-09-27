## Chapter 2 (Statements, Variables, Data Types, & Arrays):

1. How do you declare a variable. What does the equals sign really mean in JavaScript? What is it called in JavaScript?
  - You declare a variable in JavaScript by using the JS keyword 'var' followed by the name of the variable using CamelCase naming convention, following by assigning it a value of various datatypes.
    * ex: var name = 'Alex' means I assigned the variable name to a String value of Alex
  - An equal sign is called an ~~assignment operator~~ in JavaScript, and it's telling the computer you are going to assign a value to the variable you are declaring. It is also used to *update* the value given to a variable
  - If variables have not been assigned a value, the value is defaulted to undefined.

2. There are three big data types in JavaScript: numbers, strings, and booleans. Describe what each of them are:
  - Numbers: Anything assigned a numerical or integer value. Numbers can hold positive and negative values. A special kind of Number is called a float and that means it is a decimal value.
  - Strings: Any characters, numbers, or symbols encased in quotation or tick marks. Strings are typically used to hold statements or pass information.
  - Booleans: Assign a variable a value of true or false

3. What are the six rules for naming variables? What are a few JavaScript reserved words that you should avoid using for variable names?
  1. The name must begin with a letter, dollar sign ($), or an underscore. It may *NOT* begin with a number
  2. The name can contain letters, numbers, dollar sign ($), or underscores (_). The name should not contain dashes (-) or periods (.)
  3. You cannot use keywords or reserved words (var, let, const)
  4. All variables are case sensitive (ex: score and Score would be different), but it is *bad* practice to create to variables with same name w/ different cases
  5. Always use a name that describes the information that the variable stores
  6. If the variable name is made up of more than one word, use camelCase

4. How can an array be useful when dealing with multiple related values? How do you access/change a value in an array?
  - An array can be used to store multiple related values within the same variable (var colors = ['red', 'blue', 'green']). This is useful when you do not know how many items a list will contain because you do not need to declare how many values an array will hold
  - In JavaScript, an array is a zero-indexed variable, meaning the first value located in the array is placement 0. To access a value within an array (otherwise known as an "element"), you will call that variable w/ the location of the value. (ex: colors[0]; would call the value 'red' in the above array)
  - If you wanted to reassign the final item in the colors array, you would do something like this: color[2] = purple;

5. What is the difference between an expression and a statement?
  - Expression: evaluates (results in) a **single** value.
    * Expression 1: Assigns a single datatype to a variable
    * Expression 2: Uses two or more previously declared variables to result in a single new one
    * Expressions rely on ~~operators~~, allowing programmers to create a single value from one or more values
  - Statement: anything that instructs the computer or program to do something
    * Declaring a variable or function is a statement (var total), whereas a statement expression would be var total = 0

6. What are three types of operators and how are they used?
  - Operators are used to help create a single value out of many values
  - Assignment operator: assigns a value to a variable
  - Arithmetic operator: performs basic math
  - String operator: combines two strings
  - Comparison operator: compares two values and returns true or false
  - Logical operator: combine expressions and returns true or false

### Exercises: Variables

##### The Fortune Teller

`console.log("You will be a " + jobTitle + " in " + geoLocation + ", married to " + partnerName + " with " + numberOfChildren + " kids.");`

  - Expected output: "You will be a Marine Biologist in Seattle, married to Leslie with 4 kids.""

##### The Age Calculator
`var currentYear = 2021;
var birthYear = 1993;
var wrongAge = currentYear - currentYear;
var rightAge = currentYear - birthYear;
console.log("You are either " + rightAge + " or " + wrongAge);`

  - Expected output: "You are either 28 or 0"

##### The Lifetime Supply Calculator
`var currentAge = 28;
var maxAge = 93;
var amtPerDay = 7;
var total = (maxAge - currentAge) * (amtPerDay * 365);
console.log("You will need " + total + " to last you until the ripe old age of " + maxAge);`

  - Expected output: "You will need 166075 to last you until the ripe old age of 93"
