# **Phase 2 – Lookup & Reference Functions**

**Project Goal:** Learn to **search, reference, and extract data** efficiently in your Employee Dataset using lookup functions.

---

## **1. VLOOKUP Function**

* **Purpose:** Look for a value in the **first column** of a table and return a value from another column in the same row.
* **Syntax:**

```
=VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])
```

* **Parameters:**

  * `lookup_value`: Value to search for
  * `table_array`: Range containing the data
  * `col_index_num`: Column number of the value to return
  * `[range_lookup]`: TRUE for approximate match, FALSE for exact match
* **Step-by-Step Usage:**

  1. Click the cell where you want the result
  2. Type `=VLOOKUP(`
  3. Select `lookup_value` → `,`
  4. Select `table_array` → `,`
  5. Enter `col_index_num` → `,`
  6. Enter `FALSE` for exact match → `)` → Enter
* **Example:** Find Salary for Employee ID 101:

```
=VLOOKUP(101, A2:F11, 6, FALSE)
```

* **Mini Practice:**

  * Lookup Employee Name, Department, or Bonus using Employee ID

---

## **2. HLOOKUP Function**

* **Purpose:** Look for a value in the **first row** of a table and return a value from another row in the same column.
* **Syntax:**

```
=HLOOKUP(lookup_value, table_array, row_index_num, [range_lookup])
```

* **Example:** Find Department in row 2 for Employee ID in row 1:

```
=HLOOKUP(101, A1:F2, 2, FALSE)
```

* **Mini Practice:**

  * Lookup Bonus or Joining Date horizontally

---

## **3. INDEX Function**

* **Purpose:** Returns the value of a cell at the **intersection of a specific row and column** in a range.
* **Syntax:**

```
=INDEX(array, row_num, [column_num])
```

* **Step-by-Step Usage:**

  1. Click target cell
  2. Type `=INDEX(`
  3. Select array → `,`
  4. Enter row number → `,` (optional: column number) → `)` → Enter
* **Example:** Value at 3rd row, 2nd column in Employee Table:

```
=INDEX(A2:F11,3,2)
```

* **Mini Practice:**

  * Retrieve Name, Department, or Salary using row & column numbers

---

## **4. MATCH Function**

* **Purpose:** Returns the **position** (row or column number) of a value in a range.
* **Syntax:**

```
=MATCH(lookup_value, lookup_array, [match_type])
```

* **Parameters:**

  * `match_type`: 0 for exact match, 1 for less than, -1 for greater than
* **Example:** Find row number of Employee ID 104:

```
=MATCH(104, A2:A11, 0)
```

* **Mini Practice:**

  * Find position of employees with specific IDs or names

---

## **5. Combining INDEX & MATCH**

* **Purpose:** Flexible lookup; better than VLOOKUP (can lookup any column).
* **Syntax:**

```
=INDEX(return_range, MATCH(lookup_value, lookup_range, 0))
```

* **Example:** Find Salary of Employee ID 103:

```
=INDEX(F2:F11, MATCH(103, A2:A11, 0))
```

* **Mini Practice:**

  * Lookup Department, Bonus, or Joining Date using Employee ID

---

## **6. XLOOKUP Function** *(Excel 365 / 2021+)*

* **Purpose:** Modern replacement for VLOOKUP/HLOOKUP; allows lookup **in any direction**.
* **Syntax:**

```
=XLOOKUP(lookup_value, lookup_array, return_array, [if_not_found], [match_mode], [search_mode])
```

* **Example:** Find Salary for Employee ID 102:

```
=XLOOKUP(102, A2:A11, F2:F11, "Not Found", 0)
```

* **Mini Practice:**

  * Lookup Name, Department, Salary, or Bonus using Employee ID
  * Handle values not found gracefully

---

## **7. ROW and COLUMN Functions**

* **Purpose:** Return **row number** or **column number** of a cell.
* **Syntax:**

```
=ROW(cell_reference)  
=COLUMN(cell_reference)
```

* **Example:**

```
=ROW(B2) → 2  
=COLUMN(C2) → 3
```

* **Mini Practice:**

  * Find row & column numbers dynamically for INDEX / MATCH formulas

---

## **8. Tips for Beginners**

1. Use **INDEX & MATCH** instead of VLOOKUP when possible (more flexible).
2. Use **XLOOKUP** in modern Excel versions (simpler, handles errors).
3. Always use **absolute references** (`$A$2:$A$11`) for fixed ranges.
4. Test formulas with small examples before applying to large datasets.

---

## **9. Mini Exercises – Step by Step**

1. Find Salary for Employee ID 105 →

```
=VLOOKUP(105,A2:F11,6,FALSE)
```

2. Find Department horizontally →

```
=HLOOKUP(102,A1:F2,2,FALSE)
```

3. Get Name using INDEX →

```
=INDEX(B2:B11,3)
```

4. Find row of Employee ID 104 →

```
=MATCH(104,A2:A11,0)
```

5. Combine INDEX & MATCH for Salary →

```
=INDEX(F2:F11, MATCH(103,A2:A11,0))
```

6. Use XLOOKUP for Bonus →

```
=XLOOKUP(102,A2:A11,G2:G11,"Not Found")
```

7. Find row & column →

```
=ROW(C5) / =COLUMN(C5)
```

---

✅ **Outcome:**

* Able to **search, reference, and extract data efficiently**
* Can handle **large Employee Datasets** dynamically
* Next step: **Named Ranges & Data Validation**
