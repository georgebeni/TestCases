# Test Cases

Bellow are some of my test cases.

Also, you can check my [Bugs Report](https://docs.google.com/spreadsheets/d/1yuCr51GCLYAWpRpcpPQ1gcHglSZefNNS3Ji_xgW6Fwg/edit?usp=sharing) on Google Sheets.

---

## Test Case #1

**Description**
* This test case will verify the login functionality of the application.

**Steps to reproduce**
1. Launch the application.
2. Enter valid username.
3. Enter valid password.
4. Click on the _Login_ button.

**Expected result**
* The user should be successfully logged into the application and redirected to the main dashboard.

**Actual result**
* The user is successfully logged in.
* The user is redirected to the main dashboard.

**Test data**
* Username: test
* Password: test1234

---

## Test Case #2

**Description**
* Check if the login works when a person uses a correct and incorrect username & password.

**Steps to reproduce**
1. Go to www.example.com/login.
2. * Add a correct username and password.
   * Add an incorrect username and password. 
3. Press _Login_ button.

**Expected result**
* **Case #1:** User should logged in successfully to website.
* **Case #2:** User shouldn't logged in to website.

**Actual result**
* **Case #1:** User logged in successfully to website.
* **Case #2:** User couldn't logged in to website because the username or/and password are incorrect.

**Test data**
* **Case #1: Correct username and password**
  - Username: test
  - Password: test1234
* **Case #2: Incorrect username and password**
  - Username: wrong_test
  - Password: wrong_test1234

---

## Test Case #3

**Description**
* Verify if the user can successfully pay the products using a valid credit card.

**Steps to reproduce**
1. Go to https://www.shop-example.com.
2. Log in to the site.
3. Add the products to the cart.
4. Press the _Cart_ button.
5. Select credit card option for payment.
6. Provide the valid credit card details.
7. Pay for products.

**Expected result**
* User should be able to purchase successfully the products using the credit card without any error.

**Actual result**
* User couldn't purches the producs and a message error is displaed: "Credit card is expired. Please try again and insert a valid credit card."

**Test data**
* Username: test
* Password: test1234
* Cart products: Covor antiderapant, Pantofi sport de piele, Minge de fotbal
* Credit card details
  - First Name: Ion
  - Last Name: Popescu
* Credit card number: 1234-5678-9012-3456
* Payment Type: Visa
* Expiration Date: 03/2021
* CVV: 098

---

## Test Case #4

**Description**
* Test if the search bar works.

**Steps to reproduce**
1. Go to https://www.google.com.
2. Click on the search bar and search for different thinks.
3. Press _Enter_ key or click on _Google Search_ button.
4. See the results.

**Expected result**
* User should be able to search thinks using Google search bar.

**Actual result**
* User can search on internet using Google search bar.

**Test data**
* Search data:
  - Cat
  - Learn QA
  - How to recover Facebook password
  - Differences between Europe and Asia
  - How long is the Great Wall of China

---

## Test Case #5

**Description**
* Verify if the loggin function works when is inset SQL syntax in Username or Password field.

**Steps to reproduce**
1. Go to https://www.example.com/login.
2. Insert SQL syntax in username or password field.
3. Press _Login_ button.

**Expected result**
* User shouldn't logged in.
* User should see an error message like this: **Username or/and password wrong! Try again**.

**Actual result**
* User couldn't logged in.
* User see an error message: **Username or/and password wrong! Try again**.

**Test data**
* SQL Injection Syntax: **_SELECT * FROM users WHERE username=’username’ and password=’password’ or 1=1--+_**
