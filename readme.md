# ⛽ QA Fill Tank: Automated Refueling Logic Validation

> ### A comprehensive unit testing suite built with **Jest** to validate the core business logic of the "Mate Royal Oil" automated refueling system.

This repository serves as a professional showcase of **Software Quality Assurance (QA) and Unit Testing** practices in JavaScript. It demonstrates how to translate complex business requirements into robust, automated test cases using techniques like Boundary Value Analysis (BVA) and Equivalence Class Partitioning (ECP).

---

## 🎯 Project Overview

The objective of this project is to test the `fillTank` function. This function handles the automated refueling transaction, calculating how much fuel to dispense and how much money to withdraw from the customer's account based on dynamic constraints.

### The System Under Test (SUT)
The `fillTank` function accepts three parameters:
1. `customer` (Object) - Contains account balance and vehicle details.
2. `fuelPrice` (Number) - The price per 1 liter of fuel.
3. `amount` (Number, Optional) - The requested amount of fuel.

**Customer Object Structure:**
```javascript
const customer = {
  money: 3000, // Account balance
  vehicle: {
    maxTankCapacity: 40, // Maximum fuel tank volume
    fuelRemains: 8,      // Current fuel in the tank
  }
}
