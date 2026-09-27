# Nested IF & IFS Formula in Excel

## 1. Nested IF Formula

### Primary Purpose

> **To check multiple conditions in one cell.**

### Syntax

```excel
=IF(condition1, value_if_true, IF(condition2, value_if_true, value_if_false))
```

### Example

Suppose the value is in **C4**:

```excel
=IF(C4>=10,20%,IF(C4>=5,10%,IF(C4>=0,0%)))
```

### Meaning

| Condition | Result |
| --------- | -----: |
| C4 ≥ 10   |    20% |
| C4 ≥ 5    |    10% |
| C4 ≥ 0    |     0% |

### Example

If:

```text
C4 = 12
```

Result:

```text
20%
```

If:

```text
C4 = 7
```

Result:

```text
10%
```

If:

```text
C4 = 3
```

Result:

```text
0%
```

---

# 2. IFS Formula

The **IFS** function is another way to check multiple conditions. It is easier to read than a long Nested IF formula.

### Syntax

```excel
=IFS(condition1,result1,condition2,result2,condition3,result3)
```

### Example

```excel
=IFS(C4>=10,20%,C4>=5,10%,C4>=0,0%)
```

### Meaning

| Condition | Result |
| --------- | -----: |
| C4 ≥ 10   |    20% |
| C4 ≥ 5    |    10% |
| C4 ≥ 0    |     0% |

---

# 3. Nested IF vs IFS

| Nested IF                     | IFS                               |
| ----------------------------- | --------------------------------- |
| Uses multiple IF functions    | Uses one IFS function             |
| Can become difficult to read  | Easier to read                    |
| Works in older Excel versions | Available in newer Excel versions |
| Example: `IF(...,IF(...))`    | Example: `IFS(...,...)`           |
