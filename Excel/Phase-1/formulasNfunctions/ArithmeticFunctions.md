# **Excel Arithmetic / Mathematical Functions – Beginner Notes**

**Phase:** 1
**Project Goal:** Learn to **perform all numeric calculations** in your Employee Dataset using Excel functions.

---

## **1. SUM Function**

* **Purpose:** Adds numbers in a range or individual cells.
* **Syntax:**

```
=SUM(number1, [number2], …)
```

* **How to Use:**

  1. Click the cell where the result should appear.
  2. Type `=SUM(`
  3. Select the range of cells (e.g., F2\:F11)
  4. Close parenthesis `)` and press **Enter**
* **Example:** `=SUM(F2:F11)` → Total Base Salary
* **Tip:** Use **AutoSum** button (Home → Editing → AutoSum) for quick summation

---

## **2. AVERAGE Function**

* **Purpose:** Calculates the arithmetic mean of numbers.
* **Syntax:**

```
=AVERAGE(number1, [number2], …)
```

* **How to Use:**

  1. Click target cell
  2. Type `=AVERAGE(`
  3. Select range (e.g., F2\:F11)
  4. Close parenthesis `)` → Press **Enter**
* **Example:** `=AVERAGE(F2:F11)` → Average Base Salary
* **Tip:** Ignores blank cells automatically

---

## **3. MIN and MAX Functions**

* **Purpose:** Returns the smallest (`MIN`) or largest (`MAX`) value.
* **Syntax:**

```
=MIN(range)  
=MAX(range)
```

* **How to Use:**

  1. Click cell
  2. Type `=MIN(` or `=MAX(`
  3. Select range → `)` → Enter
* **Example:**

  * `=MIN(F2:F11)` → Lowest Salary
  * `=MAX(F2:F11)` → Highest Salary

---

## **4. COUNT and COUNTA Functions**

* **Purpose:** Count numeric values (`COUNT`) or all non-empty cells (`COUNTA`)
* **Syntax:**

```
=COUNT(range)  
=COUNTA(range)
```

* **How to Use:**

  1. Click target cell
  2. Type `=COUNT(` or `=COUNTA(`
  3. Select range → `)` → Enter
* **Example:**

  * `=COUNT(F2:F11)` → Number of numeric salaries
  * `=COUNTA(B2:B11)` → Number of employees with names

---

## **5. ROUND Functions**

* **Purpose:** Round numbers to a specific decimal place

* **Functions & Syntax:**
  \| Function | Syntax | Purpose |
  \|----------|--------|--------|
  \| ROUND | `=ROUND(number, num_digits)` | Round normally |
  \| ROUNDUP | `=ROUNDUP(number, num_digits)` | Always round up |
  \| ROUNDDOWN | `=ROUNDDOWN(number, num_digits)` | Always round down |
  \| INT | `=INT(number)` | Round down to nearest integer |
  \| TRUNC | `=TRUNC(number, num_digits)` | Remove decimals without rounding |

* **How to Use:**

  1. Click target cell
  2. Type function (e.g., `=ROUND(F2,0)`)
  3. Enter → Rounded value displayed

* **Example:**

  * `=ROUND(F2,0)` → Round Base Salary
  * `=ROUNDUP(G2,0)` → Round Bonus up

---

## **6. ABS Function**

* **Purpose:** Returns absolute (positive) value
* **Syntax:** `=ABS(number)`
* **How to Use:** Click cell → Type `=ABS(F2-G2)` → Enter
* **Example:** Difference between Salary and Bonus: `=ABS(F2-G2)`

---

## **7. POWER and SQRT Functions**

* **POWER:** Raises a number to a power

  * Syntax: `=POWER(number, power)` → `=POWER(G2,2)` (Bonus squared)
* **SQRT:** Calculates square root

  * Syntax: `=SQRT(number)` → `=SQRT(F2)` (Square root of Salary)
* **How to Use:** Click cell → Type function → Select cell → Close parenthesis → Enter

---

## **8. MOD Function**

* **Purpose:** Returns remainder after division
* **Syntax:** `=MOD(number, divisor)`
* **How to Use:** Click cell → Type `=MOD(F2,1000)` → Enter
* **Example:** Salary remainder after dividing by 1000

---

## **9. SUMPRODUCT Function**

* **Purpose:** Multiply corresponding elements in arrays and return sum
* **Syntax:** `=SUMPRODUCT(array1, array2, …)`
* **How to Use:**

  1. Click cell
  2. Type `=SUMPRODUCT(`
  3. Select first array → `,` → Select second array → `)` → Enter
* **Example:** Total weighted Salary × Bonus: `=SUMPRODUCT(F2:F11,G2:G11)`

---

## **10. EXP and LN Functions (Optional)**

* **EXP(number):** Returns e^number
* **LN(number):** Returns natural log
* **Use:** Scientific calculations, optional for payroll

---

## **11. Order of Operations**

* Excel follows **BODMAS/PEMDAS**
* **Example:**

```
=F2+G2*10% → Adds 10% of Bonus to Base Salary  
=(F2+G2)*10% → 10% of Total Compensation (parentheses change result)
```

---

## **12. Tips for Beginners**

1. Always start formulas with `=`
2. Use **cell references**, not fixed numbers
3. Combine multiple functions for **complex calculations**
4. Use **AutoSum** and `fx` function suggestion for efficiency

---

## **13. Step-by-Step Mini Exercises**

1. Total Compensation → `=SUM(F2:G2)` → Enter
2. Average Salary → `=AVERAGE(F2:F11)` → Enter
3. Highest & Lowest Salary → `=MAX(F2:F11)` / `=MIN(F2:F11)` → Enter
4. Round Salary → `=ROUND(F2,0)` → Enter
5. Absolute Difference → `=ABS(F2-G2)` → Enter
6. Bonus squared → `=POWER(G2,2)` → Enter
7. Salary remainder → `=MOD(F2,1000)` → Enter
8. Weighted Total → `=SUMPRODUCT(F2:F11,G2:G11)` → Enter

---

✅ **Outcome:**

* Able to **perform all arithmetic calculations using Excel functions**
* Can **use SUM, AVERAGE, MIN, MAX, ROUND, ABS, POWER, SQRT, MOD, SUMPRODUCT** step by step
* Next step: **Logical Functions (IF, AND, OR, NOT, IFERROR)**
