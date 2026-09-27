# 🧮 Essential Excel Formulas

## 📌 Overview

These are the essential Excel formulas I am learning and practicing as part of my **Data Analyst preparation**.

## 🎲 1. Random Number

### Formula

```excel
=RANDBETWEEN(1,100)
```

Generates a random whole number between **1 and 100**.

### Example

```text
=RANDBETWEEN(10,50)
```

Generates a random number between **10 and 50**.

---

## ➕ 2. SUM

### Formula

```excel
=SUM(A1:A10)
```

Adds all the numbers in the selected range.

### Example

If `A1:A5` contains:

```text
10
20
30
40
50
```

Formula:

```excel
=SUM(A1:A5)
```

Result:

```text
150
```

---

## 🔽 3. MIN

### Formula

```excel
=MIN(A1:A10)
```

Returns the **smallest value** from the selected range.

### Example

```text
10
25
5
40
15
```

Formula:

```excel
=MIN(A1:A5)
```

Result:

```text
5
```

---

## 🔼 4. MAX

### Formula

```excel
=MAX(A1:A10)
```

Returns the **largest value** from the selected range.

### Example

```text
10
25
5
40
15
```

Formula:

```excel
=MAX(A1:A5)
```

Result:

```text
40
```

---

## 📊 5. AVERAGE

### Formula

```excel
=AVERAGE(A1:A10)
```

Calculates the **average (mean)** of the numbers in the selected range.

### Example

```text
10
20
30
40
50
```

Formula:

```excel
=AVERAGE(A1:A5)
```

Result:

```text
30
```

---

## 📈 6. Percentage

### Formula

```excel
=(Part/Total)*100
```

Used to calculate the percentage of a value compared with the total.

### Example

If:

```text
Part = 25
Total = 100
```

Formula:

```excel
=(25/100)*100
```

Result:

```text
25%
```
