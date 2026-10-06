# 📋 Paste Special in Excel

**Paste Special** in Microsoft Excel allows you to control how copied data is pasted into another location.

It provides different options for pasting **formulas, values, formatting, links, pictures, validation, and more**.

---

# 1️⃣ 📋 Paste Options

The **Paste** options include:

* 🧮 Formulas
* 🔢 Formulas & Number Formatting
* 🎨 Keep Source Formatting
* 🚫 No Borders
* 📏 Keep Source Column Width
* 🔄 Transpose

## 🧮 Formulas

Pastes the **formulas** from the copied cells.

It does not copy the source formatting.

Example:

```excel
=A1+B1
```

---

## 🧮🔢 Formulas & Number Formatting

Pastes:

* Formulas
* Number formatting

It does not copy other source formatting such as colors and borders.

---

## 🎨 Keep Source Formatting

Pastes the data while keeping the **formatting of the source data**.

It can keep:

* Font
* Font color
* Fill color
* Borders
* Alignment
* Number formatting

---

## 🚫 No Borders

Pastes the copied data **without the source borders**.

This is useful when you do not want the borders from the source data to be copied.

---

## 📏 Keep Source Column Width

Pastes the data while keeping the **source column width**.

This is useful when you want the destination columns to have the same width as the source columns.

---

## 🔄 Transpose

Changes the orientation of the copied data.

```text
Rows → Columns
Columns → Rows
```

### Example

Before:

| Name   | Age | City |
| ------ | --: | ---- |
| Sanika |  21 | Pune |

After Transpose:

|      |        |
| ---- | ------ |
| Name | Sanika |
| Age  | 21     |
| City | Pune   |

---

# 2️⃣ 🔢 Paste Values

The **Paste Values** options include:

* 🔢 Values
* 🔢 Values & Number Formatting
* 🎨 Values & Source Formatting

## 🔢 Values

Pastes only the **final values**.

If the source contains:

```excel
=A1+B1
```

and the result is:

```text
15000
```

only `15000` is pasted.

The formula is not copied.

---

## 🔢 Values & Number Formatting

Pastes:

* Values
* Number formatting

The original formula is not pasted.

Example:

```text
15000.00
```

The value and its number format are copied.

---

## 🎨 Values & Source Formatting

Pastes:

* Values
* Source formatting

The original formula is not copied.

The source formatting is also maintained.

---

# 3️⃣ 🛠️ Other Paste Options

The **Other Paste Options** include:

* 🎨 Formatting
* 🔗 Paste Link
* 🖼️ Picture
* 🔗🖼️ Picture with Link

## 🎨 Formatting

Pastes only the **formatting** of the source cells.

It can include:

* Font
* Font color
* Fill color
* Borders
* Alignment
* Number formatting

The actual data is not pasted.

---

## 🔗 Paste Link

Creates a **link between the destination and source data**.

The destination refers to the original source cell.

If the source data changes, the linked result can update.

---

## 🖼️ Picture

Pastes the selected data as a **picture**.

The pasted content behaves like an image and can be moved or resized.

---

## 🔗🖼️ Picture with Link

Pastes the selected data as a **picture with a link to the original data**.

When the source data changes, the linked picture can update.

---

# 4️⃣ ⚙️ Paste Special

The **Paste Special** dialog box provides more detailed options.

It has two main sections:

## 4.1 📋 Paste

The **Paste** section contains:

* All
* Formulas
* Values
* Formats
* Comments
* Validation

### All

Pastes all available data and formatting from the source.

### Formulas

Pastes only formulas.

### Values

Pastes only values.

### Formats

Pastes only formatting.

### Comments

Pastes comments or notes.

### Validation

Pastes **Data Validation rules**, such as drop-down lists.

---

# 4.2 ➕ Operation

The **Operation** section allows you to perform calculations while pasting.

It contains:

* None
* Add
* Multiply
* Subtract
* Divide

### None

Pastes the data without performing a mathematical operation.

### Add

Adds the copied value to the destination value.

Example:

```text
Destination = 100
Copied Data = 50

Result = 150
```

### Multiply

Multiplies the destination value by the copied value.

```text
Destination = 100
Copied Data = 2

Result = 200
```

### Subtract

Subtracts the copied value from the destination value.

```text
Destination = 100
Copied Data = 20

Result = 80
```

### Divide

Divides the destination value by the copied value.

```text
Destination = 100
Copied Data = 2

Result = 50
```

---

# 📌 How to Use Operation

1. Select or copy the data containing the value.
2. Select the **particular destination cell or range**.
3. Open **Paste Special**.
4. Select the required operation.
5. Click **OK**.

```text
Select/Copy Data
       ↓
Select Destination Cell
       ↓
Paste Special
       ↓
Operation
       ↓
Add / Multiply / Subtract / Divide
       ↓
OK
```

---

# 📊 Complete Summary

| Section                     | Options                                                                                                         |
| --------------------------- | --------------------------------------------------------------------------------------------------------------- |
| 📋 Paste                    | Formulas, Formulas & Number Formatting, Keep Source Formatting, No Borders, Keep Source Column Width, Transpose |
| 🔢 Paste Values             | Values, Values & Number Formatting, Values & Source Formatting                                                  |
| 🛠️ Other Paste Options     | Formatting, Paste Link, Picture, Picture with Link                                                              |
| ⚙️ Paste Special → Paste    | All, Formulas, Values, Formats, Comments, Validation                                                            |
| ➕ Paste Special → Operation | None, Add, Multiply, Subtract, Divide                                                                           |

---

# ⭐ Quick Remember

```text
1️⃣ Paste Options
   → Formulas
   → Formulas & Number Formatting
   → Keep Source Formatting
   → No Borders
   → Keep Source Column Width
   → Transpose

2️⃣ Paste Values
   → Values
   → Values & Number Formatting
   → Values & Source Formatting

3️⃣ Other Paste Options
   → Formatting
   → Paste Link
   → Picture
   → Picture with Link

4️⃣ Paste Special
   → Paste
      → All
      → Formulas
      → Values
      → Formats
      → Comments
      → Validation

   → Operation
      → None
      → Add
      → Multiply
      → Subtract
      → Divide
```
