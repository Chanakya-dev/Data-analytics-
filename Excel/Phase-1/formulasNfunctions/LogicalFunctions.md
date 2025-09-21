# **Excel Logical Functions – Beginner Notes**

**Phase:** 1
**Project Goal:** Learn to **make decisions in Excel** using logical functions to analyze your Employee Dataset efficiently.

---

## **1. IF Function**

* **Purpose:** Returns one value if a condition is TRUE, another if FALSE.
* **Syntax:**

```
=IF(logical_test, value_if_true, value_if_false)
```

* **How to Use:**

  1. Click cell where result should appear
  2. Type `=IF(`
  3. Select or type **condition** (e.g., H2>=2)
  4. Type `,` → Enter value if TRUE
  5. Type `,` → Enter value if FALSE → Close `)` → Enter
* **Example:** Bonus eligibility based on years of service:

```
=IF(H2>=2,"Yes","No")
```

* **Step-by-Step:**

  * Click I2 → `=IF(H2>=2,"Yes","No")` → Enter → “Yes” or “No” displayed

**Mini Practice:**

* Check if employees are eligible for bonus (`Yes` if years ≥ 2)

---

## **2. AND Function**

* **Purpose:** Returns TRUE if **all conditions** are TRUE
* **Syntax:**

```
=AND(condition1, condition2, …)
```

* **How to Use:**

  1. Click cell
  2. Type `=AND(`
  3. Enter conditions separated by commas
  4. Close `)` → Enter
* **Example:** Employee eligible for bonus if **years ≥ 2 AND salary > 50000**:

```
=AND(H2>=2,F2>50000)
```

* Returns TRUE or FALSE

**Mini Practice:**

* Find employees who meet both criteria (seniority and salary threshold)

---

## **3. OR Function**

* **Purpose:** Returns TRUE if **any condition** is TRUE
* **Syntax:**

```
=OR(condition1, condition2, …)
```

* **How to Use:**

  1. Click cell
  2. Type `=OR(`
  3. Enter conditions → Close `)` → Enter
* **Example:** Employee eligible if **years ≥ 2 OR salary > 70000**:

```
=OR(H2>=2,F2>70000)
```

**Mini Practice:**

* Identify employees eligible by **either criterion**

---

## **4. NOT Function**

* **Purpose:** Reverses a logical value (TRUE → FALSE, FALSE → TRUE)
* **Syntax:**

```
=NOT(condition)
```

* **How to Use:**

  1. Click cell
  2. Type `=NOT(`
  3. Enter condition → Close `)` → Enter
* **Example:** Employee **not eligible for bonus**:

```
=NOT(H2>=2)
```

**Mini Practice:**

* Highlight employees **not meeting minimum years requirement**

---

## **5. Nested IF**

* **Purpose:** Apply multiple conditions using IF inside IF
* **Syntax:**

```
=IF(condition1, value_if_true1, IF(condition2, value_if_true2, value_if_false))
```

* **Example:** Bonus Eligibility Grades:

```
=IF(H2>=5,"High",IF(H2>=2,"Medium","Low"))
```

* Returns “High” if years ≥5, “Medium” if ≥2, else “Low”

**Mini Practice:**

* Categorize employees into High, Medium, Low bonus tiers

---

## **6. IFERROR Function**

* **Purpose:** Returns a value if formula results in error (e.g., #DIV/0!)
* **Syntax:**

```
=IFERROR(formula, value_if_error)
```

* **How to Use:**

  1. Click cell
  2. Type `=IFERROR(`
  3. Enter formula → `,` → Enter value if error → Close `)` → Enter
* **Example:** Handle division by zero in salary bonus calculation:

```
=IFERROR(F2/G2,0)
```

* Returns 0 instead of error

**Mini Practice:**

* Prevent errors when **Bonus column has empty cells**

---

## **7. Combining Logical Functions**

* Logical functions can be **nested or combined**:

```
=IF(AND(H2>=2,F2>50000),"Eligible","Not Eligible")
=IF(OR(H2>=5,G2>2000),"High Bonus","Regular Bonus")
```

* **How to Use:**

  * Combine AND/OR inside IF to handle complex conditions
* **Tip:** Keep conditions simple for readability

---

## **8. Tips for Beginners**

1. Always start formulas with `=`
2. Use **cell references** instead of numbers for dynamic results
3. Combine functions for **complex decision-making**
4. Test each condition separately before combining

---

## **9. Mini Exercises – Step by Step**

1. Check **Bonus eligibility**: `=IF(H2>=2,"Yes","No")`
2. Find employees who are **eligible by AND criteria**: `=AND(H2>=2,F2>50000)`
3. Identify employees eligible by **OR criteria**: `=OR(H2>=2,F2>70000)`
4. Reverse eligibility: `=NOT(H2>=2)`
5. Create **Bonus Grade**: `=IF(H2>=5,"High",IF(H2>=2,"Medium","Low"))`
6. Handle errors in calculation: `=IFERROR(F2/G2,0)`
7. Combine AND/OR in IF: `=IF(AND(H2>=2,F2>50000),"Eligible","Not Eligible")`

---

✅ **Outcome:**

* You can now **use all major Logical Functions** in Excel
* Able to **analyze Employee Dataset**, create eligibility criteria, categorize employees, and prevent errors
* Next step: **Text Functions (LEFT, RIGHT, MID, CONCAT, TRIM, LEN, UPPER/LOWER/PROPER)**
