# Cakes
A local bakery creates unique cake sets. Each cake set contains three different cakes.  
Here is the cakes table:

![duudeed0](https://user-images.githubusercontent.com/94882786/165150310-86be8238-7c21-46d9-bddc-abc4fd3d7d32.jpg)

Тoday a customer want a cake set that has minimal calories.  

Write a query to sort the cakes by calorie count and select the first 3 cakes from the list to offer the customer.

>🛈 Try to combine **ORDER BY** and **LIMIT** keywords.

---

```sql
SELECT * 
FROM cakes 
ORDER BY calories 
LIMIT 3;
```
