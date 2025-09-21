# **Phase 1: Excel – Formulas (Detailed Notes)**

**Project Goal:** Learn to **write formulas to perform calculations, analyze data, and automate results** in your Employee Dataset.

---

## **1. What is a Formula?**

* **Definition:** A formula is a **user-defined calculation** in Excel that performs operations using numbers, cell references, operators, or functions.
* **All formulas start with `=`**.
* Formulas can include:

  1. **Operators** (`+`, `-`, `*`, `/`, `^`)
  2. **Cell references** (`A2`, `B3`)
  3. **Constants** (fixed numbers, e.g., `100`)
  4. **Functions** (predefined formulas, optional)

**Example:**

```
=F2+G2
```

* Adds values in F2 (Base Salary) and G2 (Bonus)

---

## **2. Components of a Formula**

1. **Equal Sign `=`:** Indicates that the cell contains a formula
2. **Operands:** Numbers or cell references involved in calculation
3. **Operators:** Symbols that perform operations
4. **Functions (optional):** Built-in calculations like SUM, AVERAGE

---

## **3. Operators in Excel Formulas**

| Operator | Purpose        | Example   | Result         |
| -------- | -------------- | --------- | -------------- |
| `+`      | Addition       | `=A2+B2`  | Sum of A2 & B2 |
| `-`      | Subtraction    | `=A2-B2`  | Difference     |
| `*`      | Multiplication | `=A2*B2`  | Product        |
| `/`      | Division       | `=A2/B2`  | Quotient       |
| `^`      | Exponent       | `=A2^2`   | A2 squared     |
| `%`      | Percentage     | `=A2*10%` | 10% of A2      |

**Mini Practice:**

* Total Compensation → `=F2+G2`
* 10% Tax on Total Compensation → `=(F2+G2)*10%`
* Bonus squared → `=G2^2`

---

## **4. Using Cell References**

* **Relative Reference:** Changes when formula is copied

  * Example: `=F2+G2` copied to next row → becomes `=F3+G3`
* **Absolute Reference:** Fixed reference using `$`

  * Example: `=$F$2+$G$2` → Always refers to F2 & G2
* **Mixed Reference:** Partially fixed

  * Example: `=F$2+$G2` → Row fixed for F, Column fixed for G

**Practice:**

* Create formula for **Total Compensation**
* Copy formula down using **relative references**
* Fix a cell for **Tax Rate (absolute reference)**

---

## **5. Order of Operations in Formulas**

* Excel follows **BODMAS/PEMDAS**:

  1. **Parentheses `( )`**
  2. **Exponent `^`**
  3. **Multiplication `*` / Division `/`**
  4. **Addition `+` / Subtraction `-`**

**Example:**

```
=F2+G2*10%   → Bonus*10% added to Base Salary
=(F2+G2)*10% → Total *10%, parentheses change order
```

**Mini Practice:** Test both versions on Employee Dataset

---

## **6. Common Formula Types**

### **6.1 Arithmetic Formulas**

* Perform simple calculations with numbers
* Example: `=F2+G2`, `=F2-G2`, `=F2*1.1`

### **6.2 Logical Formulas**

* Use conditions with IF
* Example: `=IF(H2>=2,"Yes","No")`

### **6.3 Text Formulas**

* Combine or manipulate text
* Example: `=A2 & "-" & B2` → "101-John"

### **6.4 Date & Time Formulas**

* Calculate age, tenure
* Example: `=TODAY()-D2` → Days since joining

---

## **7. Errors in Formulas**

* Common errors you may encounter:
  \| Error | Cause | Example |
  \|-------|-------|---------|
  \| `#DIV/0!` | Division by zero | `=F2/0` |
  \| `#VALUE!` | Wrong data type | `="Text"+1` |
  \| `#REF!` | Deleted/missing cell | `=A2+B20` (B20 deleted) |
  \| `#NAME?` | Wrong function name | `=SUMM(F2:F10)` |

**Tip:** Use `IFERROR` to handle errors gracefully:

```
=IFERROR(F2/G2,0)
```

---

## **8. Mini Practice Exercises – Formulas**

1. Calculate **Total Compensation** → `=F2+G2`
2. Calculate **Tax (10%)** → `=(F2+G2)*10%`
3. Calculate **Net Salary** → `=F2+G2-H2`
4. Combine **Employee ID & Name** → `=A2 & "-" & B2`
5. Test **absolute reference** by fixing Tax Rate cell `$H$1`

---

✅ **Outcome:**

* You can now **write custom formulas** to perform calculations
* Understand **cell references, operators, and error handling**
* Prepared to combine **formulas with functions** for advanced calculations
