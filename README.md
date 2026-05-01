# Test Suite: Sign Up

## Test Case 1: Successful Registration
- **Test Case ID:** TC_Signup_01  
- **Description:** Register with valid data  
- **Pre-condition:** Email does not exist in the system  
- **Priority:** High  

### Test Steps:
1. Click **Sign in**
2. Click **Create one**
3. Enter valid full name
4. Enter valid email
5. Enter password
6. Confirm password
7. Click **Create Account**

### Result:
- User successfully created  

**Status:** Passed  

---

## Test Case 2: Registration with Duplicate Email
- **Test Case ID:** TC_Signup_02  
- **Description:** Registration should fail with existing email  
- **Pre-condition:** Registration page is open  
- **Priority:** High  

### Test Steps:
1. Enter an already existing email
2. Fill other fields with valid data
3. Click **Create one**

### Result:
- “Email already in use” message is not shown  
- New user is created  

**Status:** Failed  

---

## Test Case 3: Confirm Password Validation
- **Test Case ID:** TC_Signup_03  
- **Description:** Error shown when passwords do not match  
- **Pre-condition:** Registration page is open  
- **Priority:** High  

### Test Steps:
1. Enter password: `123456`
2. Enter different confirm password
3. Click **Create one**

### Expected Result:
- “Passwords do not match” message should appear  

### Actual Result:
- Message not shown  
- Registration completed  

**Status:** Failed  

---

## Test Case 4: Email Format Validation
- **Test Case ID:** TC_Signup_04  
- **Description:** Email format validation  
- **Pre-condition:** Registration page is open  
- **Priority:** High  

### Test Steps:
1. Enter invalid email (e.g., `gmail@com`)
2. Fill other fields
3. Click **Create one**

### Result:
- Registration fails  
- “Invalid email” message displayed  

**Status:** Passed  

---

# Test Suite: Sign In

## Test Case 5: Login with Valid Credentials
- **Test Case ID:** TC_Signin_05  
- **Description:** User logs in successfully with correct credentials  
- **Pre-condition:** User is registered  
- **Priority:** High  

### Test Steps:
1. Click **Sign in**
2. Enter valid email
3. Enter valid password
4. Click **Sign in**

### Result:
- User logged in successfully  
- Redirected to homepage  

**Status:** Passed  

---

## Test Case 6: Login with Incorrect Password
- **Test Case ID:** TC_Signin_06  
- **Description:** Error shown for wrong password  
- **Pre-condition:** User is registered  
- **Priority:** High  

### Test Steps:
1. Click **Sign in**
2. Enter valid email
3. Enter incorrect password
4. Click **Sign in**

### Result:
- Error message not shown  
- User redirected to homepage  

**Status:** Failed  

---

## Test Case 7: Login with Empty Fields
- **Test Case ID:** TC_Signin_07  
- **Description:** Login attempt with empty fields  
- **Pre-condition:** User is registered  
- **Priority:** High  

### Test Steps:
1. Click **Sign in**
2. Leave fields empty
3. Click **Sign in**

### Result:
- Validation messages displayed  

**Status:** Passed  

---

# Test Suite: Profile

## Test Case 8: Display Profile Information
- **Test Case ID:** TC_Profile_08  
- **Description:** Profile data displayed correctly  
- **Pre-condition:** User logged in  
- **Priority:** High  

### Test Steps:
1. Open profile page  

### Result:
- Email displayed correctly  
- Other information incorrect  

**Status:** Failed  

---

## Test Case 9: Update Profile Information
- **Test Case ID:** TC_Profile_09  
- **Description:** User updates profile successfully  
- **Pre-condition:** User logged in  
- **Priority:** High  

### Test Steps:
1. Open profile page
2. Update fields with valid data  

### Result:
- Shipping address not updated  

**Status:** Failed  

---

## Test Case 10: Invalid Format Update
- **Test Case ID:** TC_Profile_10  
- **Description:** Invalid inputs should not be accepted  
- **Pre-condition:** User logged in  
- **Priority:** High  

### Test Steps:
1. Enter invalid email format
2. Click **Save changes**

### Result:
- No error message  
- Data updated incorrectly  

**Status:** Failed  

---

# Test Suite: Cart

## Test Case 11: Add Product to Cart
- **Test Case ID:** TC_Cart_11  
- **Description:** User can add product to cart  
- **Pre-condition:** Products page is open  
- **Priority:** High  

### Test Steps:
1. Open products page
2. Click **Add to Cart**

### Result:
- Product added to cart  

**Status:** Passed  

---

## Test Case 12: Update Product Quantity
- **Test Case ID:** TC_Cart_12  
- **Description:** User can change quantity  
- **Pre-condition:** Cart page is open  
- **Priority:** High  

### Test Steps:
1. Open cart
2. Increase/decrease quantity  

### Result:
- Total price updated  

**Status:** Passed  

---

## Test Case 13: Remove Product from Cart
- **Test Case ID:** TC_Cart_13  
- **Description:** User can remove product  
- **Pre-condition:** Cart page is open  
- **Priority:** High  

### Test Steps:
1. Open cart
2. Click **Remove**

### Result:
- Product removed  
- Total price updated  

**Status:** Passed  

---

## Test Case 14: Price Calculation
- **Test Case ID:** TC_Cart_14  
- **Description:** Cart calculates total correctly  
- **Pre-condition:** Products added to cart  
- **Priority:** High  

### Test Steps:
1. Add multiple products
2. Apply discount coupon  

### Result:
- Total price incorrect  

**Status:** Failed  

---

# Test Suite: Home Page

## Test Case 15: Homepage Load
- **Test Case ID:** TC_Homepage_15  
- **Description:** Homepage loads successfully  
- **Pre-condition:** URL is opened  
- **Priority:** Critical  

### Test Steps:
1. Enter URL  

### Result:
- Page loads successfully  

**Status:** Passed  

---

## Test Case 16: Search Functionality
- **Test Case ID:** TC_Homepage_16  
- **Description:** Search works correctly  
- **Pre-condition:** Homepage is open  
- **Priority:** High  

### Test Steps:
1. Enter keyword in search bar
2. Press Enter  

### Result:
- Relevant product not shown  

**Status:** Failed  
