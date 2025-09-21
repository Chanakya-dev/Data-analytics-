# **Excel Date & Time Functions – Beginner Notes**

**Phase:** 1
**Project Goal:** Learn to **manage, analyze, and calculate dates and times** in your Employee Dataset efficiently using Excel Date & Time functions.

---

## **1. TODAY Function**

* **Purpose:** Returns the **current date** (updates automatically).
* **Syntax:**

```
=TODAY()
```

* **How to Use:**

  1. Click the cell where date should appear
  2. Type `=TODAY()` → Enter
* **Example:** Calculate employee tenure:

```
=TODAY()-G2
```

* **Tip:** Format the cell as Date if Excel shows a number

---

## **2. NOW Function**

* **Purpose:** Returns **current date and time**
* **Syntax:**

```
=NOW()
```

* **Example:** Track report generation time:

```
=NOW()
```

---

## **3. DATE Function**

* **Purpose:** Creates a date from **year, month, day**
* **Syntax:**

```
=DATE(year, month, day)
```

* **How to Use:**

  1. Click cell → Type `=DATE(`
  2. Enter year, month, day → Close `)` → Enter
* **Example:** Create Joining Date:

```
=DATE(2023,9,21)
```

---

## **4. YEAR, MONTH, DAY Functions**

* **Purpose:** Extract specific components from a date
* **Syntax:**

```
=YEAR(date) → 2025  
=MONTH(date) → 1-12  
=DAY(date) → 1-31
```

* **How to Use:**

  1. Click cell → Type function → Select date cell → Enter
* **Example:**

```
=YEAR(G2) → Joining Year  
=MONTH(G2) → Joining Month  
=DAY(G2) → Joining Day
```

---

## **5. WEEKDAY Function**

* **Purpose:** Returns the **day of the week** as a number (1 = Sunday, 7 = Saturday by default)
* **Syntax:**

```
=WEEKDAY(date, [return_type])
```

* **Example:** Determine joining weekday:

```
=WEEKDAY(G2)
```

* **Tip:** `return_type = 2` → Monday=1, Sunday=7

---

## **6. NETWORKDAYS Function**

* **Purpose:** Counts **working days** between two dates (excludes weekends)
* **Syntax:**

```
=NETWORKDAYS(start_date, end_date, [holidays])
```

* **Example:** Calculate days employee worked between Joining Date and Today:

```
=NETWORKDAYS(G2,TODAY())
```

---

## **7. EOMONTH Function**

* **Purpose:** Returns **last day of the month** n months before/after a date
* **Syntax:**

```
=EOMONTH(start_date, months)
```

* **Example:** Get month-end date after 3 months of joining:

```
=EOMONTH(G2,3)
```

---

## **8. HOUR, MINUTE, SECOND Functions**

* **Purpose:** Extract hours, minutes, seconds from a time value
* **Syntax:**

```
=HOUR(time)  
=MINUTE(time)  
=SECOND(time)
```

* **Example:** If time is 14:35:50 → HOUR=14, MINUTE=35, SECOND=50

---

## **9. TIME Function**

* **Purpose:** Creates a time value from hours, minutes, seconds
* **Syntax:**

```
=TIME(hour, minute, second)
```

* **Example:** Meeting time 9:30 AM →

```
=TIME(9,30,0)
```

---

## **10. DATEDIF Function** *(Hidden Function)*

* **Purpose:** Calculates difference between two dates in **years, months, or days**
* **Syntax:**

```
=DATEDIF(start_date, end_date, unit)
```

* **Units:**

  * `"Y"` → Years
  * `"M"` → Months
  * `"D"` → Days
* **Example:** Employee tenure in years:

```
=DATEDIF(G2,TODAY(),"Y")
```

---

## **11. TEXT Function for Dates**

* **Purpose:** Format dates in readable style
* **Syntax:**

```
=TEXT(date,"format_text")
```

* **Examples:**

```
=TEXT(G2,"dd-mmm-yyyy") → 21-Sep-2025  
=TEXT(G2,"dddd") → Monday  
=TEXT(G2,"mmm-yyyy") → Sep-2025
```

---

## **12. Tips for Beginners**

1. Excel stores dates as **numbers**; formatting is key
2. Always check **cell formatting** (Date/Time/General)
3. Combine functions to calculate **tenure, payroll cycles, deadlines**
4. NETWORKDAYS helps in **project scheduling and leave calculation**

---

## **13. Mini Exercises – Step by Step**

1. Show **today’s date** → `=TODAY()`
2. Show **current date & time** → `=NOW()`
3. Create Joining Date → `=DATE(2023,9,21)`
4. Extract **year/month/day** → `=YEAR(G2)`, `=MONTH(G2)`, `=DAY(G2)`
5. Find **weekday of joining** → `=WEEKDAY(G2)`
6. Count working days → `=NETWORKDAYS(G2,TODAY())`
7. Get **month-end date after 3 months** → `=EOMONTH(G2,3)`
8. Extract hour/minute/second from time → `=HOUR(H2)`, `=MINUTE(H2)`, `=SECOND(H2)`
9. Create time → `=TIME(9,30,0)`
10. Calculate tenure in years → `=DATEDIF(G2,TODAY(),"Y")`
11. Format date → `=TEXT(G2,"dd-mmm-yyyy")`

---

✅ **Outcome:**

* You can now **calculate, extract, format, and analyze dates and times** in Excel
* Able to prepare **employee tenure reports, project timelines, and date-based calculations**
* Next step: **Lookup & Reference Functions (VLOOKUP, HLOOKUP, INDEX, MATCH, XLOOKUP)**
