# **Phase 1: Excel – Formatting (Detailed Notes)**

**Project Goal:** Learn to **format cells, numbers, text, dates, and apply conditional formatting** in your Employee Dataset for clarity and professional appearance.

---

## **1. Why Formatting is Important**

* Makes data **readable**
* Helps in **quick analysis**
* Ensures **professional presentation**
* Improves **accuracy** (e.g., correct number/date formatting prevents calculation errors)

---

## **2. Cell Formatting**

### **2.1 Font Formatting**

* **Font Type & Size:** Choose style (Calibri, Arial, Times New Roman) and size (e.g., 11, 12)
* **Bold / Italic / Underline:** Highlight headers or important values
* **Font Color:** Change text color for emphasis
* **Cell Fill (Background Color):** Highlight headers or specific rows/columns

**Example:**

* Header row (A1\:G1) → Bold, White font, Blue fill
* Bonus column → Green font if eligible

**Mini Practice:** Format Employee Dataset headers

---

### **2.2 Alignment**

* **Horizontal Alignment:** Left, Center, Right

  * Text → Left-aligned by default
  * Numbers → Right-aligned by default
* **Vertical Alignment:** Top, Middle, Bottom
* **Wrap Text:** Makes long text visible in a single cell
* **Merge & Center:** Combine multiple cells for titles

  * Example: Merge A1\:G1 → “Employee Management”

**Mini Practice:**

* Merge first row → Title of Dataset → Center + Bold + Font size 14
* Wrap Text for Department column

---

### **2.3 Number Formatting**

| Format     | Purpose                        | Example                          |
| ---------- | ------------------------------ | -------------------------------- |
| General    | Default                        | 12345                            |
| Number     | Add decimal places, separators | 12,345.00                        |
| Currency   | Show currency symbol           | ₹50,000.00                       |
| Accounting | Align currency symbols         | ₹ 50,000.00                      |
| Percentage | Convert to %                   | 0.85 → 85%                       |
| Scientific | Display in exponential         | 1230000 → 1.23E+06               |
| Custom     | Custom formatting              | “0” → round, “0.00” → 2 decimals |

**Mini Practice:**

* Base Salary → Currency
* Bonus → Number with 2 decimals
* Tax Rate → Percentage

---

### **2.4 Date & Time Formatting**

| Format     | Example                   | Display                   |
| ---------- | ------------------------- | ------------------------- |
| Short Date | 21/09/2025                | 21-Sep-25                 |
| Long Date  | Friday, 21 September 2025 | Friday, 21 September 2025 |
| Time       | 09:30:00                  | 9:30 AM                   |
| Custom     | dd-mmm-yyyy               | 21-Sep-2025               |

**Mini Practice:** Format DOB → Short Date, Joining Date → Long Date

---

### **2.5 Cell Borders**

* **Purpose:** Improve readability and separate data
* **How:** Home → Borders → Choose style

  * Example: Outline header row, draw gridlines around data

**Mini Practice:**

* Add thin borders around dataset
* Add thick border around header row

---

### **2.6 Conditional Formatting**

* **Definition:** Apply formatting automatically based on cell values
* **Types:**

  1. **Highlight Cell Rules:** Greater than, Less than, Equal to

     * Example: Base Salary > 60,000 → Green fill
  2. **Top/Bottom Rules:** Top 10 items, Bottom 10%
  3. **Data Bars:** Visual bar in cell representing value
  4. **Color Scales:** Gradient colors
  5. **Icon Sets:** Arrows, flags, traffic lights

**Mini Practice:**

* Highlight employees with Base Salary > 50,000 → Green fill
* Apply color scale to Bonus column

---

### **2.7 Tips for Efficient Formatting**

* Use **Format Painter** to copy formatting across cells
* **CTRL + 1** → Open Format Cells dialog (full options)
* Avoid excessive colors → keep it clean and professional
* Apply **styles** for headers → Home → Cell Styles

---

## **3. Mini Exercises – Formatting**

1. Apply **bold and color fill** to header row
2. Align all text and numbers correctly
3. Format **Base Salary and Bonus** → Currency
4. Format **DOB and Joining Date** → Correct date formats
5. Add **borders** around the dataset
6. Apply **conditional formatting** for high salaries and bonus eligibility
7. Use **Format Painter** to replicate header formatting on other sheets

---

✅ **Outcome:**

* Your Employee Dataset now looks **organized, professional, and easy to read**
* Formatting ensures **accuracy in calculations and clarity in reports**
* You’re ready for **next topics: Basic Formulas and Arithmetic Functions**
