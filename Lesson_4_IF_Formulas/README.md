# 🔀 IF Formulas

## 1. IF with AND

**Syntax:**

```excel
=IF(AND(condition1, condition2), "Pass", "Fail")
```

**Example:**

```excel
=IF(AND(C2>=35, B2>=35, E2>=35), "Pass", "Fail")
```

👉 **AND** means **all conditions must be TRUE**.

---

## 2. IF with OR

**Syntax:**

```excel
=IF(OR(condition1, condition2), "Result1", "Result2")
```

**Example:**

```excel
=IF(OR(C2<35, D2<35, E2<35), "Fail", "Pass")
```

👉 **OR** means **any one condition being TRUE** is enough.

