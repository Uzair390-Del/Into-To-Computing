# 📊 Week 4: Spreadsheet Tools – Basics & Intermediate (MS Excel / Google Sheets)

This lecture-lab covers **spreadsheet software**, the most widely used tool for organizing, calculating, analyzing, and reporting data in business and academic settings. You will start from the very basics (entering data and simple formulas) and move to business-level skills (IF, COUNTIF, lookups, validation, filtering, sorting).

> 🎯 **CLO-3:** Use productivity software tools (spreadsheets) to organize, analyze, and present data for practical business problems.

---

## 📌 Lab Overview

| Item                 | Details                                                         |
| -------------------- | --------------------------------------------------------------- |
| **Course**           | Introduction to Computing                                       |
| **Topic**            | Spreadsheet Tools (Basics + Intermediate)                       |
| **Tools**            | MS Excel (2016 or later / Microsoft 365) **or** Google Sheets   |
| **Estimated time**   | 3 hours (can be split into two lab sessions)                    |
| **Difficulty**       | Beginner → Intermediate                                         |
| **Files you create** | `Lab4_Gradebook` and `Lab4_Sales_Report` (spreadsheet files)    |

### 🎓 Learning Objectives

By the end of this lab, you will be able to:

1. Explain what a spreadsheet is and identify its main components.
2. Enter, edit, and format data in cells, rows, and columns.
3. Apply **conditional formatting** to highlight important values automatically.
4. Use **SUM, AVERAGE, MAX, MIN** (and COUNT) to summarize data.
5. Use business functions: **IF, COUNTIF, SUMIF, VLOOKUP, XLOOKUP**.
6. Restrict and control input using **data validation** (drop-downs, number limits).
7. Use **filters** and **sorting** to prepare clean business reports.

### 🗺️ Lab Roadmap

| Part  | Section                                      | Approx. Time |
| ----- | -------------------------------------------- | ------------ |
| **A** | 22. Introduction to Spreadsheets             | 15 min       |
| **A** | 23. Entering Data & Formatting Cells         | 25 min       |
| **A** | 24. Conditional Formatting                   | 20 min       |
| **A** | 25. Basic Formulas (SUM, AVERAGE, MAX, MIN)  | 35 min       |
| **B** | 26. Business Functions (IF, COUNTIF, Lookup) | 45 min       |
| **B** | 27. Data Validation                          | 20 min       |
| **B** | 28. Filtering Techniques                     | 15 min       |
| **B** | 29. Sorting Data for Business Reports        | 15 min       |
| —     | 30. Common Errors & Troubleshooting          | 10 min       |
| —     | 31. Practice Tasks, Quiz & Recap             | 20 min       |

---

# 🅰️ PART A: SPREADSHEET BASICS

---

## 22. Introduction to Spreadsheets

### What is a Spreadsheet?

A **spreadsheet** is a software tool that organizes data in a grid of **rows and columns** and lets you perform **calculations automatically** using formulas. If data changes, results update instantly, with no need to recalculate by hand.

### Popular Spreadsheet Tools

| Tool               | Type                                              | Key Advantage                                              |
| ------------------ | ------------------------------------------------- | ---------------------------------------------------------- |
| **Microsoft Excel** | Desktop/offline (cloud sync via Microsoft 365)    | Industry standard, powerful analysis, huge function library |
| **Google Sheets**  | Cloud-based, browser                              | Free, real-time collaboration, auto-saves to Google Drive  |

| Feature                  | MS Excel                       | Google Sheets                    |
| ------------------------ | ------------------------------ | -------------------------------- |
| Works offline            | ✅ Yes                          | ⚠️ Limited (needs setup)         |
| Real-time collaboration  | ⚠️ Needs OneDrive/365           | ✅ Built-in                       |
| Cost                     | Paid (or one-time license)     | Free                             |
| Large datasets           | ✅ Handles very large files     | ⚠️ Slows down with huge data      |
| Auto-save                | Needs OneDrive/AutoSave on     | ✅ Automatic                      |
| File format              | `.xlsx`                        | Saved in Drive (export as `.xlsx`) |

### Anatomy of a Spreadsheet

| Term                  | Meaning                                                                 | Example               |
| --------------------- | ----------------------------------------------------------------------- | --------------------- |
| **Workbook**          | The whole file (Excel) / "Spreadsheet" (Sheets); can hold many sheets   | `Lab4_Gradebook.xlsx` |
| **Worksheet (Sheet)** | A single tab inside the workbook                                        | `Sheet1`              |
| **Cell**              | The box where a row and column meet; the smallest unit holding data     | `B3`                  |
| **Cell Address**      | Column letter + Row number                                              | `C5` = column C, row 5 |
| **Row**               | Horizontal line of cells, labeled with numbers                          | Row 1, 2, 3...        |
| **Column**            | Vertical line of cells, labeled with letters                            | A, B, C...            |
| **Range**             | A group of cells                                                        | `B2:B11`              |
| **Formula Bar**       | Shows the real content of the selected cell (value or formula)          | `=SUM(B2:B11)`        |
| **Name Box**          | Shows the address of the selected cell; type an address to jump there   | `D7`                  |
| **Active Cell**       | The cell currently selected (highlighted border)                        | -                     |
| **Fill Handle**       | Small square at the bottom-right corner of a cell; drag to copy/extend  | -                     |

### Types of Data in a Cell

| Data Type   | Description                  | Example           | Default Alignment |
| ----------- | ---------------------------- | ----------------- | ----------------- |
| **Text**    | Letters/words (labels)       | `Ali Khan`        | Left              |
| **Number**  | Numeric values               | `78`, `1200.50`   | Right             |
| **Date**    | Calendar date                | `2026-01-05`      | Right             |
| **Formula** | Starts with `=`              | `=B2+C2`          | Shows result      |
| **Boolean** | TRUE / FALSE                 | `TRUE`            | Center            |

> 💡 **Quick check:** If your number is aligned to the **left**, Excel/Sheets is probably treating it as **text**. Calculations on it may fail.

### Real-Life Uses of Spreadsheets

- 🏫 Student gradebooks and attendance sheets
- 🛒 Sales reports and inventory tracking
- 💰 Personal/household budgeting
- 👥 Employee records and payroll
- 📈 Charts and dashboards for management

### ✋ Hands-On Activity 22.1: Explore Your Workspace

1. Open **MS Excel** (Blank workbook) **or** go to [sheets.google.com](https://sheets.google.com) → **Blank spreadsheet**.
2. Click cell **C5** and read its address in the **Name Box**.
3. Type `D10` in the Name Box and press **Enter**. Notice where you land.
4. Click and drag from **A1** to **D4** to select a range. What does the Name Box (or status bar) show?
5. Rename `Sheet1` to **Gradebook** (right-click the tab → **Rename**, or double-click the tab).
6. Save the file as **Lab4_Gradebook**.

---

## 23. Entering Data & Formatting Cells

### 23.1 Entering Data

**Basic rules:**

- Click a cell and just start typing.
- Press **Enter** → confirm and move **down**; **Tab** → confirm and move **right**; **Esc** → cancel.
- To edit a cell later: double-click it or press **F2**.
- Always put **one type of data per column** and **headings in the first row**.

**Best practices for a clean table:**

| ✅ Do                                          | ❌ Don't                                           |
| ---------------------------------------------- | ------------------------------------------------- |
| Use one header row with clear names            | Leave blank rows/columns inside your data          |
| Keep one value per cell                        | Type "78 marks" (mix number + text)               |
| Keep the same data type in each column         | Merge cells inside the data table                  |
| Use consistent spelling (e.g., always "North") | Mix "north", "North ", "NORTH"                     |

### 23.2 Auto-Fill (Fill Handle)

The **fill handle** saves typing:

| You type                | Drag the fill handle → you get      |
| ----------------------- | ----------------------------------- |
| `1` and `2` (select both) | `3, 4, 5, 6...`                   |
| `Monday`                | `Tuesday, Wednesday...`             |
| `Jan`                   | `Feb, Mar, Apr...`                  |
| A formula               | Same formula copied to other rows (references adjust) |

**Shortcut:** Double-click the fill handle to auto-fill down as far as the adjacent column has data.

### 23.3 Formatting Cells

Formatting improves readability and professionalism. Find the tools in the **Home** tab (Excel) or the **toolbar** (Sheets).

| Tool                        | What it does                                         | Shortcut (Excel / Sheets) |
| --------------------------- | ---------------------------------------------------- | ------------------------- |
| **Bold / Italic / Underline** | Emphasize text                                    | `Ctrl+B / I / U`          |
| **Font & Font size**        | Change text style and size                           | -                         |
| **Text / Fill color**       | Change font color or cell background                 | -                         |
| **Borders**                 | Draw lines around cells                              | -                         |
| **Alignment**               | Left, Center, Right, Top, Middle, Bottom             | -                         |
| **Wrap Text**               | Show long text on multiple lines inside one cell     | -                         |
| **Merge & Center**          | Combine cells into one (use for titles only)         | -                         |
| **Number Format**           | Show data as currency, percentage, date, decimals    | -                         |
| **Column width / Row height** | Resize to fit content (double-click the border)    | -                         |
| **Freeze Panes**            | Keep header row visible while scrolling              | View → Freeze             |

### 23.4 Number Formats

| Format         | Before        | After          | When to use                     |
| -------------- | ------------- | -------------- | ------------------------------- |
| **General**    | `85000`       | `85000`        | Default                         |
| **Number**     | `85000`       | `85,000.00`    | Quantities with decimals/commas |
| **Currency**   | `85000`       | `Rs 85,000`    | Prices, salaries                |
| **Percentage** | `0.85`        | `85%`          | Rates, discounts                |
| **Date**       | `46027`       | `05-Jan-2026`  | Dates                           |
| **Text**       | `00123`       | `00123`        | Phone numbers, IDs with leading zeros |

> 💡 **Tip:** Format changes only how data **looks**, not the actual value stored in the cell.

> 📌 **Rs / PKR currency:** In Excel use **Format Cells → Number → Currency → Symbol: Rs** (or *Custom*: `"Rs" #,##0`). In Sheets use **Format → Number → Custom currencies**.

### ✋ Hands-On Activity 23.1: Build the Student Gradebook

In your **Gradebook** sheet, type the following data starting at **A1**:

| Roll No | Name          | Math | English | Computer | Physics |
| ------- | ------------- | ---- | ------- | -------- | ------- |
| 1       | Ali Khan      | 78   | 65      | 90       | 72      |
| 2       | Sara Ahmed    | 92   | 88      | 95       | 85      |
| 3       | Usman Tariq   | 45   | 52      | 60       | 48      |
| 4       | Ayesha Noor   | 85   | 91      | 78       | 80      |
| 5       | Hamza Sheikh  | 33   | 40      | 55       | 38      |
| 6       | Fatima Zahra  | 67   | 74      | 82       | 70      |
| 7       | Bilal Hussain | 58   | 49      | 64       | 55      |
| 8       | Zainab Malik  | 96   | 94      | 98       | 91      |
| 9       | Omar Farooq   | 71   | 68      | 75       | 66      |
| 10      | Hina Raza     | 49   | 61      | 58       | 52      |

**Now format it:**

1. **Header row (A1:F1):** Bold, white font, dark blue fill, centered.
2. **Whole table (A1:F11):** Add **All Borders**.
3. **Marks columns (C2:F11):** Center-align.
4. **Column widths:** Select all columns → double-click a column border to **AutoFit**.
5. **Freeze the header row:** *View → Freeze Panes → Freeze Top Row* (Sheets: *View → Freeze → 1 row*).
6. **Insert a title:** Insert a new row above row 1, type `Class Gradebook – Semester 1` in A1, merge **A1:F1**, center it, and use font size 16 bold.

> ✅ **Checkpoint:** Your table should now look neat and professional, with the header stuck at the top when you scroll.

---

## 24. Conditional Formatting

### What is Conditional Formatting?

**Conditional formatting** automatically changes the **appearance of cells** (color, font, icons) **based on their values**. It helps you spot patterns, problems, and top performers at a glance, without reading every number.

### Where to find it

| Tool         | Location                                                     |
| ------------ | ------------------------------------------------------------ |
| **Excel**    | **Home → Conditional Formatting**                            |
| **Sheets**   | **Format → Conditional formatting** (opens a side panel)     |

### Types of Rules

| Rule Type                   | What it does                                             | Example Use                          |
| --------------------------- | -------------------------------------------------------- | ------------------------------------ |
| **Highlight Cells Rules**   | Color cells that are `>`, `<`, `=`, between, contain text, duplicates | Marks below 50 → red   |
| **Top/Bottom Rules**        | Highlight top 10 items, bottom 10%, above average        | Top 3 students                       |
| **Data Bars** (Excel)       | Adds in-cell bars proportional to value                  | Compare sales visually               |
| **Color Scales**            | Gradient colors from low → high                          | Heat-map of marks                    |
| **Icon Sets** (Excel)       | Arrows, traffic lights, stars                            | 🔴🟡🟢 performance status           |
| **Custom Formula**          | Highlight based on your own formula                      | Highlight entire row if Status = "Pending" |

### ✋ Hands-On Activity 24.1: Highlight Failing and Excellent Marks

**Task 1: Failing marks (below 50) in red**

*Excel:*
1. Select **C3:F12** (the marks cells; adjust if you did not add a title row).
2. **Home → Conditional Formatting → Highlight Cells Rules → Less Than...**
3. Enter `50`, choose **Light Red Fill with Dark Red Text** → **OK**.

*Google Sheets:*
1. Select the marks range → **Format → Conditional formatting**.
2. *Format cells if...* → **Less than** → value `50`.
3. Choose a red fill → **Done**.

**Task 2: Excellent marks (85 or above) in green**

1. Select the same range.
2. Add a new rule: **Greater Than or Equal To** `85` → **Green Fill with Dark Green Text**.

**Task 3: Color scale on one subject**

1. Select only the **Math** column.
2. *Excel:* **Conditional Formatting → Color Scales → Green-Yellow-Red**.
   *Sheets:* **Conditional formatting → Color scale** tab.

**Task 4 (Excel): Data bars on the Computer column**

1. Select the **Computer** column → **Conditional Formatting → Data Bars → Gradient Fill**.

**Task 5: Highlight an entire row using a custom formula** *(Intermediate)*

Goal: Highlight the whole row of the student whose Math marks are below 40.

1. Select **A3:F12**.
2. *Excel:* **Conditional Formatting → New Rule → Use a formula to determine which cells to format**.
   *Sheets:* **Conditional formatting → Custom formula is**.
3. Enter the formula: `=$C3<40`
4. Choose a yellow fill → **OK**.

> 💡 **Why `$C3`?** The `$` locks the **column** so every cell in the row checks column C, while the row number changes for each row.

### Managing Rules

| Action              | Excel                                                  |
| ------------------- | ------------------------------------------------------ |
| View/edit all rules | **Conditional Formatting → Manage Rules**              |
| Delete rules        | **Conditional Formatting → Clear Rules**               |
| Rule priority       | Use the up/down arrows in *Manage Rules*               |

### ✅ Expected Result (check yourself)

- Red cells should appear for: Usman (Math 45, Physics 48), Hamza (Math 33, English 40, Physics 38), Bilal (English 49), Hina (Math 49).
- Green cells should appear for: Ali (Computer 90), Sara (all four), Ayesha (Math 85, English 91), and Zainab (all four).

---

## 25. Basic Formulas: SUM, AVERAGE, MAX, MIN

### 25.1 What is a Formula?

A **formula** is an instruction that tells the spreadsheet to calculate something. **Every formula starts with an equals sign (`=`).**

```
=B2+C2          → adds two cells
=B2*C2          → multiplies
=(B2+C2)/2      → uses brackets for order of operations
=SUM(B2:B11)    → uses a function
```

### 25.2 Arithmetic Operators

| Operator | Meaning        | Example     | Result (if A1=10, B1=2) |
| -------- | -------------- | ----------- | ----------------------- |
| `+`      | Addition       | `=A1+B1`    | 12                      |
| `-`      | Subtraction    | `=A1-B1`    | 8                       |
| `*`      | Multiplication | `=A1*B1`    | 20                      |
| `/`      | Division       | `=A1/B1`    | 5                       |
| `^`      | Power          | `=A1^B1`    | 100                     |
| `%`      | Percent        | `=A1*10%`   | 1                       |

**Order of operations (BODMAS):** Brackets → Orders (powers) → Division/Multiplication → Addition/Subtraction.

### 25.3 What is a Function?

A **function** is a ready-made formula. Structure:

```
=FUNCTION_NAME(argument1, argument2, ...)
```

Example: `=SUM(C2:F2)`, where `SUM` is the function name and `C2:F2` is the argument (a range).

### 25.4 The Four Basic Functions

| Function      | Purpose                         | Syntax                 | Example              |
| ------------- | ------------------------------- | ---------------------- | -------------------- |
| **SUM**       | Adds all numbers in a range     | `=SUM(range)`          | `=SUM(C2:F2)`        |
| **AVERAGE**   | Calculates the mean             | `=AVERAGE(range)`      | `=AVERAGE(C2:F2)`    |
| **MAX**       | Finds the largest value         | `=MAX(range)`          | `=MAX(C2:C11)`       |
| **MIN**       | Finds the smallest value        | `=MIN(range)`          | `=MIN(C2:C11)`       |

**Bonus helpers:**

| Function      | Purpose                                      | Example              |
| ------------- | -------------------------------------------- | -------------------- |
| **COUNT**     | Counts cells that contain **numbers**        | `=COUNT(C2:C11)`     |
| **COUNTA**    | Counts **non-empty** cells                   | `=COUNTA(B2:B11)`    |
| **ROUND**     | Rounds a number to given decimals            | `=ROUND(G2,1)`       |

### 25.5 Ways to Enter a Function

1. **Type it:** `=SUM(` then select the range with the mouse, type `)` and press Enter.
2. **AutoSum (Excel):** Select a cell below/next to numbers → **Home → AutoSum (Σ)**.
3. **Insert Function:** **Formulas → Insert Function** (Excel) / **Insert → Function** (Sheets).
4. **Select range first** and look at the **status bar** (Excel) for a quick Sum/Average/Count preview.

### 25.6 Cell References: Relative vs Absolute

This is **one of the most important concepts** in spreadsheets.

| Type         | Looks like | Behavior when copied                      | Use case                         |
| ------------ | ---------- | ----------------------------------------- | -------------------------------- |
| **Relative** | `B2`       | Changes automatically (`B2`→`B3`→`B4`)    | Row-by-row calculations          |
| **Absolute** | `$B$2`     | Never changes                             | Fixed value like tax rate        |
| **Mixed**    | `$B2` / `B$2` | Locks only the column / only the row   | Tables and custom formulas       |

> ⌨️ Press **F4** (Excel) while editing a reference to cycle through `B2 → $B$2 → B$2 → $B2`.

**Example:** If tax rate is in cell `H1` and price in `B2`:
```
=B2*$H$1     ← copy this down; B2 changes, $H$1 stays fixed ✅
=B2*H1       ← copy this down; H1 becomes H2, H3... ❌ (wrong results)
```

### ✋ Hands-On Activity 25.1: Calculate Totals and Averages per Student

Add new headers in **G** and **H** (assuming data in rows 3–12 under your title row; if you skipped the title row, rows are 2–11):

| Cell | Heading   | Formula (for first student, row 3) |
| ---- | --------- | ---------------------------------- |
| G2   | **Total**   | `=SUM(C3:F3)`                    |
| H2   | **Average** | `=AVERAGE(C3:F3)`                |

1. Type the formulas in **G3** and **H3**.
2. Select **G3:H3** and **double-click the fill handle** to copy the formulas down to row 12.
3. Format **H3:H12** to **2 decimal places** (or use `=ROUND(AVERAGE(C3:F3),2)`).

### ✋ Hands-On Activity 25.2: Summary Statistics Row

Below the table (row 14 onward), create a summary block:

| Cell | Label           | Formula (for Math column C) |
| ---- | --------------- | --------------------------- |
| B14  | **Class Total**   | `=SUM(C3:C12)`            |
| B15  | **Class Average** | `=AVERAGE(C3:C12)`        |
| B16  | **Highest Marks** | `=MAX(C3:C12)`            |
| B17  | **Lowest Marks**  | `=MIN(C3:C12)`            |

Write the formulas in column **C**, then **drag right** (fill handle) across to column **F** so Math, English, Computer, and Physics are all calculated.

### ✅ Answer Key for Activity 25.1 & 25.2

**Per student:**

| Roll No | Name          | Total | Average |
| ------- | ------------- | ----- | ------- |
| 1       | Ali Khan      | 305   | 76.25   |
| 2       | Sara Ahmed    | 360   | 90.00   |
| 3       | Usman Tariq   | 205   | 51.25   |
| 4       | Ayesha Noor   | 334   | 83.50   |
| 5       | Hamza Sheikh  | 166   | 41.50   |
| 6       | Fatima Zahra  | 293   | 73.25   |
| 7       | Bilal Hussain | 226   | 56.50   |
| 8       | Zainab Malik  | 379   | 94.75   |
| 9       | Omar Farooq   | 280   | 70.00   |
| 10      | Hina Raza     | 220   | 55.00   |

**Class statistics:**

| Statistic | Math | English | Computer | Physics |
| --------- | ---- | ------- | -------- | ------- |
| Total     | 674  | 682     | 755      | 657     |
| Average   | 67.4 | 68.2    | 75.5     | 65.7    |
| Highest   | 96   | 94      | 98       | 91      |
| Lowest    | 33   | 40      | 55       | 38      |

> ✅ **Self-check:** The sum of all student totals (G3:G12) must equal the sum of the four subject totals = **2768**.

### 💡 Quick Tips for Formulas

- A range uses a **colon** (`C2:C11`); separate individual cells with a **comma** (`=SUM(C2, E2, G2)`).
- Function names are **not case-sensitive** (`=sum(...)` works).
- Use **cell references instead of typing numbers**, so results update automatically when data changes.
- Click a formula cell and press **F2** to see colored boxes showing which cells it uses.
- To show all formulas on screen: *Excel:* `Ctrl + `` ` (backtick). *Sheets:* **View → Show → All formulas**.

---

# 🅱️ PART B: SPREADSHEET INTERMEDIATE

> Part B uses a new dataset. Create a **new file** named **Lab4_Sales_Report** with three sheets: **Sales**, **Products**, and **Employees**.

### ✋ Setup Activity: Create the Sales Dataset

**Sheet 1: rename to `Sales`.** Type this data starting from **A1**:

| A: Order ID | B: Date    | C: Salesperson | D: Region | E: Product | F: Qty | G: Unit Price | H: Status |
| ----------- | ---------- | -------------- | --------- | ---------- | ------ | ------------- | --------- |
| 1001        | 2026-01-05 | Ahmed          | North     | Laptop     | 2      | 85000         | Delivered |
| 1002        | 2026-01-07 | Sana           | South     | Mouse      | 15     | 1200          | Delivered |
| 1003        | 2026-01-09 | Bilal          | East      | Keyboard   | 8      | 2500          | Pending   |
| 1004        | 2026-01-12 | Ahmed          | North     | Monitor    | 4      | 32000         | Delivered |
| 1005        | 2026-01-15 | Sana           | West      | Laptop     | 1      | 85000         | Cancelled |
| 1006        | 2026-01-18 | Ayesha         | East      | Printer    | 3      | 28000         | Delivered |
| 1007        | 2026-01-21 | Bilal          | South     | Mouse      | 25     | 1200          | Delivered |
| 1008        | 2026-01-24 | Ayesha         | West      | Monitor    | 2      | 32000         | Pending   |
| 1009        | 2026-01-27 | Ahmed          | East      | Keyboard   | 10     | 2500          | Delivered |
| 1010        | 2026-01-30 | Sana           | North     | Printer    | 2      | 28000         | Delivered |
| 1011        | 2026-02-02 | Bilal          | West      | Laptop     | 3      | 85000         | Delivered |
| 1012        | 2026-02-05 | Ayesha         | South     | Monitor    | 5      | 32000         | Cancelled |

**Add a Total column:**

| Cell | Heading   | Formula              |
| ---- | --------- | -------------------- |
| I1   | **Total** | `=F2*G2` (fill down to row 13) |

**Sheet 2: rename to `Products`:**

| A: Product | B: Category | C: Warranty (Months) |
| ---------- | ----------- | -------------------- |
| Laptop     | Computers   | 24                   |
| Monitor    | Displays    | 12                   |
| Mouse      | Accessories | 6                    |
| Keyboard   | Accessories | 6                    |
| Printer    | Peripherals | 12                   |

**Sheet 3: rename to `Employees`:**

| A: Salesperson | B: Employee ID | C: Monthly Target |
| -------------- | -------------- | ----------------- |
| Ahmed          | E101           | 300000            |
| Sana           | E102           | 150000            |
| Bilal          | E103           | 250000            |
| Ayesha         | E104           | 200000            |

> ✅ **Checkpoint:** The sum of all values in `Sales!I2:I13` should be **1,095,000**.

> 💡 **Tip:** Format the Date column as a proper date (*Format Cells → Date*), the Unit Price and Total as currency, and apply the same professional header style you learned in Part A.

---

## 26. Business Functions: IF, COUNTIF, VLOOKUP / XLOOKUP

### 26.1 Logical Test Basics

Many business decisions are "if this, then that." Spreadsheets handle these using **comparison operators**:

| Operator | Meaning                  | Example         |
| -------- | ------------------------ | --------------- |
| `=`      | Equal to                 | `A1="Pending"`  |
| `>`      | Greater than             | `A1>100000`     |
| `<`      | Less than                | `A1<50`         |
| `>=`     | Greater than or equal to | `A1>=50`        |
| `<=`     | Less than or equal to    | `A1<=50`        |
| `<>`     | Not equal to             | `A1<>"Cancelled"` |

A comparison returns **TRUE** or **FALSE**. Text in formulas must be inside **double quotes** (`"Delivered"`).

---

### 26.2 The IF Function

**Purpose:** Returns one value if a condition is TRUE, another if FALSE.

```
=IF(logical_test, value_if_true, value_if_false)
```

**Example 1: Pass/Fail (Gradebook):**
```
=IF(H3>=50, "Pass", "Fail")
```

**Example 2: Order priority (Sales):**
```
=IF(I2>=100000, "High Value", "Standard")
```

**Example 3: Nested IF (multiple conditions), assign grades:**
```
=IF(H3>=80, "A", IF(H3>=70, "B", IF(H3>=60, "C", IF(H3>=50, "D", "F"))))
```

> 🧠 **How nested IF reads:** *If average ≥ 80 → "A"; otherwise if ≥ 70 → "B"; otherwise if ≥ 60 → "C"; otherwise if ≥ 50 → "D"; otherwise "F".* Always test from the **highest** to the **lowest**.

**Combining conditions with AND / OR:**

| Function | Meaning                          | Example                                          |
| -------- | -------------------------------- | ------------------------------------------------ |
| `AND`    | **All** conditions must be true  | `=IF(AND(H2="Delivered", I2>=100000), "Big Win", "-")` |
| `OR`     | **At least one** must be true    | `=IF(OR(H2="Pending", H2="Cancelled"), "Follow Up", "OK")` |

#### ✋ Hands-On Activity 26.1: IF Practice

**In the `Sales` sheet:**

| Cell | Heading         | Formula (row 2)                                           |
| ---- | --------------- | --------------------------------------------------------- |
| J1   | **Order Size**  | `=IF(I2>=100000,"High Value","Standard")`                 |
| K1   | **Action**      | `=IF(H2="Pending","Follow Up",IF(H2="Cancelled","Review","OK"))` |
| L1   | **Commission**  | `=IF(H2="Delivered", I2*5%, 0)`                           |

Fill all formulas down to row 13.

**In the `Gradebook` sheet:**

| Cell | Heading    | Formula (row 3)                                                         |
| ---- | ---------- | ----------------------------------------------------------------------- |
| I2   | **Result** | `=IF(H3>=50,"Pass","Fail")`                                             |
| J2   | **Grade**  | `=IF(H3>=90,"A+",IF(H3>=80,"A",IF(H3>=70,"B",IF(H3>=60,"C",IF(H3>=50,"D","F")))))` |

✅ **Answer check (Gradebook):** Only **Hamza Sheikh (41.50)** should show **Fail**. Grades: Ali = B, Sara = A+, Usman = D, Ayesha = A, Hamza = F, Fatima = B, Bilal = D, Zainab = A+, Omar = B, Hina = D.

✅ **Answer check (Sales):** **4** orders should be "High Value" (1001, 1004, 1011, 1012). **2** orders = "Follow Up", **2** orders = "Review".

---

### 26.3 COUNTIF, COUNTIFS, SUMIF, SUMIFS, AVERAGEIF

These functions **count, add, or average only the cells that meet a condition.** They are essential for business reports.

| Function         | Purpose                                         | Syntax                                                   |
| ---------------- | ----------------------------------------------- | -------------------------------------------------------- |
| **COUNTIF**      | Count cells meeting **one** condition           | `=COUNTIF(range, criteria)`                              |
| **COUNTIFS**     | Count cells meeting **multiple** conditions     | `=COUNTIFS(range1, crit1, range2, crit2)`                |
| **SUMIF**        | Add values meeting one condition                | `=SUMIF(criteria_range, criteria, sum_range)`            |
| **SUMIFS**       | Add values meeting multiple conditions          | `=SUMIFS(sum_range, crit_range1, crit1, crit_range2, crit2)` |
| **AVERAGEIF**    | Average values meeting one condition            | `=AVERAGEIF(criteria_range, criteria, average_range)`    |

**Criteria examples:**

| You want...               | Criteria to write |
| ------------------------- | ----------------- |
| Exactly "Delivered"       | `"Delivered"`     |
| Greater than 100000       | `">100000"`       |
| Not equal to "Cancelled"  | `"<>Cancelled"`   |
| Text starts with "A"      | `"A*"`            |
| Value from another cell   | `A20` or `">"&A20` |

#### ✋ Hands-On Activity 26.2: Sales Summary Dashboard

Create a new sheet named **Summary** and build this report (formulas refer to the `Sales` sheet):

| Question                                   | Formula                                                  | Expected Answer |
| ------------------------------------------ | -------------------------------------------------------- | --------------- |
| Total number of orders                     | `=COUNTA(Sales!A2:A13)`                                  | 12              |
| Number of **Delivered** orders             | `=COUNTIF(Sales!H2:H13,"Delivered")`                     | 8               |
| Number of **Pending** orders               | `=COUNTIF(Sales!H2:H13,"Pending")`                       | 2               |
| Number of **Cancelled** orders             | `=COUNTIF(Sales!H2:H13,"Cancelled")`                     | 2               |
| Orders from the **North** region           | `=COUNTIF(Sales!D2:D13,"North")`                         | 3               |
| Total sales of **Delivered** orders        | `=SUMIF(Sales!H2:H13,"Delivered",Sales!I2:I13)`          | 766,000         |
| Total sales by **Ahmed** (all statuses)    | `=SUMIF(Sales!C2:C13,"Ahmed",Sales!I2:I13)`              | 323,000         |
| Delivered orders by **Ahmed**              | `=COUNTIFS(Sales!C2:C13,"Ahmed",Sales!H2:H13,"Delivered")` | 3             |
| Delivered sales in the **West** region     | `=SUMIFS(Sales!I2:I13,Sales!D2:D13,"West",Sales!H2:H13,"Delivered")` | 255,000 |
| Orders worth **more than 100,000**         | `=COUNTIF(Sales!I2:I13,">100000")`                       | 4               |
| Average value of Delivered orders          | `=AVERAGEIF(Sales!H2:H13,"Delivered",Sales!I2:I13)`      | 95,750          |

> 💡 **Pro tip:** Put the label (e.g., "Delivered") in a cell like `A5` and use `=COUNTIF(Sales!H2:H13, A5)`. Now you can change the label without editing the formula!

#### ✋ Hands-On Activity 26.3: Salesperson Performance Table

Build a mini table on the `Summary` sheet:

| Salesperson | Orders (COUNTIF) | Total Sales (SUMIF) | Delivered Sales (SUMIFS) |
| ----------- | ---------------- | ------------------- | ------------------------ |
| Ahmed       | ?                | ?                   | ?                        |
| Sana        | ?                | ?                   | ?                        |
| Bilal       | ?                | ?                   | ?                        |
| Ayesha      | ?                | ?                   | ?                        |

Use the name cell (e.g., `A20`) as the criteria and **lock the ranges with `$`** so you can fill down:

```
=COUNTIF(Sales!$C$2:$C$13, A20)
=SUMIF(Sales!$C$2:$C$13, A20, Sales!$I$2:$I$13)
=SUMIFS(Sales!$I$2:$I$13, Sales!$C$2:$C$13, A20, Sales!$H$2:$H$13, "Delivered")
```

✅ **Answer check:**

| Salesperson | Orders | Total Sales | Delivered Sales |
| ----------- | ------ | ----------- | --------------- |
| Ahmed       | 3      | 323,000     | 323,000         |
| Sana        | 3      | 159,000     | 74,000          |
| Bilal       | 3      | 305,000     | 285,000         |
| Ayesha      | 3      | 308,000     | 84,000          |

---

### 26.4 Lookup Functions: VLOOKUP and XLOOKUP

**Lookup functions** search for a value in one table and return related information from another. Example: given a product name, find its category or warranty period.

#### VLOOKUP (Vertical Lookup)

```
=VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])
```

| Argument           | Meaning                                                                 |
| ------------------ | ----------------------------------------------------------------------- |
| **lookup_value**   | The value you are searching for (e.g., `E2`, the product name)          |
| **table_array**    | The table to search in. The **first column** must hold the lookup value |
| **col_index_num**  | Which column of the table to return (1 = first column, 2 = second...)   |
| **range_lookup**   | `FALSE` (or `0`) = **exact match** ✅ ; `TRUE` = approximate match      |

**Example:** Find the category of each product in the Sales sheet:

```
=VLOOKUP(E2, Products!$A$2:$C$6, 2, FALSE)
```

*Read it as:* "Look for the product in E2 in the first column of Products!A2:C6, and return the value from the **2nd column** (Category), exact match only."

**⚠️ VLOOKUP limitations:**

- Can only look **to the right** (the lookup column must be the left-most).
- Breaks if you insert/delete columns (the column number becomes wrong).
- Always use `FALSE` for exact matches, otherwise you may get wrong answers silently.

#### XLOOKUP (Modern Replacement)

> ✅ **Available in:** Excel 2021 / Excel for Microsoft 365, and Google Sheets.
> ❌ **Not available in:** Excel 2016 / 2019. Use VLOOKUP there.

```
=XLOOKUP(lookup_value, lookup_array, return_array, [if_not_found], [match_mode])
```

| Argument           | Meaning                                                       |
| ------------------ | ------------------------------------------------------------- |
| **lookup_value**   | What you are searching for                                    |
| **lookup_array**   | The single column/row to search in                            |
| **return_array**   | The single column/row to return results from                  |
| **if_not_found**   | (Optional) Custom message instead of `#N/A`                   |
| **match_mode**     | (Optional) 0 = exact (default), -1 = exact or next smaller, 1 = exact or next larger |

**Example:**
```
=XLOOKUP(E2, Products!$A$2:$A$6, Products!$B$2:$B$6, "Not found")
```

#### VLOOKUP vs XLOOKUP

| Feature                      | VLOOKUP                    | XLOOKUP                       |
| ---------------------------- | -------------------------- | ----------------------------- |
| Default match                | Approximate (risky)        | **Exact** (safer)             |
| Look to the left             | ❌ No                       | ✅ Yes                         |
| Column number needed         | ✅ Yes (breaks on insertion)| ❌ No (select return column)   |
| Built-in "not found" message | ❌ Needs `IFERROR`          | ✅ Yes                         |
| Works in older Excel         | ✅ Yes                      | ❌ No (2021/365 only)          |

#### ✋ Hands-On Activity 26.4: Exact-Match Lookups

In the `Sales` sheet add:

| Cell | Heading                   | Formula (row 2)                                                          |
| ---- | ------------------------- | ------------------------------------------------------------------------ |
| M1   | **Category** *(VLOOKUP)*  | `=VLOOKUP(E2,Products!$A$2:$C$6,2,FALSE)`                                |
| N1   | **Warranty (Months)** *(VLOOKUP)* | `=VLOOKUP(E2,Products!$A$2:$C$6,3,FALSE)`                        |
| O1   | **Employee ID** *(XLOOKUP)* | `=XLOOKUP(C2,Employees!$A$2:$A$5,Employees!$B$2:$B$5,"Not found")`     |

Fill down to row 13. ✅ **Check:** Row 2 (Laptop, Ahmed) should return **Computers**, **24**, **E101**.

> 📌 **If your Excel does not support XLOOKUP**, use `=VLOOKUP(C2,Employees!$A$2:$B$5,2,FALSE)` instead.

#### ✋ Hands-On Activity 26.5: Approximate-Match Lookup (Grade Table)

A classic business use of `VLOOKUP(..., TRUE)` is a **range-based lookup**. Create a grade table on the `Gradebook` sheet in **L2:M8**:

| L: Minimum Average | M: Grade |
| ------------------ | -------- |
| 0                  | F        |
| 50                 | D        |
| 60                 | C        |
| 70                 | B        |
| 80                 | A        |
| 90                 | A+       |

Then in **K2** (heading `Grade (Lookup)`) use:

```
=VLOOKUP(H3,$L$3:$M$8,2,TRUE)
```

> ⚠️ For approximate match, the first column of the table **must be sorted in ascending order**. Compare the result with your nested IF from Activity 26.1; they should be identical!

#### ✋ Hands-On Activity 26.6: Handling Errors with IFERROR

Try `=VLOOKUP("Tablet", Products!$A$2:$C$6, 2, FALSE)`. You get **`#N/A`** because "Tablet" doesn't exist. Make it friendlier:

```
=IFERROR(VLOOKUP("Tablet", Products!$A$2:$C$6, 2, FALSE), "Product not listed")
```

**Syntax:** `=IFERROR(formula, value_if_error)`

---

## 27. Data Validation

### What is Data Validation?

**Data validation** controls **what users are allowed to type** into a cell. It prevents typing mistakes ("Delivred" instead of "Delivered"), impossible numbers (negative quantity), and inconsistent data, which makes your reports reliable.

### Where to find it

| Tool         | Location                                       |
| ------------ | ---------------------------------------------- |
| **Excel**    | **Data → Data Validation → Data Validation...** |
| **Sheets**   | **Data → Data validation → Add rule**          |

### Common Validation Types

| Type                | What it restricts                           | Example Use                           |
| ------------------- | ------------------------------------------- | ------------------------------------- |
| **List**            | Only values from a drop-down list           | Status: Delivered / Pending / Cancelled |
| **Whole Number**    | Integers within limits                      | Quantity between 1 and 1000           |
| **Decimal**         | Numbers with decimals within limits         | Discount between 0 and 0.5            |
| **Date**            | Dates within a range                        | Order date in 2026 only               |
| **Text Length**     | Number of characters                        | ID must be exactly 4 characters       |
| **Custom Formula**  | Any rule you can write as a formula         | No duplicate Order IDs                |

### The Three Tabs (Excel)

| Tab               | Purpose                                                       |
| ----------------- | ------------------------------------------------------------- |
| **Settings**      | Define the rule (what's allowed)                              |
| **Input Message** | A hint that appears when the cell is selected                 |
| **Error Alert**   | The message shown when invalid data is typed (**Stop / Warning / Information**) |

### ✋ Hands-On Activity 27.1: Drop-Down List for Status

1. In the `Sales` sheet, select **H2:H13** (and extend to H50 if you expect more orders).
2. *Excel:* **Data → Data Validation** → *Allow:* **List** → *Source:* `Delivered,Pending,Cancelled` → ensure **In-cell dropdown** is ticked → **OK**.
   *Sheets:* **Data → Data validation → Add rule** → *Criteria:* **Drop-down** → add the 3 options → **Done**.
3. Click on any cell in H and use the arrow to change a status.
4. Try typing `Shipped`. You should get an **error**.

### ✋ Hands-On Activity 27.2: Quantity Must Be a Whole Number from 1 to 1000

1. Select **F2:F13**.
2. *Allow:* **Whole number** → *Data:* **between** → *Minimum:* `1`, *Maximum:* `1000`.
3. **Input Message tab:** Title: `Quantity` | Message: `Enter a whole number between 1 and 1000`.
4. **Error Alert tab:** Style: **Stop** | Title: `Invalid Quantity` | Message: `Quantity must be a whole number from 1 to 1000.`
5. Test with `0`, `-5`, `2.5`, and `abc`; all must be rejected.

### ✋ Hands-On Activity 27.3: Date Validation

1. Select **B2:B13**.
2. *Allow:* **Date** → *between* `1/1/2026` and `12/31/2026`.
3. Add an error alert: `Please enter a valid 2026 date.`

### ✋ Hands-On Activity 27.4: Dynamic Drop-Down from a Range *(Intermediate)*

Make the **Salesperson** column (C) use the names stored in `Employees!A2:A5`:

1. Select **C2:C13** → **Data Validation** → *Allow:* **List**.
2. *Source:* `=Employees!$A$2:$A$5` (Excel). In Sheets choose **Drop-down (from a range)** and select that range.
3. Add a new employee in the Employees sheet. Notice that you must extend the source range (or convert it to a **Table** in Excel for automatic growth).

### ✋ Hands-On Activity 27.5: Prevent Duplicate Order IDs *(Custom Formula)*

1. Select **A2:A50**.
2. *Allow:* **Custom** → *Formula:* `=COUNTIF($A$2:$A$50,A2)=1`
3. Test by typing `1001` in an empty cell, which should be rejected.

### Useful Extras

| Task                                    | How                                                                 |
| --------------------------------------- | ------------------------------------------------------------------- |
| Circle existing invalid data (Excel)    | **Data Validation → Circle Invalid Data**                           |
| Remove validation                       | **Data Validation → Clear All**                                     |
| Copy validation to other cells          | Copy the cell → **Paste Special → Validation**                      |

> ⚠️ **Limitation:** Validation does **not** check data that was already typed or **pasted** in (pasting can overwrite rules). Always test after pasting.

---

## 28. Filtering Techniques

### What is Filtering?

**Filtering** temporarily **hides rows that don't match your criteria**, so you can focus on specific data. The hidden data is **not deleted**; it comes back when you clear the filter.

### Turning Filters On

| Tool         | Steps                                                                                           |
| ------------ | ----------------------------------------------------------------------------------------------- |
| **Excel**    | Click any cell in the table → **Data → Filter** (or `Ctrl+Shift+L`)                             |
| **Sheets**   | Click any cell in the data → **Data → Create a filter** (or click the funnel icon ▼ in the toolbar) |

Drop-down arrows appear in each header cell.

### Filter Options

| Filter Type              | Available for | Example                                       |
| ------------------------ | ------------- | --------------------------------------------- |
| **Select values**        | All columns   | Show only `North` and `East`                  |
| **Text filters**         | Text          | Begins with, Ends with, Contains              |
| **Number filters**       | Numbers       | Greater than, Between, Top 10, Above Average  |
| **Date filters**         | Dates         | This month, Last quarter, Between two dates   |
| **Filter by color**      | Any           | Show only red-highlighted cells               |
| **Search box**           | All           | Type part of a value to find it quickly       |

### ✋ Hands-On Activity 28.1: Basic Filtering

Go to the `Sales` sheet and complete the tasks. **Clear the filter after each task.**

| #  | Task                                              | Expected number of rows shown |
| -- | ------------------------------------------------- | ----------------------------- |
| 1  | Show only **Delivered** orders                    | 8                             |
| 2  | Show only orders from the **East** region         | 3                             |
| 3  | Show only orders by **Sana**                      | 3                             |
| 4  | Show orders where **Total > 100,000**             | 4                             |
| 5  | Show orders for **Laptop** **or** **Monitor**     | 6                             |
| 6  | Show orders with Qty **between 5 and 15**         | 4                             |

### ✋ Hands-On Activity 28.2: Multi-Column Filters

Filters on **different columns combine with AND**. Apply:

1. **Region = South** AND **Status = Delivered** → how many rows? (✅ Answer: **2**: orders 1002 and 1007)
2. **Salesperson = Ahmed** AND **Total ≥ 50,000** → (✅ Answer: **2**: orders 1001 and 1004)

### ✋ Hands-On Activity 28.3: Filter by Color

1. Add a conditional-format rule to **H2:H13** that colors **"Cancelled"** red and **"Pending"** yellow.
2. Open the filter on column H → **Filter by Color** → choose red.
3. You should see only the cancelled orders.

### ✋ Hands-On Activity 28.4: Use the Status Bar to Analyze Filtered Data (Excel)

1. Filter **Status = Delivered**.
2. Select the **Total** column (I2:I13). Look at the **status bar** at the bottom. It shows Sum, Average, and Count for **visible cells only** (Sum should be **766,000**).

> 💡 **Using SUBTOTAL for filtered data:** `=SUM()` adds hidden rows too, but `=SUBTOTAL(109, I2:I13)` adds **only visible rows**. Use `SUBTOTAL(103, A2:A13)` to count visible rows.

### Filter Views (Google Sheets only)

A **Filter View** (*Data → Filter views → Create new filter view*) lets you apply your own filter **without changing what other collaborators see**, and you can save it with a name.

### Advanced Filter vs. FILTER function

| Method                | Where             | Use                                              |
| --------------------- | ----------------- | ------------------------------------------------ |
| **AutoFilter**        | Both              | Quick, interactive hide/show                     |
| **Advanced Filter**   | Excel             | Complex criteria, copy results to another place  |
| **`=FILTER()` function** | Excel 365, Sheets | Returns matching rows live, e.g. `=FILTER(Sales!A2:I13, Sales!H2:H13="Delivered")` |

### Removing Filters

- Clear one column: click the filter ▼ → **Clear Filter**.
- Clear all: **Data → Clear** (Excel) / **Data → Remove filter** (Sheets).

---

## 29. Sorting Data for Business Reports

### What is Sorting?

**Sorting** rearranges the **rows** of your data in a specific order based on one or more columns. Sorted data is much easier to read, compare, and present in reports.

### Sort Orders

| Data Type | Ascending (A → Z)        | Descending (Z → A)       |
| --------- | ------------------------ | ------------------------ |
| Text      | A → Z                    | Z → A                    |
| Numbers   | Smallest → Largest       | Largest → Smallest       |
| Dates     | Oldest → Newest          | Newest → Oldest          |

### How to Sort

| Tool         | Quick Sort                                                                   | Multi-level Sort                                      |
| ------------ | ---------------------------------------------------------------------------- | ----------------------------------------------------- |
| **Excel**    | Click a cell in the column → **Data → Sort A→Z / Z→A**                       | **Data → Sort** → *Add Level*                         |
| **Sheets**   | Right-click a column header → **Sort sheet A→Z / Z→A**                       | **Data → Sort range → Advanced range sorting options** |

> ⚠️ **Golden Rule:** Always sort the **entire table**, not just one column. Sorting only one column **scrambles** the connection between data (e.g., Ali's name would end up with Sara's marks!). In Excel, click **one cell inside the table**; Excel will select the full table automatically. Check that **"My data has headers"** is ticked.

### Types of Sorting

| Type               | Description                                                          | Example                                  |
| ------------------ | -------------------------------------------------------------------- | ---------------------------------------- |
| **Single-level**   | Sort by one column                                                   | Highest Total first                      |
| **Multi-level**    | Sort by several columns in priority order                            | Region (A→Z), then Total (Largest→Smallest) |
| **Custom list**    | Sort in your own order instead of alphabetical                       | Status: Pending → Delivered → Cancelled  |
| **By color**       | Sort by fill or font color                                           | Red cells on top                         |

### ✋ Hands-On Activity 29.1: Single-Level Sorting

On the `Sales` sheet:

1. Sort by **Total (Largest to Smallest)**. Which order is on top? (✅ **1011**, Rs 255,000)
2. Sort by **Date (Oldest to Newest)** to restore the original order.
3. Sort by **Salesperson (A to Z)**.

### ✋ Hands-On Activity 29.2: Multi-Level Sorting for a Regional Report

*Excel:* **Data → Sort** → click **Add Level** to build:

| Level | Sort by      | Order                |
| ----- | ------------ | -------------------- |
| 1     | **Region**   | A to Z               |
| 2     | **Status**   | A to Z               |
| 3     | **Total**    | Largest to Smallest  |

*Sheets:* **Data → Sort range → Advanced range sorting options** → tick *Data has header row* → add the same three sort columns.

**Business meaning:** Management sees each region together, with each status grouped, and the biggest orders at the top of every group.

### ✋ Hands-On Activity 29.3: Custom Sort Order (Excel)

1. **Data → Sort** → *Sort by:* **Status** → *Order:* **Custom List...**
2. In *List entries* type (one per line): `Pending`, `Delivered`, `Cancelled` → **Add** → **OK**.
3. Pending orders (needing action) are now on top.

### ✋ Hands-On Activity 29.4: Sort the Gradebook into a Merit List

1. Go to the `Gradebook` sheet, select the full student table (A2:K12), and sort by **Total (Largest to Smallest)**.
2. Add a **Position** column using the formula `=RANK(G3,$G$3:$G$12)` *(or `RANK.EQ`)* **before** sorting to make ranks stay with each student.

✅ **Expected top 3:** 1st **Zainab Malik (379)**, 2nd **Sara Ahmed (360)**, 3rd **Ayesha Noor (334)**.

### 📊 Sorting + Filtering Together: A Mini Business Report

**Scenario:** Your manager asks: *"Give me all delivered orders, biggest first."*

1. Filter **Status = Delivered**.
2. Sort the filtered data by **Total (Largest to Smallest)**.
3. Check that the top 3 are **1011 (255,000)**, **1001 (170,000)**, **1004 (128,000)**.

### Tips for Report-Ready Sorting

- 💾 **Save a copy** before a big sort (or use **Undo** `Ctrl+Z` immediately if something looks wrong).
- 🔢 If numbers sort strangely (e.g., 100 before 25), they are stored as **text**; convert them to numbers first.
- 🧹 Remove extra **spaces** in names (`TRIM` function) so values sort/filter correctly.
- 🧾 Formulas with **relative references** to other rows can change after sorting; test the results.

---

## 30. Common Errors & Troubleshooting

### Error Codes

| Error          | Meaning                                    | Typical Cause                                          | Fix                                              |
| -------------- | ------------------------------------------ | ------------------------------------------------------ | ------------------------------------------------ |
| `#DIV/0!`      | Division by zero                           | `=A1/B1` where B1 is 0 or blank                        | Use `=IF(B1=0,"",A1/B1)` or `IFERROR`            |
| `#NAME?`       | Unrecognized function/name                 | Typo (`=SUMM(...)`), missing quotes around text        | Check spelling; add quotes around text           |
| `#VALUE!`      | Wrong data type in a formula               | Adding text to a number (`=A1+B1` with text in B1)     | Check cell contents                              |
| `#REF!`        | Invalid cell reference                     | The referenced cell/column was deleted                 | Fix the formula to point to a valid range        |
| `#N/A`         | Value not found                            | Lookup value doesn't exist in the table                | Check spelling/spaces; use `IFERROR`             |
| `#####`        | Column too narrow to display the value     | Number or date is wider than the column                | Widen the column (double-click the border)       |

### Common Student Mistakes

| Mistake                                              | Result                                    | Solution                                         |
| ---------------------------------------------------- | ----------------------------------------- | ------------------------------------------------ |
| Forgetting `=` at the start                          | Formula displays as plain text            | Start every formula with `=`                     |
| Typing text criteria without quotes                  | `#NAME?`                                  | `=COUNTIF(H2:H13,"Delivered")`                   |
| Using VLOOKUP without `FALSE`                        | Wrong/unpredictable result                | Always add `,FALSE` for exact matches            |
| Not locking ranges (`$`) when copying lookups        | `#N/A` or wrong values after fill-down    | Use `$A$2:$C$6`                                  |
| Sorting only one column                              | Data gets mixed up                        | Sort the whole table with headers                |
| Extra spaces in cells ("North ")                     | COUNTIF/VLOOKUP don't match               | Use `=TRIM()` or Find & Replace                  |
| Numbers stored as text                               | SUM ignores them                          | Convert to numbers (Data → Text to Columns, or multiply by 1) |
| Typing a comma instead of semicolon (regional settings) | Formula error on some computers        | Use the list separator your region uses (`,` or `;`) |

### Handy Keyboard Shortcuts

| Action                            | Windows Excel        | Google Sheets          |
| --------------------------------- | -------------------- | ---------------------- |
| Save                              | `Ctrl + S`           | Auto-saves             |
| Select entire column / row        | `Ctrl + Space` / `Shift + Space` | Same       |
| Select all data in table          | `Ctrl + A`           | `Ctrl + A`             |
| Jump to end of data               | `Ctrl + Arrow Keys`  | `Ctrl + Arrow Keys`    |
| Edit active cell                  | `F2`                 | `F2`                   |
| Cycle absolute/relative reference | `F4`                 | `F4`                   |
| AutoSum                           | `Alt + =`            | -                      |
| Copy formula from cell above      | `Ctrl + D`           | `Ctrl + D`             |
| Insert row/column                 | `Ctrl + Shift + +`   | `Ctrl + Alt + +`       |
| Toggle filter                     | `Ctrl + Shift + L`   | `Ctrl + Shift + L`     |
| Undo / Redo                       | `Ctrl + Z / Y`       | `Ctrl + Z / Y`         |

---

## 31. Practice Tasks, Quiz & Recap

### 🏋️ Practice Task 1: Personal Monthly Budget (Basics)

Create a new sheet with this data and complete the tasks:

| Category      | Jan   | Feb   | Mar   | Total | Average |
| ------------- | ----- | ----- | ----- | ----- | ------- |
| Rent          | 25000 | 25000 | 25000 |       |         |
| Groceries     | 18000 | 16500 | 19200 |       |         |
| Transport     | 6000  | 5500  | 7200  |       |         |
| Utilities     | 9500  | 8800  | 7600  |       |         |
| Entertainment | 4000  | 6500  | 3000  |       |         |

**Tasks:**
1. Calculate **Total** and **Average** for each category (`SUM`, `AVERAGE`).
2. Calculate the **monthly total** in a new row at the bottom.
3. Find the **highest** and **lowest** single expense (`MAX`, `MIN`).
4. Apply **currency format** and use **conditional formatting** to highlight any expense above Rs 20,000 in orange.
5. Add a data bar on the Total column.

✅ **Check:** Monthly totals → Jan = **62,500**, Feb = **62,300**, Mar = **62,000**. Highest expense = **25,000**, lowest = **3,000**.

### 🏋️ Practice Task 2: Employee Records (Intermediate)

Create this table:

| Emp ID | Name    | Department | Salary | Years of Service |
| ------ | ------- | ---------- | ------ | ---------------- |
| E01    | Kamran  | IT         | 85000  | 6                |
| E02    | Rabia   | HR         | 62000  | 3                |
| E03    | Danish  | Finance    | 74000  | 8                |
| E04    | Mehwish | IT         | 91000  | 10               |
| E05    | Taimoor | Marketing  | 58000  | 2                |
| E06    | Iqra    | Finance    | 69000  | 4                |
| E07    | Shahid  | HR         | 55000  | 1                |
| E08    | Nimra   | IT         | 78000  | 5                |

**Tasks:**
1. Add a **Bonus** column: `=IF(E2>=5, D2*10%, D2*5%)` (10% bonus for 5+ years, 5% otherwise).
2. Add a **Level** column using nested IF: Salary ≥ 85000 → "Senior", ≥ 65000 → "Mid", else "Junior".
3. Use **COUNTIF** to find how many employees are in **IT**.
4. Use **SUMIF** to find the total salary of the **Finance** department.
5. Use **AVERAGEIF** to find the average salary for **HR**.
6. Apply **data validation** to the Department column (drop-down with IT, HR, Finance, Marketing).
7. **Filter** to show only IT employees with salary above 80,000.
8. **Sort** by Department (A→Z) and then Salary (Largest→Smallest).

✅ **Check:** IT count = **3**; Finance total salary = **143,000**; HR average salary = **58,500**.

### 🏋️ Practice Task 3: Challenge, Mini Sales Report

Using your `Sales_Report` file, produce a **one-page management report** on the `Summary` sheet that includes:

- Total orders, delivered, pending, and cancelled counts
- Total sales per **region** (SUMIF) and per **salesperson**
- **Target achievement** for each salesperson: use `XLOOKUP`/`VLOOKUP` to fetch the Monthly Target from the `Employees` sheet, then:
  `=IF(DeliveredSales>=Target,"Target Met","Below Target")`
- Conditional formatting: green for "Target Met," red for "Below Target"
- A **chart** (Insert → Chart): bar/column chart of sales by salesperson
- Everything neatly **formatted**, with a **title**, and sorted by Total Sales (descending)

> 🌟 **Bonus:** Insert a **PivotTable** (Excel: *Insert → PivotTable*; Sheets: *Insert → Pivot table*) to summarize sales by Region and Product, and compare it with your formula-based answers.

### 🧠 Self-Assessment Quiz

**Q1.** What symbol must every formula start with?
**Q2.** What is the cell address of the cell in column D, row 7?
**Q3.** Which function finds the **largest** value in a range?
**Q4.** What does `$B$2` mean, and when would you use it?
**Q5.** Write a formula to give "Pass" if cell B2 ≥ 40, otherwise "Fail."
**Q6.** What is the difference between `COUNT` and `COUNTIF`?
**Q7.** In `=VLOOKUP(A2, D2:F10, 3, FALSE)`, what does `3` mean and what does `FALSE` mean?
**Q8.** Name **two** advantages of XLOOKUP over VLOOKUP.
**Q9.** What does data validation do, and give one example.
**Q10.** What is the difference between **sorting** and **filtering**?
**Q11.** Why can sorting a single column be dangerous?
**Q12.** What does the error `#N/A` usually mean in a lookup formula?

<details>
<summary>✅ Click to reveal answers</summary>

1. The equals sign `=`.
2. `D7`.
3. `MAX`.
4. An **absolute reference**: it stays fixed when copied. Use it for fixed values like a tax rate or a lookup range.
5. `=IF(B2>=40,"Pass","Fail")`
6. `COUNT` counts all numeric cells; `COUNTIF` counts only cells that meet a given condition.
7. `3` = return the value from the 3rd column of the table; `FALSE` = exact match only.
8. Any two: looks left or right, no column number needed, exact match by default, built-in "if not found" message, doesn't break when columns are inserted.
9. It restricts what can be entered in a cell, e.g., a drop-down list for Status or a number between 1 and 1000.
10. **Sorting** rearranges the order of rows; **filtering** hides rows that don't match criteria (without deleting them).
11. It breaks the connection between related data in a row (names get mismatched with their marks).
12. The lookup value was not found in the lookup table (typo, extra space, or it doesn't exist).

</details>

### 📋 Grading Rubric (Suggested, 20 Marks)

| Criteria                                                              | Marks |
| --------------------------------------------------------------------- | ----- |
| **Formatting**: headers, borders, number formats, freeze panes        | 3     |
| **Conditional formatting**: at least 3 correct rules                  | 3     |
| **Basic formulas**: SUM, AVERAGE, MAX, MIN used correctly             | 3     |
| **Business functions**: IF, COUNTIF/SUMIF, VLOOKUP/XLOOKUP            | 5     |
| **Data validation**: list + number rules with messages                | 2     |
| **Filtering and sorting** applied correctly to produce the report     | 2     |
| **Overall presentation** and accuracy of results                      | 2     |
| **Total**                                                             | **20** |

### 📤 Submission Checklist

- [ ] `Lab4_Gradebook` file with: formatting, conditional formatting, totals/averages, summary stats, Pass/Fail, and Grade columns
- [ ] `Lab4_Sales_Report` file with: Sales, Products, Employees, and Summary sheets
- [ ] Data validation set on Status, Quantity, and Date columns
- [ ] Filtered & sorted report screenshot (delivered orders, biggest first)
- [ ] Practice Tasks 1 and 2 completed (Task 3 is optional/bonus)
- [ ] File names follow the format: `RollNo_Name_Lab4.xlsx`

---

## 32. Week 4 Quick Recap

✅ A **spreadsheet** organizes data in rows, columns, and cells; the **cell address** (e.g., `B3`) identifies each cell
✅ **Formatting** (number formats, borders, colors, freeze panes) makes data readable; **conditional formatting** highlights values automatically
✅ Formulas begin with `=`; the four essentials are **SUM, AVERAGE, MAX, MIN**
✅ **Relative** (`B2`), **absolute** (`$B$2`), and **mixed** (`$B2`) references control how formulas behave when copied
✅ **IF** makes decisions; **COUNTIF / SUMIF / AVERAGEIF** summarize data by condition
✅ **VLOOKUP / XLOOKUP** fetch related data from another table (always use **exact match** unless you need ranges)
✅ **Data validation** prevents bad data using lists, number limits, dates, and custom rules
✅ **Filters** hide unwanted rows; **sorting** orders rows (single- or multi-level), and together they create report-ready data

### 🧾 Function Cheat Sheet

| Function      | Syntax                                          | Purpose                          |
| ------------- | ----------------------------------------------- | -------------------------------- |
| `SUM`         | `=SUM(range)`                                   | Add numbers                      |
| `AVERAGE`     | `=AVERAGE(range)`                               | Mean of numbers                  |
| `MAX` / `MIN` | `=MAX(range)` / `=MIN(range)`                   | Largest / smallest value         |
| `COUNT`       | `=COUNT(range)`                                 | Count numeric cells              |
| `IF`          | `=IF(test, true_value, false_value)`            | Make a decision                  |
| `AND` / `OR`  | `=AND(test1, test2)`                            | Combine conditions               |
| `COUNTIF`     | `=COUNTIF(range, criteria)`                     | Count by condition               |
| `SUMIF`       | `=SUMIF(range, criteria, sum_range)`            | Add by condition                 |
| `SUMIFS`      | `=SUMIFS(sum_range, range1, crit1, range2, crit2)` | Add by multiple conditions    |
| `AVERAGEIF`   | `=AVERAGEIF(range, criteria, avg_range)`        | Average by condition             |
| `VLOOKUP`     | `=VLOOKUP(value, table, col, FALSE)`            | Look up (left → right)           |
| `XLOOKUP`     | `=XLOOKUP(value, lookup_col, return_col)`       | Modern lookup                    |
| `IFERROR`     | `=IFERROR(formula, "message")`                  | Replace errors with a message    |
| `RANK`        | `=RANK(number, range)`                          | Position in a list               |
| `ROUND`       | `=ROUND(number, digits)`                        | Round a number                   |
| `TRIM`        | `=TRIM(text)`                                   | Remove extra spaces              |

---

### 📚 Recommended Next Step

Take a real-life dataset (your own expenses, your class timetable, or a small shop's sales) and build a mini-report using **at least one function from each category**: calculation (SUM/AVERAGE), decision (IF), summary (COUNTIF/SUMIF), and lookup (VLOOKUP/XLOOKUP). Add validation to the input cells and finish with a filtered + sorted view. This is exactly how spreadsheets are used in real offices! 🚀

### 🔗 Helpful Resources

- [Microsoft Excel Help & Learning](https://support.microsoft.com/excel)
- [Google Sheets Help Center](https://support.google.com/docs/topic/9054603)
- [Google Sheets Function List](https://support.google.com/docs/table/25273)
