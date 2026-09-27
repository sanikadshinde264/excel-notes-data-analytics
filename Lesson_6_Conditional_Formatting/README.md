# 🎨 Conditional Formatting in Excel

Conditional Formatting is an Excel feature used to **automatically format cells based on specific conditions or rules**.

It helps to quickly identify important values, trends, duplicates, and patterns in a dataset.

---

## 1️⃣ Highlight Cells Rules

**Path:**

`Home → Conditional Formatting → Highlight Cells Rules`

These rules are used to highlight cells based on their values.

### 🔹 Available Rules

* ➕ **Greater Than** → Highlights values greater than a specified number.
* ➖ **Less Than** → Highlights values less than a specified number.
* 🔄 **Between** → Highlights values within a specified range.
* 🟰 **Equal To** → Highlights cells equal to a specified value.
* 🔤 **Text That Contains** → Highlights cells containing specific text.
* 📅 **A Date Occurring** → Highlights dates based on a selected date condition.
* 📋 **Duplicate Values** → Highlights duplicate or unique values.

---

# 2️⃣ 🏆 Top/Bottom Rules

These rules identify the highest, lowest, above-average, or below-average values.

### 🔝 Top Rules

* **Top 10 Items** → Highlights the top 10 values.
* **Top 10%** → Highlights values belonging to the top 10%.

### 🔻 Bottom Rules

* **Bottom 10 Items** → Highlights the lowest 10 values.
* **Bottom 10%** → Highlights values belonging to the bottom 10%.

### 📊 Average Rules

* **Above Average** → Highlights values above the average.
* **Below Average** → Highlights values below the average.

---

# 3️⃣ 📊 Data Bars

**Data Bars** display horizontal bars inside cells.

The length of the bar represents the relative value of the cell.

➡️ Higher value → Longer bar
➡️ Lower value → Shorter bar

---

# 4️⃣ 🌈 Color Scales

**Color Scales** use different colors to represent the magnitude of values.

For example:

```text
Low Value    →    Medium Value    →    High Value
```

This makes it easy to identify high and low values visually.

---

# 5️⃣ 🔔 Icon Sets

**Icon Sets** display icons in cells based on their values.

Examples include:

* 🟢 High value
* 🟡 Medium value
* 🔴 Low value

They are useful for quickly understanding the status or performance of data.

---

# 6️⃣ 🆕 New Rule

The **New Rule** option allows you to create a custom conditional formatting rule.

### 📌 Steps

1. Select the required **rows and columns**.
2. Go to **Home → Conditional Formatting**.
3. Click **New Rule**.
4. Select **"Use a formula to determine which cells to format."**
5. Enter your formula.
6. Click **Format**.
7. Select the required formatting.
8. Click **OK**.

### 💡 Example

Suppose column **D** contains product names and you want to highlight rows where the product is **Mouse**.

Formula:

```excel
=$D2="Mouse"
```

This formula checks whether the value in column D is `"Mouse"`.

If the condition is TRUE, the selected formatting is applied.

---

# 7️⃣ 🔗 Types of Cell References

When creating formulas, Excel supports different types of cell references.

### 1. 🔒 Absolute Reference

Example:

```excel
=$D$2
```

Both the **column and row are fixed**.

### 2. 🔄 Relative Reference

Example:

```excel
=D2
```

Both the **column and row can change** when the formula is copied.

### 3. 🔐 Mixed Reference

Examples:

```excel
=$D2
=D$2
```

* `$D2` → Column D is fixed, row can change.
* `D$2` → Row 2 is fixed, column can change.

---

# 8️⃣ 🗑️ Remove Conditional Formatting

To remove conditional formatting:

### Option 1: Clear Rules

Go to:

`Home → Conditional Formatting → Clear Rules`

You can choose:

* **Clear Rules from Selected Cells**
* **Clear Rules from Entire Sheet**

### Option 2: Manage Rules

Go to:

`Home → Conditional Formatting → Manage Rules`

From here, you can:

* ✏️ Edit a rule
* 🗑️ Delete a rule
* 🔼 Move a rule up
* 🔽 Move a rule down
* 👀 Change the range to which the rule applies

---
