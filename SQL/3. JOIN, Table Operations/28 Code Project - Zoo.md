# Zoo
You manage a zoo. Each animal in the zoo comes from a different country. Here are the tables you have:  

**Animals**

![x8hrzx2u](https://user-images.githubusercontent.com/94882786/165198311-5722d0bf-792f-4457-b54a-22804199c705.jpg)

**Countries**

![d74pjtd4](https://user-images.githubusercontent.com/94882786/165198319-f23c17b8-17c6-4e68-b4e6-fe4f50181ae2.jpg)

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
