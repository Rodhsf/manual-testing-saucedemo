# Test Cases - SauceDemo

---

## TC001 - Login with success

**Preconditions:**  
User is on the login page  

**Test Data:**  
- Username: standard_user  
- Password: secret_sauce  

**Steps:**
1. Enter username  
2. Enter password  
3. Click the "Login" button  

**Expected Result:**  
User is successfully redirected to the products page  

**Status:**  
Pass  

---

## TC002 - Login with incorrect password

**Preconditions:**  
User is on the login page  

**Test Data:**  
- Username: standard_user  
- Password: 1234  

**Steps:**
1. Enter a valid username  
2. Enter an invalid password  
3. Click the "Login" button  

**Expected Result:**  
System displays an error message and does not allow login  

**Status:**  
Fail  

---

## TC003 - Login with empty fields

**Preconditions:**  
User is on the login page  

**Test Data:**  
- Username: empty  
- Password: empty  

**Steps:**
1. Access the login page  
2. Leave the username and password fields empty  
3. Click the "Login" button  

**Expected Result:**  
System displays a required fields error message and does not allow login  

**Status:**  
Fail  

---

## TC004 - Login with locked out user

**Preconditions:**  
User is on the login page  

**Test Data:**  
- Username: locked_out_user  
- Password: secret_sauce  

**Steps:**
1. Enter the username  
2. Enter the password  
3. Click the "Login" button  

**Expected Result:**  
System does not allow login and displays an error message indicating that the user is locked out  

**Status:**  
Fail  

---

## TC005 - Add product to cart

**Preconditions:**  
User is logged in  

**Test Data:**  
- Product: Sauce Labs Backpack  

**Steps:**
1. Locate the product "Sauce Labs Backpack"  
2. Click the "Add to cart" button  

**Expected Result:**  
Product is added to the cart and the cart counter is updated correctly  

**Status:**  
Pass  

---

## TC006 - Add multiple products to cart

**Preconditions:**  
User is logged in  

**Test Data:**  
- Product 1: Sauce Labs Backpack  
- Product 2: Sauce Labs Bolt T-Shirt  

**Steps:**
1. Locate the product "Sauce Labs Backpack"  
2. Click the "Add to cart" button  
3. Locate the product "Sauce Labs Bolt T-Shirt"  
4. Click the "Add to cart" button  

**Expected Result:**  
Both products are added to the cart and the cart counter is updated to reflect the correct quantity  

**Status:**  
Pass  

---

## TC007 - Remove product from cart

**Preconditions:**  
Product is already added to the cart  

**Test Data:**  
- Product: Sauce Labs Backpack  

**Steps:**
1. Locate the product "Sauce Labs Backpack" in the cart  
2. Click the "Remove" button  

**Expected Result:**  
Product is removed from the cart and the cart counter is updated accordingly  

**Status:**  
Pass  

---

## TC008 - Checkout with valid data

**Preconditions:**  
Product is already added to the cart  

**Test Data:**  
- First Name: John  
- Last Name: Doe  
- Postal Code: 12345  

**Steps:**
1. Access the cart  
2. Click the "Checkout" button  
3. Enter first name, last name, and postal code  
4. Click the "Continue" button  
5. Click the "Finish" button  

**Expected Result:**  
User is redirected to the confirmation page and a success message is displayed  

**Status:**  
Pass  

---

## TC009 - Checkout with empty fields

**Preconditions:**  
Product is already added to the cart  

**Test Data:**  
- First Name: empty  
- Last Name: empty  
- Postal Code: empty  

**Steps:**
1. Access the checkout page  
2. Leave all required fields empty  
3. Click the "Continue" button  

**Expected Result:**  
System displays an error message for required fields and does not allow the user to proceed  

**Status:**  
Fail  

---
