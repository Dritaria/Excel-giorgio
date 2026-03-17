# Conditional Logic in Excel

Conditional logic functions are essential tools in Excel that allow users to perform different actions based on whether specified conditions are met. Below are some crucial functions: 

## 1. IF Function
The IF function checks whether a condition is met and returns one value for a TRUE result and another for a FALSE result.
- **Syntax**: `IF(logical_test, value_if_true, value_if_false)`  
- **Example**: `=IF(A1 > 10, "Greater than 10", "10 or less")`  
**Scenario**: Use this to categorize scores: if the score is greater than 75, mark it as "Pass", otherwise, "Fail".

## 2. IFS Function
The IFS function checks multiple conditions and returns a value corresponding to the first TRUE condition.
- **Syntax**: `IFS(condition1, value1, [condition2, value2], ...)`  
- **Example**: `=IFS(A1 > 75, "A", A1 > 50, "B", A1 > 25, "C", TRUE, "D")`  
**Scenario**: Automatically assign letter grades based on score ranges.

## 3. AND Function
The AND function tests multiple conditions and returns TRUE only if all conditions are TRUE.
- **Syntax**: `AND(logical1, [logical2], ...)`  
- **Example**: `=AND(A1 > 0, B1 < 100)`  
**Scenario**: Check if a sale meets both the minimum quantity and price range.

## 4. OR Function
The OR function tests multiple conditions and returns TRUE if at least one condition is TRUE.
- **Syntax**: `OR(logical1, [logical2], ...)`  
- **Example**: `=OR(A1 > 0, B1 < 100)`  
**Scenario**: Determine if a purchase is eligible for a discount if it meets one of the criteria.

## 5. NOT Function
The NOT function reverses the boolean value of its argument.
- **Syntax**: `NOT(logical)`  
- **Example**: `=NOT(A1 > 10)`  
**Scenario**: Check if a value is NOT greater than a certain amount.

## 6. ISBLANK Function
The ISBLANK function checks if a cell is empty and returns TRUE or FALSE.
- **Syntax**: `ISBLANK(value)`  
- **Example**: `=ISBLANK(A1)`  
**Scenario**: Validate form entries to ensure all required fields are completed.

## 7. ISNUMBER Function
The ISNUMBER function checks if a cell contains a numeric value.
- **Syntax**: `ISNUMBER(value)`  
- **Example**: `=ISNUMBER(A1)`  
**Scenario**: Verify if user input is a valid numeric score.

## 8. ISTEXT Function
The ISTEXT function checks if a cell contains text and returns TRUE or FALSE.
- **Syntax**: `ISTEXT(value)`  
- **Example**: `=ISTEXT(A1)`  
**Scenario**: Ensure that a name entered in a form is actual text.

## Complex Practical Scenario:
Imagine a sales team that uses a spreadsheet to track performance:
- **Task**: Create a performance evaluation system.
- **Conditions**:  
1. If a salesperson achieves more than $10,000 in sales, they receive a "Gold" rating.  
2. If they achieve between $5,000 and $10,000, they get a "Silver" rating.  
3. Below $5,000, they receive a "Bronze" rating.

### Solution:
Using a combination of nested IF functions:  
`=IF(A1 > 10000, "Gold", IF(A1 >= 5000, "Silver", "Bronze"))`  
This formula evaluates the sales amount and assigns the correct performance category.  

By mastering these functions, users can enhance their data analysis capabilities and streamline decision-making processes within Excel.