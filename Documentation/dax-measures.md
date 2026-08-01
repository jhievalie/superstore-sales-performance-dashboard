# DAX Measures

## Total Sales

```DAX
Total Sales =
SUM(Orders[Sales])
```

---

## Total Orders

```DAX
Total Orders =
DISTINCTCOUNT(Orders[Order ID])
```

---

## Average Order Value

```DAX
Average Order Value =
DIVIDE([Total Sales],[Total Orders])
```

---

## Average Sales per Day

```DAX
Average Sales per Day =
DIVIDE(
    [Total Sales],
    DISTINCTCOUNT(Calendar[Date])
)
```