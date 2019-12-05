# README #

### How do I set up? ###

* Create DB
* Set database configuration in .env
* Run localhost:3000/sync (script to create table with one user)

### NOTE: Fork this project and send me your github link ###

1) ### Create user endpoint ###

* Create user endpoint for add, update and delete user. (Changed should be reflected in the DB)
* Each endpoint must validate data type. (ex: validate email. If is not valid, return code error with error description).
* Implement jwt Auth. For login, the user should call to /login and use his name and email as credentials.
* Only users logged in should be able to edit their data.

2) ### Create a query to get sales by year and month from this table ###

| id  | provider_id | client_id  | price | created             |
| --- |:-----------:| ----------:| -----:| -------------------:|
|  1  | 3049        |   493      | $1600 | 2018-09-12 10:32:13 |
|  2  | 3495        |   540      | $1200 | 2018-09-16 11:32:27 |
|  3  | 5444        |   493      | $1000 | 2018-10-14 13:32:16 |
|  4  | 3049        |   493      | $1400 | 2018-10-12 10:32:13 |
|  5  | 3495        |   540      | $1650 | 2018-10-16 11:32:27 |
|  6  | 5444        |   124      | $1100 | 2019-01-14 13:32:16 |
|  7  | 3495        |   453      | $1900 | 2019-02-16 11:32:27 |
|  8  | 5444        |   123      | $900  | 2019-03-14 13:32:16 |


Ouput example:

| year | month | reservation | total |
| ---  |:-----:| -----------:| -----:|
| 2018 |  09   |   2         | $2800 |
| 2018 |  10   |   3         | $4050 |
| 2019 |  01   |   1         | $1100 |
| 2019 |  02   |   1         | $1900 |
| 2019 |  03   |   1         | $900  |


3) ### What are the differences between? ###

1 - Encontrar la secuencia más larga de números consecutivos en 2 arrays de entrada

Ejemplo: Input: [1, 2, 5, 3, 7, 8, 9] y [6, 8, 9, 3, 4, 5] Output: [3, 4, 5] o [7, 8, 9]

2 - Filtrar del array los elementos repetidos.

Ejemplo: Input: [1, 3, 2, 3, 4, 5, 6, h, s, c, h, 3, 6] output: [1, 3, 2, 4, 5 ,6, h, s, c]

4) ### Create layout ###

![alt text](https://dzwonsemrish7.cloudfront.net/items/3m34141R2v1W0v0L2j0c/test-layout-mobile.png?v=c2b9a871)
<br>
