# Apartments
You want to rent an apartment and have the following table named **Apartments**:

![gid7cbe6](https://user-images.githubusercontent.com/94882786/165194550-97e50426-b3a4-48ac-97a2-a5840baaa64a.jpg)

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
