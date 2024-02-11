# Kaizntree Front-End Take-Home Challenge

## My Challenge

Welcome to Kaizntree's Front-End Take-Home Challenge! In this challenge, I will be fixing bugs in the provided starter code. These bugs are independent of each other, so I can fix them in any order.

## Bugs to be Fixed

### Bug 1: Select dropdown doesn't scroll with rest of the page

How to reproduce:
Make your viewport smaller in height. Small enough to have a scroll bar.
Click on the Filter by employee select to open the options dropdown.
Scroll down the page.
Expected: Options dropdown moves with its parent input as you scroll the page.
Actual: Options dropdown stays in the same position as you scroll the page, losing the reference to the select input.

### Bug 2: Approve checkbox not working

How to reproduce:
Click on the checkbox on the right of any transaction.
Expected: Clicking the checkbox toggles its value.
Actual: Nothing happens.

### Bug 3: Cannot select _All Employees_ after selecting an employee

How to reproduce:
Click on the Filter by employee select to open the options dropdown.
Select an employee from the list.
Click on the Filter by employee select to open the options dropdown.
Select All Employees option.
Expected: All transactions are loaded.
Actual: The page crashes.

### Bug 4: Clicking on View More button not showing correct data

How to reproduce:
Click on the View more button.
Wait until the new data loads.
Expected: Initial transactions plus new transactions are shown on the page.
Actual: New transactions replace initial transactions, losing initial transactions.

### Bug 5: Employees filter not available during loading more data

How to reproduce (Part 1):
Open devtools to watch the simulated network requests in the console.
Refresh the page.
Quickly click on the Filter by employee select to open the options dropdown.
Expected: The filter should stop showing "Loading employees.." as soon as the request for employees is succeeded.
Actual: The filter stops showing "Loading employees.." until paginatedTransactions is succeeded.

How to reproduce (Part 2):
Open devtools to watch the simulated network requests in the console.
Click on View more button.
Quickly click on the Filter by employee select to open the options dropdown.
Expected: The employees filter should not show "Loading employees..." after clicking View more.
Actual: The employees filter shows "Loading employees..." after clicking View more until new transactions are loaded.

### Bug 6: View more button not working as expected

How to reproduce (Part 1):
Click on the Filter by employee select to open the options dropdown.
Select an employee from the list.
Wait until transactions load.
Expected: The View more button is not visible when transactions are filtered by user.
Actual: The View more button is visible even when transactions are filtered by employee.
How to reproduce (Part 2):
Click on View more button.
Wait until it loads more data.
Repeat these steps as many times as you can.
Expected: When you reach the end of the data, the View More button disappears.
Actual: When you reach the end of the data, the View More button is still showing and you are still able to click the button.


### Bug 7: Approving a transaction won't persist the new value

How to reproduce:
Click on the Filter by employee select to open the options dropdown.
Select an employee from the list (E.g. James Smith).
Toggle the first transaction (E.g. Uncheck Social Media Ads Inc).
Click on the Filter by employee select to open the options dropdown.
Select All Employees option.
Verify values.
Click on the Filter by employee select to open the options dropdown.
Verify values.
Expected: In steps 6 and 8, toggled transaction kept the same value it was given in step 2 (E.g. Social Media Ads Inc is unchecked).
Actual: In steps 6 and 8, toggled transaction lost the value given in step 2. (E.g. Social Media Ads Inc is checked again).

## Submission

To view my solution, please visit the [CodeSandbox](link-to-codesandbox) link.

## Notes
- My solution will be evaluated based on correctness, clarity, and adherence to the instructions.

Thank you for considering my submission!

Happy bug fixing! 🐛🔨

