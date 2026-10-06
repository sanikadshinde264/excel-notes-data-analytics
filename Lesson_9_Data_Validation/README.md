# ✅ Data Validation in Excel

**Data Validation** in Microsoft Excel is used to control what type of data users can enter into a cell.

It helps maintain **accurate, consistent, and error-free data** in a worksheet.

The SORT formula can be combined with Data Validation to create a dynamic drop-down list.

Data Validation is available from:

```text
Data → Data Validation
```

---

# 1️⃣ 📊 Data Validation

### Steps to Open Data Validation

1. Select the cell or range of cells.
2. Go to the **Data** tab.
3. Select **Data Validation**.
4. Set the required validation criteria.

```text
Data → Data Validation
```

---

# 2️⃣ ⚙️ Data Validation Settings

The **Settings** tab is used to define what type of data can be entered into the selected cells.

The main validation criteria include:

* Whole Number
* Decimal
* List
* Date
* Time
* Text Length
* Custom

---

# 3️⃣ 📋 List Validation

The **List** option is used to create a **drop-down list** in a cell.

### Steps

1. Select the cell.
2. Go to:

```text
Data → Data Validation
```

3. Under **Allow**, select:

```text
List
```

4. Enter the values in the **Source** box.
5. Click **OK/Done**.

### Example

For a days list:

```text
Sunday,Monday,Tuesday,Wednesday,Thursday,Friday,Saturday
```

The selected cell will now display a drop-down list.

---

# 4️⃣ 📅 Create a Drop-Down List for Days

You can create a drop-down list containing all days of the week.

### Method 1: Enter Values Directly

In the Data Validation **Source** box, enter:

```text
Sunday,Monday,Tuesday,Wednesday,Thursday,Friday,Saturday
```

The cell will show a drop-down arrow.

Example:

```text
┌─────────────────┐
│ Monday       ▼  │
└─────────────────┘
```

---

# 5️⃣ 📋 Create a List Using Cells

Instead of typing the values directly into the Source box, you can store the list in cells.

Example:

| A         |
| --------- |
| Sunday    |
| Monday    |
| Tuesday   |
| Wednesday |
| Thursday  |
| Friday    |
| Saturday  |

Then select the cell where you want the drop-down.

Go to:

```text
Data → Data Validation → List
```

For **Source**, select:

```excel
=$A$1:$A$7
```

Now the drop-down will use the values from those cells.

---

# 6️⃣ 🖱️ Create a Day List Quickly

Another simple method is to type:

```text
Sunday
```

in one cell and drag the **fill handle** downward.

Excel can automatically continue the series:

```text
Sunday
Monday
Tuesday
Wednesday
Thursday
Friday
Saturday
```

This is useful for quickly creating a list of days.

---

# 7️⃣ 📝 Input Message

The **Input Message** option displays instructions to the user when they select the validated cell.

### Purpose

It gives users information about what they should enter or select.

Example:

```text
Title:
Select Day

Input Message:
Please select a day from the drop-down list.
```

### Steps

Go to:

```text
Data → Data Validation → Input Message
```

Then enter:

* **Title**
* **Input Message**

---

# 8️⃣ ⚠️ Error Alert

The **Error Alert** option displays a message when a user enters invalid data.

### Purpose

It prevents or warns users about incorrect entries.

Go to:

```text
Data → Data Validation → Error Alert
```

You can specify:

* **Style**
* **Title**
* **Error Message**

### Example

```text
Title:
Invalid Day

Error Message:
Please select a valid day from the drop-down list.
```

---

# 9️⃣ 🚨 Error Alert Styles

Excel provides different error alert styles.

### Stop

Prevents the user from entering invalid data.

```text
Stop → Invalid entry is not accepted
```

### Warning

Displays a warning but may allow the user to continue.

```text
Warning → User can choose whether to continue
```

### Information

Displays an informational message.

```text
Information → Shows information about the entry
```

---

# 🔟 📋 Custom List

A **Custom List** allows you to create your own predefined order of values.

For example:

```text
Sunday
Monday
Tuesday
Wednesday
Thursday
Friday
Saturday
```

You can also create custom lists such as:

```text
High
Medium
Low
```

or:

```text
Beginner
Intermediate
Advanced
```

---

# 1️⃣1️⃣ 🛠️ Creating a Custom List

In desktop Excel, custom lists can be managed from Excel Options.

Typical path:

```text
File
  ↓
Options
  ↓
Advanced
  ↓
General
  ↓
Edit Custom Lists
```

Then:

1. Select **NEW LIST**.
2. Enter your custom values.
3. Click **Add**.
4. Click **OK**.

### Example Custom List

```text
Sunday
Monday
Tuesday
Wednesday
Thursday
Friday
Saturday
```

Excel can then recognize this as a custom sequence.

---

# 1️⃣2️⃣ 🔃 Custom List and Sorting

Custom Lists are especially useful when sorting data in a specific order.

For example, normal alphabetical sorting might produce:

```text
Friday
Monday
Saturday
Sunday
Thursday
Tuesday
Wednesday
```

But a **Custom List** can maintain the correct day order:

```text
Sunday
Monday
Tuesday
Wednesday
Thursday
Friday
Saturday
```

This is useful for:

* Days of the week
* Months
* Priority levels
* Business categories
* Custom statuses

---

# 1️⃣3️⃣ 🔢 Data Validation Criteria

Data Validation can restrict different types of values.

| Criteria     | Purpose                   |
| ------------ | ------------------------- |
| Whole Number | Allows whole numbers      |
| Decimal      | Allows decimal numbers    |
| List         | Creates a drop-down list  |
| Date         | Allows valid dates        |
| Time         | Allows valid times        |
| Text Length  | Controls text length      |
| Custom       | Uses a formula-based rule |

---

# 1️⃣4️⃣ 🧮 Custom Validation

The **Custom** option allows you to create a validation rule using a formula.

For example, to allow only values greater than 10:

```excel
=A1>10
```

The formula determines whether the entered value is valid.

Custom validation is useful when the standard validation options are not enough.

---

# 1️⃣5️⃣ 💡 Example: Day Drop-Down

Suppose you want users to select only a day of the week.

### Step 1

Select the cell:

```text
B2
```

### Step 2

Go to:

```text
Data → Data Validation
```

### Step 3

Select:

```text
Allow → List
```

### Step 4

Enter:

```text
Sunday,Monday,Tuesday,Wednesday,Thursday,Friday,Saturday
```

### Step 5

Click:

```text
OK / Done
```

Now **B2** will contain a drop-down list of days.

---

# 1️⃣6️⃣ ⚠️ Spill Error

A **#SPILL!** error can occur when a dynamic array formula tries to return multiple results but the cells where the results should appear are not empty.

### Example

If you use:

```excel
=SORT(A2:A10)
```

Excel may need multiple cells to display the results.

If another value is already present in the required output area, Excel may show:

```text
#SPILL!
```

### Solution

Check the cells where the formula needs to spill and remove any blocking data.

---

