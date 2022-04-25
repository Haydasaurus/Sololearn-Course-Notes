# Apartments
You want to rent an apartment and have the following table named **Apartments**:

![[gid7cbe6.bmp]]

Write a query to output the apartments whose prices **are greater than the average** and are also **not rented**, sorted by the 'Price' column.

>🛈 Recall the **AVG** keyword.

---

```sql
SELECT * 
FROM Apartments 
WHERE price > (SELECT AVG(price) FROM Apartments) 
AND status = 'Not rented' 
ORDER BY price;
```