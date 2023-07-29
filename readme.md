# Weekend Assignment: Car Marketplace Management System

## **Objective:**

Your task is to create a JavaScript program that manages a car marketplace. This system should be able to handle different entities such as car agencies, customers, and a tax authority. The car marketplace data will be provided to you. All actions will be executed with console outputs.

## Requirements:

Your JavaScript program should be able to perform the following functionalities:

1. **Agency Operations:**

   - Search for a car agency by its name or ID.
   - Retrieve all agencies' names.
   - Add a new car to an agency's inventory.
   - Remove a car from an agency's inventory.
   - Change the cash or credit of an agency.
   - Update the price of a specific car in an agency (Method: `updateCarPrice`).
   - Calculate and return the total revenue for a specific agency (Method: `getTotalAgencyRevenue`).
   - Transfer a car from one agency to another (Method: `transferCarBetweenAgencies`).

2. **Customer Operations:**

   - Search for a customer by their name or ID.
   - Retrieve all customers' names.
   - Change the cash of a customer.
   - Calculate the total value of all cars owned by a specific customer (Method: `getCustomerTotalCarValue`).

3. **Car Operations:**

   - Retrieve all cars available for purchase.
   - Search for cars based on certain criteria. The search parameters should include the production year, price, and optionally, the brand of the car.
   - Return the most expensive car available for sale (Method: `getMostExpensiveCar`).
   - Return the cheapest car available for sale (Method: `getCheapestCar`).

4. **Car Purchase Operations:**

   - Implement a `sellCar` function that sells a car to a specific customer. This function should:
     - Check the availability of the car at the agency.
     - Verify if the customer has enough cash to purchase the car.
     - Update the cash and credit for both the agency and the customer accordingly.
     - Update the tax authority's records.
   - Calculate and return the total revenue of the entire market (Method: `getTotalMarketRevenue`).

    ### Instructions for handling taxes:

     - a. Subtract the vehicle amount + 17% (tax) from the customer's cash.
     - b. Add the vehicle value to the car agency cash.
     - c. Change the car owner's id to the customer's id.
     - d. Remove the car from the array of the agency's car models.
     - e. Add the car to the client cars array.

     Taxes Authority:

     - f. Pay 17 percent of the vehicle value to the tax authority. (add the amount to totalTaxesPaid)
     - g. Increase the number of transactions made in one (numberOfTransactions)
     - h. Add the vehicle amount + tax to sumOfAllTransactions
     - Check that there is the requested vehicle at the agency in not return 'The vehicle does not exist at the agency'
     - Check that the customer has enough money to purchase the vehicle, if not return 'The customer does not have enough money'

## Notes:

- Make sure to handle possible edge cases, for example, when a car or a customer doesn't exist, or when a customer doesn't have enough cash to buy a car.
- Remember to break down your code into manageable and logically separated functions for better readability and maintainability.
- Comment your code appropriately to describe the functionality of your methods.

Good luck!
