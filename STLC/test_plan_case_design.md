# Grocery Online Webshop Test Cases

## 1. Register and Login Functionality

### Test Design Techniques: 
- Equivalence Partitioning (EP)
- Boundary Value Analysis (BVA)
- Error Guessing

### Test Cases:

#### 1.1 EP: Valid Registration
- **Test Case:** Verify registration with valid details (name, email, password).
- **Input:** Name = "John Doe", Email = "john@example.com", Password = "Password@123"
- **Expected Outcome:** User registration successful.

#### 1.2 BVA: Password Boundary Check
- **Test Case:** Verify registration with a password that is exactly at the minimum limit (8 characters).
- **Input:** Password = "P@sswrd1"
- **Expected Outcome:** User registration successful.

#### 1.3 BVA: Password Below Minimum Length
- **Test Case:** Verify registration fails when password is below the minimum length (7 characters).
- **Input:** Password = "P@sswd1"
- **Expected Outcome:** Error message: "Password must be at least 8 characters."

#### 1.4 EP: Invalid Email Format
- **Test Case:** Verify registration fails when an invalid email format is used.
- **Input:** Email = "johnexample.com"
- **Expected Outcome:** Error message: "Please enter a valid email address."

#### 1.5 Error Guessing: Missing Mandatory Fields
- **Test Case:** Verify registration fails when mandatory fields (e.g., password) are left blank.
- **Input:** Password = (empty)
- **Expected Outcome:** Error message: "Password is required."

---

## 2. Searching, Sorting, and Filtering Products

### Test Design Techniques:
- Use Case Testing
- Equivalence Partitioning (EP)

### Test Cases:

#### 2.1 Use Case: Product Search
- **Test Case:** Verify that users can search for products by name.
- **Input:** Search for "Apple".
- **Expected Outcome:** Products related to "Apple" are displayed.

#### 2.2 EP: Sort Products by Price
- **Test Case:** Verify that products can be sorted by price (low to high).
- **Input:** Sort by price.
- **Expected Outcome:** Products displayed in ascending order by price.

#### 2.3 EP: Filter by Category
- **Test Case:** Verify that users can filter products by a specific category (e.g., "Fruits").
- **Input:** Select category "Fruits".
- **Expected Outcome:** Only products from the "Fruits" category are displayed.

---

## 3. Product Rating System

### Test Design Techniques:
- Boundary Value Analysis (BVA)
- Error Guessing

### Test Cases:

#### 3.1 BVA: Valid Rating Submission
- **Test Case:** Verify that users can submit a 5-star rating with valid feedback.
- **Input:** 5 stars, feedback: "Great product!"
- **Expected Outcome:** Rating and feedback are saved successfully.

#### 3.2 Error Guessing: Rating Submission Without Purchase
- **Test Case:** Verify that only users who purchased a product can submit a rating.
- **Input:** Unpurchased product, attempt to rate.
- **Expected Outcome:** Error message: "You must purchase the product to leave a review."

#### 3.3 BVA: Feedback Length Validation
- **Test Case:** Verify that feedback cannot exceed 500 characters.
- **Input:** Feedback with 501 characters.
- **Expected Outcome:** Error message: "Feedback cannot exceed 500 characters."

---

## 4. Age Verification for Alcoholic Products

### Test Design Techniques:
- Equivalence Partitioning (EP)
- Error Guessing

### Test Cases:

#### 4.1 EP: Valid Age Input
- **Test Case:** Verify that users above 18 can access alcoholic products.
- **Input:** Birthdate = "01/01/2000" (Age = 24)
- **Expected Outcome:** Access to alcoholic products category granted.

#### 4.2 EP: Underage Access Denied
- **Test Case:** Verify that users under 18 are denied access to alcoholic products.
- **Input:** Birthdate = "01/01/2010" (Age = 14)
- **Expected Outcome:** Access denied, user is redirected to homepage.

#### 4.3 Error Guessing: Invalid Date Format
- **Test Case:** Verify behavior when invalid date format is entered in the age verification modal.
- **Input:** Birthdate = "32/13/2000"
- **Expected Outcome:** Error message: "Invalid date format. Please use DD/MM/YYYY."

---

## 5. Shipping Cost Calculation

### Test Design Techniques:
- Boundary Value Analysis (BVA)
- Use Case Testing

### Test Cases:

#### 5.1 BVA: Free Shipping Threshold
- **Test Case:** Verify that orders of €20 or more qualify for free shipping.
- **Input:** Order total = €20
- **Expected Outcome:** Free shipping applied.

#### 5.2 BVA: Shipping Fee Applied
- **Test Case:** Verify that orders below €20 incur a shipping fee of €5.
- **Input:** Order total = €19.99
- **Expected Outcome:** Shipping fee of €5 applied.

#### 5.3 Use Case: Display Shipping Cost During Checkout
- **Test Case:** Verify that shipping costs are displayed during the checkout process.
- **Input:** Proceed to checkout with an order total of €15.
- **Expected Outcome:** Shipping cost of €5 is displayed during checkout.
