# Excel – Navigation, Cells, Rows, and Columns**

**Project Goal (Phase 1 focus):** Learn to **move around Excel efficiently, select, insert, delete, and manage cells, rows, and columns** to build your employee dataset.

---

## **1. Workbook and Worksheet Basics**

### **1.1 Workbook**

* **Definition:** The entire Excel file you open or save.
* Can contain **multiple worksheets (tabs)**.
* File extension: `.xlsx`

**Tip:** Think of Workbook as a **book**, and each Worksheet as a **page in the book**.

---

### **1.2 Worksheet**

* **Definition:** A single sheet inside a workbook.
* Structure:

  * **Rows:** Numbered (1, 2, 3…)
  * **Columns:** Lettered (A, B, C…)
  * **Cells:** Intersection of a row and a column (e.g., B2)

**Practice:** Open a new workbook → Rename first sheet as `Employee_Data` → Second sheet as `Salary`.

---

## **2. Cells in Excel**

### **2.1 What is a Cell?**

* **Cell:** The basic unit in Excel where you type data (numbers, text, dates).
* Each cell has a **cell reference**: Column + Row.

**Example:**

* A1 → Column A, Row 1
* B5 → Column B, Row 5

---

### **2.2 Selecting Cells**

* **Single Cell:** Click the cell or use arrow keys to navigate.
* **Range of Cells:** Click and drag or use **SHIFT + Arrow keys**.

  * Example: To select B2\:B6 → Click B2, then drag down to B6 OR SHIFT + ↓ 4 times.
* **Entire Row:** Click the row number on the left.
* **Entire Column:** Click the column letter at the top.
* **Entire Worksheet:** Press **CTRL + A**.

---

### **2.3 Moving Between Cells**

* **Arrow keys:** Move one cell in the direction of the arrow.
* **CTRL + Arrow key:** Jump to the **next edge of the data**.

  * CTRL + ↓ → last filled cell in the column
  * CTRL + ↑ → first filled cell in the column
  * CTRL + → → last filled cell in the row
  * CTRL + ← → first filled cell in the row

**Mini-Practice:**

1. Enter employee names in B2\:B10
2. Use **↓ arrow** to move one cell down
3. Use **CTRL + ↓** to jump to the last name

---

### **2.4 Selecting Multiple Cells**

* **SHIFT + Arrow keys:** Select multiple cells in the arrow direction.

  * SHIFT + ↓ → select down
  * SHIFT + → → select right
* **CTRL + SHIFT + Arrow keys:** Select **all contiguous filled cells** in the direction of the arrow.

**Example:**

* Active cell = B2, data exists till B20
* CTRL + SHIFT + ↓ → selects B2\:B20 automatically

---

### **2.5 Inserting and Deleting Cells**

* **Insert Cell:** Right-click → Insert → Shift cells right / down
* **Delete Cell:** Right-click → Delete → Shift cells left / up
* **Insert Row:** Right-click row number → Insert
* **Delete Row:** Right-click row number → Delete
* **Insert Column:** Right-click column letter → Insert
* **Delete Column:** Right-click column letter → Delete

**Mini-Practice:**

1. Insert a new column for `Department` between Name and Base Salary.
2. Insert a new row for a new employee.

---

### **2.6 Copying, Cutting, and Pasting Cells**

* **Copy:** CTRL + C → select destination → CTRL + V
* **Cut:** CTRL + X → select destination → CTRL + V
* **Paste Special:** Right-click → Paste Special → Values, Formulas, Formats

**Practice:** Copy employee salary data to the Salary sheet.

---

### **2.7 AutoFill Feature**

* Drag the **fill handle** (small square at the bottom-right corner of a cell) to:

  * Copy values
  * Fill series (numbers, dates, text patterns)

**Example:**

* Employee ID 101 in A2 → drag down → auto-increments 101, 102, 103…

---

## **3. Rows in Excel**

### **3.1 Selecting Rows**

* Click row number → entire row selected
* CTRL + SHIFT + ↑/↓ → select multiple rows

### **3.2 Inserting Rows**

* Right-click row number → Insert → new blank row appears above selected row

### **3.3 Deleting Rows**

* Right-click row number → Delete → removes the row

**Practice:**

1. Insert a new row at 5 for a new employee.
2. Delete the last row after testing.

---

## **4. Columns in Excel**

### **4.1 Selecting Columns**

* Click column letter → entire column selected
* CTRL + SHIFT + → / ← → select multiple columns

### **4.2 Inserting Columns**

* Right-click column letter → Insert → new blank column inserted to the left

### **4.3 Deleting Columns**

* Right-click column letter → Delete → removes the column

**Practice:**

1. Insert a new column for `Bonus` between Base Salary and Total Compensation
2. Delete a column after practice

---

## **5. Tips for Efficient Navigation**

* **CTRL + HOME:** Go to first cell (A1)
* **CTRL + END:** Go to last filled cell
* **PAGE UP / PAGE DOWN:** Move one screen up/down
* **ALT + PAGE UP / ALT + PAGE DOWN:** Move screen left/right
* **Name Box:** Type cell reference → jump to any cell instantly

---

## **6. Mini Exercises – Navigation & Cells**

1. Open a workbook → rename sheets `Employee_Data` and `Salary`.
2. Enter 10 employees with columns: ID, Name, DOB, Base Salary.
3. Use arrow keys, CTRL + arrows, SHIFT + arrows to navigate and select.
4. Insert a new column for Department.
5. Insert a new row for a new employee.
6. Use AutoFill to create Employee IDs automatically.
7. Copy Base Salary to Salary sheet.
8. Delete the last row and column after checking.

---
