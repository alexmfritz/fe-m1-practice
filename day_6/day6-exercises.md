## Chapter 3 (Functions & Scope)


1. If we have a function defined as function sayHello(){console.log("Hello!")}, what is the difference between entering sayHello and sayHello() in the console?
  - Because sayHello() is a function, the parenthesis need to follow the functionName when naming or calling it because a function has the opportunity to take parameters/arguments. If you do not include the parenthesis you are simply referencing the function which means it will not perform the code block of statements within it.

2. What is the difference between function parameters and arguments?
  - Parameters are the variables assigned within the function parenthesis when you declare the function. These variables act as containers of information for when you pass an argument later when you call the function. The argument will be used when the function is called, meaning that argument information/data will be mapped to those parameter variables

3. What is the keyword return used for?
  - When you have statements made within the function that will process information and you need that new information give back to you, the keyword *return* will be used and the information passed back will be the *return value*

4. How are local variables better than global variables? Are there instances you can think of where you might want to use a variable that is globally scoped over local?
  - Local variables (aka function-level variables) are better than global variables because they are created only for the purpose of running the function and then removed after the function has run. If you need to run multiple similar functions using the same variable names, you will not run into any problems.
  - When using global variables, the benefit is that you will be able to use that variable anywhere else in your code through out your webpage but you will not be able to reuse the name of that variable again.
  - If you have an object for your hotel listed on a travel booking site, you will have properties assigned to that object instance that hold values for both the total number of rooms and the number of rooms booked. You can create a method within the object that will calculate the number of available rooms left in the hotel and you can return that value in a global variable and use that number through out the site.

  `function tellFortune(children, partner, location, job) {
  console.log(`You will be a ${job} in ${location}, married to ${partner} with ${children} kids!`)
}
tellFortune(15, "John", "Florida", "pool cleaner");
tellFortune(1, "Harold", "Texas", "politician");
tellFortune(0, "Rebecca", "Hawaii", "SCUBA instructor");

function calculateAge(birthYear, currentYear) {
  var age = currentYear - birthYear;
  console.log(`You are either ${age} or ${age - 1}`);
}
calculateAge(1974, 2021);
calculateAge(1993, 2021);
calculateAge(743, 831);

function calculateSupply(age, amt) {
  var maxAge = 95;
  var total = (maxAge - age) * (amt * 365);
  console.log(`You will need ${total} to last you until the ripe old age of ${maxAge}`);
}
calculateSupply(28, 3);
calculateSupply(13, 5.5);
calculateSupply(82, 3);`
