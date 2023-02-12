# dba120-exam1

This is an explanation of the MySQL queries in this repository and their result.

Excercise #1: This statement adds a new row to the Terms table.

<img width="838" alt="ch5_ex1_results" src="https://user-images.githubusercontent.com/122643455/218331673-91f7d522-37af-4c99-8849-f6b2d257a1bc.png">

Excercise #2: This statement modifies the data in the row added by the previous statement.

Excercise #3: This statement deletes the row added in excercise #1.

Excercise #4: This statement adds a new row to the Invoices table. The DEFAULT keyword instructs MySQL to generate a new value in the invoice_id cell. The NULL keyword adds a null value to the payment_date cell.

Excercise #5: This statement adds two rows to the Invoice_Line_Items table.

Excercise #6: This statement modifies the row added to Invoices in excercise #4. It uses some basic equations to caculate the values for the credit_total and payment_total cells in this row.

Excercise #7: This statement changes the account_number column to 403 for all rows that have a a vednor_id of 44.

Excercise #8: This statement modifies the Invoices table by changing the cells in the terms_id column with a value of 3 to a value of 2. I had to write this differently from what was written in the book, which said that the new value should also be 2. I can only assume this is a typo.

Excercise #9: These statements delete the two rows added to the Invoice_Line_Items table in excercise #5 and the row added to the Invoices table in excercise #4.
