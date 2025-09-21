# **Phase 1: Excel – Types of Functions**

**Goal:** Learn **different categories of Excel functions** and when to use each type to analyze your Employee Dataset efficiently.

---

## **1. Arithmetic / Mathematical Functions**

* **Purpose:** Perform calculations with numbers.
* **Common Functions:**

  1. `SUM(range)` → Adds numbers

     * Example: `=SUM(F2:F11)` → Total Base Salary
  2. `AVERAGE(range)` → Calculates average

     * Example: `=AVERAGE(F2:F11)` → Average Salary
  3. `MIN(range)` → Minimum value

     * Example: `=MIN(F2:F11)` → Lowest salary
  4. `MAX(range)` → Maximum value

     * Example: `=MAX(F2:F11)` → Highest salary
  5. `ROUND(number,digits)` → Round to specified decimals

     * Example: `=ROUND(G2,0)` → Round Bonus to nearest integer
  6. `ROUNDUP`, `ROUNDDOWN`, `INT`, `MOD`, `ABS` → Various mathematical operations

---

## **2. Logical Functions**

* **Purpose:** Make decisions or check conditions.
* **Common Functions:**

  1. `IF(condition, value_if_true, value_if_false)` → Basic conditional check

     * Example: `=IF(H2>=2,"Yes","No")` → Bonus eligibility
  2. `AND(condition1, condition2, …)` → Returns TRUE if all conditions true

     * Example: `=AND(F2>50000, H2>=2)`
  3. `OR(condition1, condition2, …)` → Returns TRUE if any condition true

     * Example: `=OR(F2>70000, Bonus="Yes")`
  4. `NOT(condition)` → Reverse logical value

     * Example: `=NOT(H2>=2)`

---

## **3. Text / String Functions**

* **Purpose:** Manipulate text and clean data.
* **Common Functions:**

  1. `LEFT(text, num_chars)` → Extract left characters

     * Example: `=LEFT(B2,5)` → First 5 letters of Name
  2. `RIGHT(text, num_chars)` → Extract right characters

     * Example: `=RIGHT(A2,3)` → Last 3 digits of Employee ID
  3. `MID(text, start_num, num_chars)` → Extract middle characters

     * Example: `=MID(B2,2,3)`
  4. `LEN(text)` → Count characters

     * Example: `=LEN(B2)` → Name length
  5. `TRIM(text)` → Remove extra spaces
  6. `UPPER(text)`, `LOWER(text)`, `PROPER(text)` → Change text case
  7. `CONCAT(text1,text2,...)` → Join texts

     * Example: `=CONCAT(A2,"-",B2)` → "101-John"

---

## **4. Date & Time Functions**

* **Purpose:** Handle dates and time for analysis.
* **Common Functions:**

  1. `TODAY()` → Current date
  2. `NOW()` → Current date and time
  3. `YEAR(date)`, `MONTH(date)`, `DAY(date)` → Extract parts of a date
  4. `WEEKDAY(date)` → Returns day of the week
  5. `EOMONTH(start_date, months)` → Last day of month
  6. `DATEDIF(start_date,end_date,"Y")` → Difference in years (Age or Tenure)
  7. `NETWORKDAYS(start_date,end_date,holidays)` → Working days between dates

---

## **5. Lookup & Reference Functions**

* **Purpose:** Retrieve data from tables or ranges.
* **Common Functions:**

  1. `VLOOKUP(lookup_value, table, col_index, range_lookup)` → Vertical lookup
  2. `HLOOKUP(lookup_value, table, row_index, range_lookup)` → Horizontal lookup
  3. `INDEX(array, row_num, col_num)` → Return value from row & column
  4. `MATCH(lookup_value, lookup_array, match_type)` → Find position of value
  5. `XLOOKUP(lookup_value, lookup_array, return_array, [if_not_found])` → Modern replacement for VLOOKUP/HLOOKUP

---

## **6. Tips for Using Functions**

* Always start with `=`
* Use **cell references** instead of fixed numbers
* **Combine functions** for complex calculations

  * Example: `=IF(AND(F2>50000,H2>=2),"Eligible","Not Eligible")`
* Use **Insert Function (fx)** → Excel suggests functions with description

---

## **7. Mini Exercises – Functions**

1. Calculate **Total Salary** → `=SUM(F2:G2)`
2. Calculate **Average Salary** → `=AVERAGE(F2:F11)`
3. Find **Highest & Lowest Salary** → `=MAX(F2:F11)`, `=MIN(F2:F11)`
4. Use **IF Function** → Bonus Eligibility → `=IF(H2>=2,"Yes","No")`
5. Combine **Text & Numbers** → `=CONCAT(A2,"-",B2)`
6. Calculate **Age** → `=DATEDIF(DOB,TODAY(),"Y")`

---

✅ **Outcome:**

* You now know **all major function categories in Excel**
* You can **decide which function type to use** depending on the dataset requirement
* Ready to **learn each function in detail with examples**, starting from Arithmetic → Logical → Text → Date → Lookup
