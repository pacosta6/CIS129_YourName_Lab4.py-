# CIS129_Paul_Acosta_Lab4.py-
Bonus Sales Calculation
Sales Amount
It covers sales Amount sales Increase 
# Step 1: Declare variables
store_amount = 0  # store bonus amount
emp_amount = 0    # employee bonus amount
sales_increase = 0  # percent of sales increase

# Step 2: Get the monthly sales
monthly_sales = float(input("Enter the monthly sales: "))

# Step 3: Determine the storeAmount bonus
if monthly_sales >= 110000:
    store_amount = 6000
elif monthly_sales >= 100000:
    store_amount = 5000
elif monthly_sales >= 90000:
    store_amount = 4000
elif monthly_sales >= 80000:
    store_amount = 3000
else:
    store_amount = 0

# Step 4: Get the percent of sales increase
sales_increase = float(input("Enter the percent increase in sales (e.g., 5 for 5%): "))
sales_increase = sales_increase / 100  # Convert percent to decimal

# Step 5: Determine the employee bonus (empAmount)
if sales_increase >= 0.05:
    emp_amount = 75
elif sales_increase >= 0.04:
    emp_amount = 50
elif sales_increase >= 0.03:
    emp_amount = 40
else:
    emp_amount = 0

# Step 6: Print the store bonus and employee bonus amounts
print("The store bonus amount is $", store_amount)
print("The employee bonus amount is $", emp_amount)

# Check if the highest bonus amounts are reached
if (store_amount == 6000) and (emp_amount == 75):
    print("Congrats! You have reached the highest bonus amounts possible!")
