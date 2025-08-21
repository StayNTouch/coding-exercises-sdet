# coding-exercises-sdet
## Cypress Automation Assignment
# Objective

Create a Cypress test with Typescript that automates a hotel reservation flow on Expedia. The test must demonstrate proficiency in handling:

Calendar selection (choosing check-in and check-out dates)

Form input (first name, last name, email, phone, etc.)

Drag-and-drop interaction (filter slider for price)

iFrame handling (if applicable on the payment/confirmation step)

Pop-up window handling (terms, confirmation, or offers modal)

# Flow Design
# Step 1: Open Reservation Page

Navigate to https://www.expedia.com/
.

Verify that the page title contains “Expedia”.

# Step 2: Select Destination City and Dates (Calendar)

Enter destination city: New York, New York.

Select arrival date = today + 2 months (e.g., if today is August 20, 2025 → arrival date should be October 20, 2025).

Select departure date = arrival date + 1 day (making it a 1-night stay).

Click on Search.

# Step 3: Filter and Select Hotel

Use drag-and-drop slider to adjust the total price range → Min: $0, Max: $500.

Apply filter for Guest Rating = “Wonderful 9+”.

Apply filter for Star Rating = 5 stars.

Select any available hotel option from the filtered list.

# Step 4: Reserve a Room

Choose any available room and click Reserve.

Fill in all required guest details (first name, last name, email, phone, etc.).

Handle any iframe present in the payment step (e.g., credit card entry field).

Click Book Now.

# Step 5: Verification

On the confirmation page, add at least 5 assertions of your choice.

# Step 6: Submit your PR to this repository

Create a separate branch for your work
