# dba120-exam1

This is an explanation of the MySQL queries in this repository and their result.

Excercise #1: INSERT INTO terms VALUES (6, 'Net due 120 days', 120);

This statement adds a new row to the Terms table.

<img width="838" alt="ch5_ex1_results" src="https://user-images.githubusercontent.com/122643455/218331673-91f7d522-37af-4c99-8849-f6b2d257a1bc.png">

Excercise #2: UPDATE terms SET terms_description = 'Net due 125 days', terms_due_days = 125 WHERE terms_id = 6;

This statement modifies the data in the row added by the previous statement.

<img width="815" alt="ch5_ex2_results" src="https://user-images.githubusercontent.com/122643455/218331713-4a8cf87f-9cdc-47cb-a0ed-e64946f5f38e.png">

Excercise #3: DELETE FROM terms WHERE terms_id = 6;

This statement deletes the row added in excercise #1.

<img width="835" alt="ch5_ex3_results" src="https://user-images.githubusercontent.com/122643455/218331722-a6a9b4dd-d442-4ca4-9d7d-10cf210a819b.png">

Excercise #4: INSERT INTO invoices VALUES (DEFAULT, 32, 'AX-014-027', '2018-08-01', 434.58, 0.00, 0.00, 2, '2018-08-31', NULL);

This statement adds a new row to the Invoices table. The DEFAULT keyword instructs MySQL to generate a new value in the invoice_id cell. The NULL keyword adds a null value to the payment_date cell.

<img width="1389" alt="ch5_ex4_results" src="https://user-images.githubusercontent.com/122643455/218331732-8b62e2cd-5978-4fc0-a237-7f0050d4275e.png">

Excercise #5: INSERT INTO invoice_line_items VALUES (115, 1, 160, 180.23, 'Hard drive'), (115, 2, 527, 254.35, 'Exchange Server update');

This statement adds two rows to the Invoice_Line_Items table.

<img width="1090" alt="ch5_ex5_results" src="https://user-images.githubusercontent.com/122643455/218331745-6b98337a-1bd5-4362-882c-c5ee417157c9.png">

Excercise #6: UPDATE invoices SET credit_total = invoice_total * 0.1, payment_total = invoice_total - credit_total WHERE invoice_id = 115;

This statement modifies the row added to Invoices in excercise #4. It uses some basic equations to caculate the values for the credit_total and payment_total cells in this row.

<img width="1472" alt="ch5_ex6_results" src="https://user-images.githubusercontent.com/122643455/218331755-73872721-e9d2-4a50-9f96-51ee2b20c596.png">

Excercise #7: UPDATE vendors SET default_account_number = 403 WHERE vendor_id = 44;

This statement changes the account_number column to 403 for all rows that have a a vednor_id of 44.

<img width="1389" alt="ch5_ex7_results-1" src="https://user-images.githubusercontent.com/122643455/218331770-5d17b3df-111e-4631-aeca-9747ca0aee0a.png">

<img width="1389" alt="ch5_ex7_results-2" src="https://user-images.githubusercontent.com/122643455/218331808-2ea13e4b-e50d-4804-8f88-069125f7ba55.png">

Excercise #8: UPDATE invoices SET terms_id = 3 WHERE terms_id = 2;

This statement modifies the Invoices table by changing the cells in the terms_id column with a value of 3 to a value of 2. I had to write this differently from what was written in the book, which said that the new value should also be 2. I can only assume this is a typo.

<img width="1383" alt="ch5_ex8_results" src="https://user-images.githubusercontent.com/122643455/218331816-2e2a21be-8e78-474a-b089-0760abe7aadf.png">

Excercise #9: DELETE FROM invoice_line_items WHERE invoice_id = 115; DELETE FROM invoices WHERE invoice_id = 115;

These statements delete the two rows added to the Invoice_Line_Items table in excercise #5 and the row added to the Invoices table in excercise #4.

<img width="1094" alt="ch5_ex9_results-1" src="https://user-images.githubusercontent.com/122643455/218331824-c308dddc-aa05-4f72-bed7-9230c543cdac.png">

<img width="1384" alt="ch5_ex9_results-2" src="https://user-images.githubusercontent.com/122643455/218331832-428f2a5a-957a-4f0c-a505-b3f90507edd7.png">
