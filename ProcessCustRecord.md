## Process customer record
A program is required to read a customer’s name, a purchase amount and a tax code. 

The tax code has been validated and will be one of the following:
    0  tax exempt (0%)
    1  state sales tax only (3%)
    2  federal and state sales tax (5%)
    3  special sales tax (7%)
	
The program must then compute the sales tax and the total amount due,and print the customer’s name, purchase amount, sales tax and total amount due.

INPUTS
customer_name
purchase_amount
tax_code

OUTPUTS 
customer_name
purchase_amount
sales_tax
total_amount_due

PROCESSING STEPS
read customer_name, purchase_amount, tax_code

taxcode_percent = 0 
if taxcode = 1 then 
	taxcode_percent = 3
else if taxcode = 2 then 
	taxcode_percent = 5 
else if taxcode = 3 
	then taxcode_percent = 7

tax_due = purchase_amount * (taxcode_percent/100)
totalamount = purchase_amount + tax_due

display customer_name, purchase_amount, tax_due, total_amount_due