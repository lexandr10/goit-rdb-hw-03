# goit-rdb-hw-03
![task 1 2](https://github.com/lexandr10/goit-rdb-hw-03/assets/133785276/28748730-af3b-4e5f-ba6b-1f368641942f)
![task 1 1](https://github.com/lexandr10/goit-rdb-hw-03/assets/133785276/4e867399-83bc-41dc-bce4-7f5aea88a2d2)
CODE: 
Select * from mydb.products;
Select name, phone from mydb.shippers;
![task 2](https://github.com/lexandr10/goit-rdb-hw-03/assets/133785276/7119e2b5-51e1-4e18-8182-d4078648427c)
CODE: 
Select  AVG(price) as middle_price, max(price) as max_price, min(price) as min_price
from mydb.products;
![task 3](https://github.com/lexandr10/goit-rdb-hw-03/assets/133785276/df39d7a8-9639-4c4c-9f65-a1e02f6c2f37)
CODE: 
Select distinct category_id, price
from mydb.products
ORDER BY  price DESC, category_id
LIMIT 10;
![task 4](https://github.com/lexandr10/goit-rdb-hw-03/assets/133785276/36054666-122d-47ad-a499-e08b212441eb)
CODE:
Select count(id) as count_products
from mydb.products
where price > 20 or price > 100;
![task 5](https://github.com/lexandr10/goit-rdb-hw-03/assets/133785276/32d13757-fecf-410b-869d-0475f985a337)
CODE: 
Select supplier_id, count(*) as count_products, AVG(price) as middle_price
from mydb.products
group by supplier_id;
