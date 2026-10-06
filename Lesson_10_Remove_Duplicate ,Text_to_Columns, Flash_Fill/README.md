# 📊 Remove Duplicates, Text to Columns & Flash Fill in Excel

Excel provides useful **Data Tools** for cleaning, separating, and automatically filling data.

The important tools are:

* 🗑️ Remove Duplicates
* ✂️ Text to Columns
* ⚡ Flash Fill

These tools are available mainly under:

**Data → Data Tools**

---

# 1️⃣ 🗑️ Remove Duplicates

**Remove Duplicates** is used to remove repeated or duplicate records from a dataset.

### 📍 Path

**Data → Data Tools → Remove Duplicates**

### 📝 Example

| City-Pincode  |
| ------------- |
| Mumbai-400086 |
| Delhi-400001  |
| Pune-412701   |
| Mumbai-400086 |
| Thane-400059  |
| Pune-412701   |

Here, **Mumbai-400086** and **Pune-412701** are duplicated.

After using **Remove Duplicates**:

| City-Pincode  |
| ------------- |
| Mumbai-400086 |
| Delhi-400001  |
| Pune-412701   |
| Thane-400059  |

---

## 🔹 Steps to Remove Duplicates

1. Select the complete dataset.
2. Go to the **Data** tab.
3. Click **Remove Duplicates**.
4. A dialog box will appear.
5. Select the column or columns to check.
6. Click **OK**.
7. Excel removes the duplicate records.

### ⚠️ Important

If your data contains multiple columns, select the **complete table**.

When Excel asks:

**Expand the selection**
or
**Continue with the current selection**

Choose **Expand the selection** when you want the entire row to remain together.

---

# 2️⃣ ✂️ Text to Columns

**Text to Columns** is used to split data from one column into multiple columns.

### 📍 Path

**Data → Data Tools → Text to Columns**

### 📝 Example

Suppose column A contains:

| City-Pincode  |
| ------------- |
| Mumbai-400086 |
| Delhi-400001  |
| Pune-412701   |
| Thane-400059  |

We can separate **City** and **Pincode** into two columns.

### Before

| City-Pincode  |
| ------------- |
| Mumbai-400086 |
| Delhi-400001  |
| Pune-412701   |
| Thane-400059  |

### After

| City   | Pincode |
| ------ | ------- |
| Mumbai | 400086  |
| Delhi  | 400001  |
| Pune   | 412701  |
| Thane  | 400059  |

---

## 🔹 Steps to Use Text to Columns

1. Select the column containing the data.
2. Go to **Data**.
3. Click **Text to Columns**.
4. Select **Delimited** if the data is separated by a character.
5. Click **Next**.
6. Select the delimiter.

For example:

`Mumbai-400086`

The separator is:

`-`

So select **Other** and enter:

`-`

7. Click **Next**.
8. Select the destination if required.
9. Click **Finish**.

---

## 🔹 Common Delimiters

Text can be separated using:

* Comma `,`
* Space
* Tab
* Semicolon `;`
* Colon `:`
* Hyphen `-`
* Other custom characters

### Example

`Sanika-Shinde-Computer`

Using `-` as the delimiter gives:

| First  | Middle | Last     |
| ------ | ------ | -------- |
| Sanika | Shinde | Computer |

---

# 3️⃣ ⚡ Flash Fill

**Flash Fill** automatically detects a pattern from your example and fills the remaining cells.

It is useful for:

* Combining data
* Separating data
* Extracting names
* Changing text format
* Creating usernames
* Formatting data

### 📍 Path

**Data → Data Tools → Flash Fill**

### ⌨️ Shortcut

**Ctrl + E**

---

# 4️⃣ 👤 Flash Fill Example: First Name and Last Name

Suppose we have:

| First Name | Last Name |
| ---------- | --------- |
| Sanika     | Shinde    |
| Rahul      | Patil     |
| Priya      | Shah      |
| Amit       | Joshi     |

We want to combine First Name and Last Name.

### Step 1

In another column, manually type:

`Sanika Shinde`

### Step 2

Go to the next cell.

### Step 3

Press:

**Ctrl + E**

Excel detects the pattern and fills:

| First Name | Last Name | Full Name     |
| ---------- | --------- | ------------- |
| Sanika     | Shinde    | Sanika Shinde |
| Rahul      | Patil     | Rahul Patil   |
| Priya      | Shah      | Priya Shah    |
| Amit       | Joshi     | Amit Joshi    |

---

# 5️⃣ 🔤 Flash Fill for Separating Names

Suppose we have:

| Full Name     |
| ------------- |
| Sanika Shinde |
| Rahul Patil   |
| Priya Shah    |
| Amit Joshi    |

We want to extract the **First Name**.

In the next column, type:

`Sanika`

Then press:

**Ctrl + E**

Excel fills:

| Full Name     | First Name |
| ------------- | ---------- |
| Sanika Shinde | Sanika     |
| Rahul Patil   | Rahul      |
| Priya Shah    | Priya      |
| Amit Joshi    | Amit       |

The same method can be used to extract the **Last Name**.

---

# 6️⃣ 🧹 Flash Fill for Data Cleaning

Flash Fill can also help format data consistently.

### Example

Original:

| Name          |
| ------------- |
| sanika shinde |
| rahul patil   |
| priya shah    |

Type the desired format:

`Sanika Shinde`

Then press:

**Ctrl + E**

Excel detects the pattern and fills the remaining names.

---

# 7️⃣ 🔄 Remove Duplicates vs Text to Columns vs Flash Fill

| Tool                  | Purpose                                        |
| --------------------- | ---------------------------------------------- |
| 🗑️ Remove Duplicates | Removes repeated records                       |
| ✂️ Text to Columns    | Splits one column into multiple columns        |
| ⚡ Flash Fill          | Detects a pattern and automatically fills data |

---

# 8️⃣ 📌 Quick Example

Suppose we have:

| City-Pincode  |
| ------------- |
| Mumbai-400086 |
| Delhi-400001  |
| Mumbai-400086 |
| Pune-412701   |

### Remove Duplicates

Removes the repeated:

`Mumbai-400086`

### Text to Columns

Splits:

`Mumbai-400086`

into:

**Mumbai | 400086**

### Flash Fill

Can automatically create or extract information based on a pattern.

---
