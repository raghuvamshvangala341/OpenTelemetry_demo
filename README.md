# E-Commerce Test Cases

## TC_01

- **Scenario ID:** SC_01
- **Test Type:** Positive
- **Severity:** Critical
- **Test Case Description:** Verify product can be added to cart successfully
- **Test Steps:**
  - 1. Open the e-commerce application.
  - 2. Select a product (e.g., Roof Binoculars).
  - 3. Select quantity 1.
  - 4. Click Add To Cart.
  - 5. Open the cart and verify the product.
- **Test Data:** Roof Binoculars; Quantity: 1
- **Expected Result:** Product should be added to cart with correct name, quantity, and price.
- **Actual Result:** Not Executed

---

## TC_02

- **Scenario ID:** SC_02
- **Test Type:** Positive
- **Severity:** High
- **Test Case Description:** Verify cart quantity update recalculates item total and order total
- **Test Steps:**
  - 1. Open the application and add a product to cart.
  - 2. Open the Shopping Cart page.
  - 3. Change the product quantity from 1 to 2.
  - 4. Observe item total and overall total.
- **Test Data:** Roof Binoculars; Quantity: 2
- **Expected Result:** Quantity should update to 2 and totals should be recalculated accurately.
- **Actual Result:** Not Executed

---

## TC_03

- **Scenario ID:** SC_03
- **Test Type:** Positive
- **Severity:** High
- **Test Case Description:** Verify currency selection updates displayed product prices
- **Test Steps:**
  - 1. Open the application.
  - 2. Note a product price in the default currency.
  - 3. Open the currency dropdown.
  - 4. Select another available currency (e.g., INR).
  - 5. Verify product price display.
- **Test Data:** Currency: USD → INR
- **Expected Result:** Prices should be displayed in the selected currency with the correct converted value.
- **Actual Result:** Not Executed

---

## TC_04

- **Scenario ID:** SC_04
- **Test Type:** Positive
- **Severity:** Critical
- **Test Case Description:** Verify checkout can place an order with valid payment details
- **Test Steps:**
  - 1. Add a product to the cart.
  - 2. Open the cart and proceed to checkout/payment.
  - 3. Enter valid card details and expiry information.
  - 4. Enter a valid CVV.
  - 5. Click Place Order.
- **Test Data:** Demo card details shown by the application
- **Expected Result:** Order should be accepted and a confirmation/success response should be displayed.
- **Actual Result:** Not Executed

---

## TC_05

- **Scenario ID:** SC_05
- **Test Type:** Positive
- **Severity:** High
- **Test Case Description:** Verify Empty Cart clears all cart items
- **Test Steps:**
  - 1. Add two products to the cart.
  - 2. Open the Shopping Cart page.
  - 3. Click Empty Cart.
  - 4. Verify cart contents and cart count.
- **Test Data:** Two products in cart
- **Expected Result:** All items should be removed; cart should show empty state and zero items.
- **Actual Result:** Not Executed

---

## TC_06

- **Scenario ID:** SC_06
- **Test Type:** Negative
- **Severity:** Critical
- **Test Case Description:** Verify checkout blocks invalid or incomplete payment details
- **Test Steps:**
  - 1. Add a product to the cart.
  - 2. Proceed to checkout/payment.
  - 3. Clear or enter an invalid card number.
  - 4. Leave CVV blank or enter an invalid value.
  - 5. Click Place Order.
- **Test Data:** Card number: invalid; CVV: blank/invalid
- **Expected Result:** Order must not be placed; validation error should be shown and cart should remain intact.
- **Actual Result:** Not Executed

---

## TC_07

- **Scenario ID:** SC_07
- **Test Type:** Negative
- **Severity:** High
- **Test Case Description:** Verify application rejects an invalid quantity selection
- **Test Steps:**
  - 1. Open a product detail page.
  - 2. Inspect the Quantity dropdown.
  - 3. Attempt to enter/select zero, negative, or an unsupported quantity (if the UI permits).
  - 4. Click Add To Cart.
  - 5. Inspect the cart.
- **Test Data:** Quantity: 0 / -1 / unsupported value
- **Expected Result:** Invalid quantity must be prevented or rejected; cart must not contain an invalid quantity.
- **Actual Result:** Not Executed

---

## TC_08

- **Scenario ID:** SC_08
- **Test Type:** Negative
- **Severity:** Critical
- **Test Case Description:** Verify repeated Add To Cart action does not create unintended duplicate/incorrect entries
- **Test Steps:**
  - 1. Open a product detail page.
  - 2. Select quantity 1.
  - 3. Click Add To Cart repeatedly in quick succession.
  - 4. Open the cart.
  - 5. Verify item count, quantity, and totals.
- **Test Data:** Same product; repeated clicks
- **Expected Result:** Cart should follow defined behavior (merge quantity or separate valid entries) without duplicate glitches, incorrect totals, or application errors.
- **Actual Result:** Not Executed

---

## TC_09

- **Scenario ID:** SC_09
- **Test Type:** Negative
- **Severity:** High
- **Test Case Description:** Verify cart handles removal/emptying when cart is already empty
- **Test Steps:**
  - 1. Open the Shopping Cart page with no items.
  - 2. Click Empty Cart.
  - 3. Refresh the page.
  - 4. Verify cart state and application behavior.
- **Test Data:** Empty cart
- **Expected Result:** Application should remain stable, show the empty-cart state, and not display negative counts or stale totals.
- **Actual Result:** Not Executed

---

## TC_10

- **Scenario ID:** SC_10
- **Test Type:** Negative
- **Severity:** Critical
- **Test Case Description:** Verify checkout cannot proceed when cart has no products
- **Test Steps:**
  - 1. Open the Shopping Cart page.
  - 2. Ensure the cart is empty (click Empty Cart if needed).
  - 3. Attempt to proceed to checkout/payment or Place Order if available.
  - 4. Observe the response.
- **Test Data:** Empty cart
- **Expected Result:** Checkout/order placement should be blocked; user should be prompted to add products and no order should be created.
- **Actual Result:** Not Executed

---

