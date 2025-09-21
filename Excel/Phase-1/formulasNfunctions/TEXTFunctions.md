# **Excel Text Functions**

**Phase:** 1
**Project Goal:** Learn to **manipulate and analyze text data** in your Employee Dataset efficiently using Excel Text Functions.

---

## **1. LEFT Function**

* **Purpose:** Extracts a specific number of characters from the **start (left)** of a text string.
* **Syntax:**

```
=LEFT(text, num_chars)
```

* **How to Use:**

  1. Click the target cell
  2. Type `=LEFT(`
  3. Select text cell → `,` → Enter number of characters → Close `)` → Enter
* **Example:** Get first 3 letters of Employee Name:

```
=LEFT(B2,3)
```

* **Step-by-Step:**

  * Click C2 → Type `=LEFT(B2,3)` → Enter → Displays first 3 letters

**Mini Practice:**

* Extract **first 2 letters** of all employee names

---

## **2. RIGHT Function**

* **Purpose:** Extracts a specific number of characters from the **end (right)** of a text string.
* **Syntax:**

```
=RIGHT(text, num_chars)
```

* **Example:** Last 3 letters of Employee ID:

```
=RIGHT(A2,3)
```

**Mini Practice:**

* Extract last 4 digits of **Employee ID**

---

## **3. MID Function**

* **Purpose:** Extracts characters from the **middle** of a text string
* **Syntax:**

```
=MID(text, start_num, num_chars)
```

* **Example:** Extract 3 characters starting from 2nd position of Name:

```
=MID(B2,2,3)
```

**Mini Practice:**

* Extract **middle portion** of Employee Code

---

## **4. LEN Function**

* **Purpose:** Returns the **number of characters** in a text string
* **Syntax:**

```
=LEN(text)
```

* **Example:** Length of Employee Name:

```
=LEN(B2)
```

**Mini Practice:**

* Find **length of each employee name**

---

## **5. TRIM Function**

* **Purpose:** Removes **extra spaces** from text (except single spaces between words)
* **Syntax:**

```
=TRIM(text)
```

* **Example:** Clean employee names:

```
=TRIM(B2)
```

**Mini Practice:**

* Remove leading/trailing/multiple spaces in names

---

## **6. CONCAT / CONCATENATE Function**

* **Purpose:** Combines text from multiple cells into one
* **Syntax:**

```
=CONCAT(text1, text2, …)  
=CONCATENATE(text1, text2, …)  → Older version
```

* **Example:** Combine First Name & Last Name with space:

```
=CONCAT(B2," ",C2)
```

**Mini Practice:**

* Merge **First Name & Last Name** into Full Name

---

## **7. UPPER, LOWER, PROPER Functions**

* **Purpose:** Change text case
* **Syntax:**

```
=UPPER(text) → All uppercase  
=LOWER(text) → All lowercase  
=PROPER(text) → Capitalize first letter of each word
```

* **Example:**

  * `=UPPER(B2)` → Convert name to uppercase
  * `=PROPER(B2)` → Standardize name formatting

**Mini Practice:**

* Convert all employee names to **Proper Case**

---

## **8. FIND and SEARCH Functions**

* **Purpose:** Locate position of a character or text within a string
* **Syntax:**

```
=FIND(find_text, within_text, [start_num]) → Case-sensitive  
=SEARCH(find_text, within_text, [start_num]) → Not case-sensitive
```

* **Example:** Position of “a” in Name:

```
=FIND("a",B2)
=SEARCH("a",B2)
```

**Mini Practice:**

* Find position of **“@” in email addresses**

---

## **9. REPLACE Function**

* **Purpose:** Replace part of text with new text
* **Syntax:**

```
=REPLACE(old_text, start_num, num_chars, new_text)
```

* **Example:** Replace first 3 letters of Employee Code with “EMP”:

```
=REPLACE(A2,1,3,"EMP")
```

**Mini Practice:**

* Standardize **Employee Codes** using REPLACE

---

## **10. SUBSTITUTE Function**

* **Purpose:** Replace specific text or characters in a string
* **Syntax:**

```
=SUBSTITUTE(text, old_text, new_text, [instance_num])
```

* **Example:** Replace “Inc” with “LLC” in company names:

```
=SUBSTITUTE(C2,"Inc","LLC")
```

**Mini Practice:**

* Replace **spaces with underscores** in Employee IDs

---

## **11. TEXT Function**

* **Purpose:** Format numbers, dates, or time into text with custom formatting
* **Syntax:**

```
=TEXT(value, format_text)
```

* **Example:** Format salary with comma and 2 decimals:

```
=TEXT(F2,"#,##0.00")
```

* Format date as “dd-mmm-yyyy”:

```
=TEXT(G2,"dd-mmm-yyyy")
```

**Mini Practice:**

* Format **Salary & Joining Date** for reports

---

## **12. Tips for Beginners**

1. Always start formulas with `=`
2. Combine text functions for **cleaning and standardizing data**
3. Use **TRIM** before other text operations
4. **CONCAT / CONCATENATE** is useful for dashboards and reports

---

## **13. Mini Exercises – Step by Step**

1. Extract first 3 letters of Name → `=LEFT(B2,3)`
2. Extract last 4 letters of Employee ID → `=RIGHT(A2,4)`
3. Extract middle 3 letters of Employee Code → `=MID(A2,2,3)`
4. Count characters in Name → `=LEN(B2)`
5. Remove extra spaces → `=TRIM(B2)`
6. Combine First & Last Name → `=CONCAT(B2," ",C2)`
7. Convert Name to Proper Case → `=PROPER(B2)`
8. Find position of “@” in email → `=FIND("@",D2)`
9. Replace first 3 letters of Code → `=REPLACE(A2,1,3,"EMP")`
10. Replace spaces with underscores → `=SUBSTITUTE(A2," ","_")`
11. Format Salary → `=TEXT(F2,"#,##0.00")`

---

✅ **Outcome:**

* You can now **extract, clean, combine, and format text** in Excel
* Able to prepare **Employee Dataset** for reporting or dashboards
* Next step: **Date & Time Functions (DATE, TODAY, NOW, YEAR, MONTH, DAY, NETWORKDAYS, EOMONTH)**
