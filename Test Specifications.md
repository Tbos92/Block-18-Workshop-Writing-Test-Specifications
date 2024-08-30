# Block-18-Workshop-Writing-Test-Specifications

Unit Tests:
A function called "multiplication" that returns the product of the two input numbers.
- Expect multiplication inputs to be 2+ nums
- Expect multiplication product(2,3) to be a number
- Expect multiplication product(2,3) to be 6
- Expect multiplication product("a",2) to be an error
- Expect if odd # of inputs are (-) for multiplication product to be -(num)
- Expect if even # of inputs are (-) for multiplication product to be +(num)
- Expect if multiplying ints for multiplication output to be greater than inputs
- Expect if any number of inputs is 0 for multiplication output to be = 0

A function called "concatOdds" takes two arrays of integers as arguments. It should return a single array that only contains the odd numbers, in ascending order, from both of the arrays.
- Expect concatOdds inputs = arrays of ints
- Expect concatOdds to loop over each of the input arrays
- Expect concatOdds (4%2) to be equal to 0 (i.e. an even num)
- Expect concatOdds (3%2) to be equal to 1 (i.e. an odd num)
- Expect concatOdds for any (int%2 equals 1) ints to be pushed into a new array
- Expect concatOdds for any (int%2 equals 1) ints to be checked against the new array
- Expect concatOdds for any (int%2 equals 1) ints found to already be in the new array not to be pushed again


Functional Tests:
A shopping cart checkout feature that allows a user to check out as a guest (without an account), or as a logged-in user. They should be allowed to do either, but should be asked if they want to create an account or log in if they check out as a guest.
- In the upper-right corner of the shopping have a log-in button option for the user to login in advance of checking out
- When the user opens their shopping cart present them with a checkout button at the bottom of their cart
- Display the subtotal of all items in the cart before the user selects chekout
- If the user is not logged in when they select the checkout button, prompt them with the option to log in or continue as a guest for checkout
- The log in option should also include a create an account prompt if they are not already signed up for an account
- The user should be able to add items to their cart while shopping
- The user should be able to edit (increase, decrease, remove) the number of a specific item in their cart from the cart itself
- Allow user to move items in their cart to a "save for later section"
- If user is guest or their account does not have saved information, prompt user with form to complete for shipping and billing information
- Until all required information is entered, the user should not be allowed to select the submit/finalize transaction button
- If user account has shipping and billing information, autofill default but allow user to update this information if they would like to change any of it
- Once the user has selected checkout and has either logged in or continued as guest, calculate taxes and shipping
- Allow user to select shipping speed/options if applicable
- Once all required user information/selections are entered, activate submit/finalize transaction button for user to select
- Once user selects submit/finalize transaction button, forward user to a "success" page with order confirmation, order  #, and tracking information if available
- Internally, this should also trigger the server to send an email to the user with the order confirmation information for their records
- Once fully checked out, the cart should be updated by clearing all purchased items from the active cart
