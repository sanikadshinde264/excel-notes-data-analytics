# 🔃 Sorting Data in Excel

**Sorting** in Microsoft Excel is used to arrange data in a specific order. It helps organize and analyze data easily.

Excel allows us to sort data in different ways, such as:

* A to Z
* Z to A
* Smallest to Largest
* Largest to Smallest
* By Cell Color
* By Font Color
* By Conditional Formatting Icon
* Using Multiple Sorting Levels

---

## 🌐 Office 365 Online Excel

**Office 365 Online Excel** can be used to practice Excel formulas and data analysis directly in a web browser.

---

# 1️⃣ Accessing the Sort Option

Excel provides sorting options mainly through the **Data** tab and **Home** tab.

### 📊 Data Tab

```text
Data → Sort & Filter → Sort
```

### 🏠 Home Tab

```text
Home → Sort & Filter
```

---

# 2️⃣ 🔤 Basic Sorting

Excel provides two quick sorting options.

## 🔼 Sort A to Z

Sorts text in **ascending order**.

```text
A → Z
```

For numbers:

```text
Smallest → Largest
```

## 🔽 Sort Z to A

Sorts text in **descending order**.

```text
Z → A
```

For numbers:

```text
Largest → Smallest
```

---

# 3️⃣ 📋 Sorting the Whole Dataset

When working with multiple columns, we should sort the **complete dataset** instead of sorting only one column.

### Steps

1. Select the column that you want to sort.
2. Choose **Sort A to Z** or **Sort Z to A**.
3. Excel may display the following option:

```text
Expand the selection
```

4. Select **Expand the selection**.
5. Click **Sort**.

### ⚠️ Important

Select **Expand the selection** when the data contains multiple related columns.

This keeps all the values belonging to the same record together.

### Example

Suppose the data is:

| Name | Department | Marks |
| ---- | ---------- | ----: |
| Amit | IT         |    80 |
| Neha | HR         |    90 |
| Ravi | IT         |    75 |

If we sort the **Marks** column, the complete rows should move together.

---

# 4️⃣ ⚙️ Advanced Sorting

For more control over sorting, use:

```text
Data → Sort
```

The **Sort** dialog box provides several options.

---

## 🔹 Sort By

Select the column that you want to sort.

Example:

```text
Sort by → Name
```

Other examples:

```text
Sort by → Department
Sort by → Salary
Sort by → Marks
```

---

## 🔹 Sort On

Excel allows data to be sorted based on different properties.

### 1. Cell Values

Sort according to the actual values in the cells.

```text
Sort On → Cell Values
```

### 2. Cell Color

Sort according to the background color of cells.

```text
Sort On → Cell Color
```

### 3. Font Color

Sort according to the font color.

```text
Sort On → Font Color
```

### 4. Conditional Formatting Icon

Sort according to icons created using conditional formatting.

```text
Sort On → Conditional Formatting Icon
```

---

# 5️⃣ 🔢 Sort Order

The available order depends on the type of data.

### For Text

```text
A to Z
Z to A
```

### For Numbers

```text
Smallest to Largest
Largest to Smallest
```

### Custom List

Excel also allows sorting according to a **Custom List**.

For example:

```text
High
Medium
Low
```

---

# 6️⃣ ➕ Multiple-Level Sorting

Excel allows us to apply more than one sorting condition.

Use:

```text
Data → Sort → Add Level
```

### Example

Suppose we have employee data.

We can sort it as:

```text
Sort by → Department
Then by → Name
Then by → Salary
```

Excel first sorts by **Department**. Within each department, it sorts by **Name**, and then by **Salary**.

### Example Structure

```text
Level 1 → Department
Level 2 → Name
Level 3 → Salary
```

This is useful when a dataset contains many categories and records.

---

# 7️⃣ 🎨 Sorting by Color

Excel can sort data based on formatting.

It supports:

* Cell Color
* Font Color
* Conditional Formatting Icon

### Example

```text
Data → Sort
     ↓
Sort On → Cell Color
```

Then select the required color and specify its order.

---

# 8️⃣ ↕️ Sort Orientation

Excel provides two main sorting orientations.

## 1. ⬇️ Sort Top to Bottom

This is the **normal sorting method**.

Data is sorted **down the columns**.

Example:

```text
A
B
C
D
```

This is the commonly used sorting direction.

---

## 2. ➡️ Sort Left to Right

This option sorts data **across rows** instead of down columns.

### Steps

```text
Data → Sort → Options
```

Select:

```text
Sort left to right
```

Then select the row that you want to sort.

---

# 9️⃣ 🔢 SORT Formula

Excel also provides the **SORT function** for sorting data using a formula.

### Syntax

```excel
=SORT(array,[sort_index],[sort_order],[by_col])
```

### Basic Example

```excel
=SORT(A2:H10)
```

This sorts the data in the range:

```text
A2:H10
```

---

# 🔟 SORT Function Arguments

The `SORT` function has four main arguments.

```text
SORT(array, sort_index, sort_order, by_col)
```

## 🔹 1. array

The range of data that you want to sort.

Example:

```excel
A2:H10
```

---

## 🔹 2. sort_index

Specifies which column or row should be used for sorting.

For example:

```text
1 → First column
2 → Second column
3 → Third column
```

Example:

```excel
=SORT(A2:H10,2)
```

This sorts the data based on the **second column**.

---

## 🔹 3. sort_order

Specifies the sorting direction.

```text
1  → Ascending
-1 → Descending
```

Example:

```excel
=SORT(A2:H10,2,-1)
```

This sorts the data based on the **second column in descending order**.

---

## 🔹 4. by_col

Specifies whether Excel should sort by rows or columns.

```text
FALSE → Sort by rows
TRUE  → Sort by columns
```

Example:

```excel
=SORT(A2:H10,2,1,FALSE)
```

This sorts the data by the second column in ascending order.

---

# 1️⃣1️⃣ SORT Formula with Headers

If your dataset contains headers, select the data range appropriately.

For example:

```text
Name | Department | Marks
Amit | IT         | 80
Neha | HR         | 90
Ravi | IT         | 75
```

You can copy the headers separately if required and apply the `SORT` formula to the data range.

Example:

```excel
=SORT(A2:C10,3,-1)
```

This sorts the data based on the **third column in descending order**.

---

