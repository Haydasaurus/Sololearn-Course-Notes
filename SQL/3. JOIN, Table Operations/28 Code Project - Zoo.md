# Zoo
You manage a zoo. Each animal in the zoo comes from a different country. Here are the tables you have:  

**Animals**

![[x8hrzx2u.bmp]]

**Countries**

![[d74pjtd4.bmp]]

1) A new animal has come in, with the following details:  
name - "Slim", type - "Giraffe", country_id - 1  
Add him to the Animals table.  

2) You want to make a complete list of the animals for the zoo’s visitors. Write a query to output a new table with each animal's name, type and country fields, sorted by countries.

>🛈 Recall **INSERT** and **INNER JOIN** keywords.

---

```sql
/* name - "Slim", type - "Giraffe", country_id - 1 */

INSERT INTO Animals
VALUES ('Slim', 'Giraffe', '1');

SELECT Animals.name, Animals.type, Countries.country
FROM Animals INNER JOIN Countries
ON Animals.country_id = Countries.id
ORDER BY country;
```