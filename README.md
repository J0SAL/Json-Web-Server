# Json-Web-Server

JSON Server

0. npm init
1. npm install json-server
2. (GET) : http://localhost:3000/reviews
         http://localhost:3000/reviews/1
3. Filtering: http://localhost:3000/products?category=electronics
              http://localhost:3000/products?category=electronics&dicount.type=shipping
4. Sorting: http://localhost:3000/products?_sort=price&order=desc
            http://http://localhost:3000/products?_sort=price,category&order=desc,asc
5. Pagenation: http://localhost:3000/products?_page=2&_limit=2 (limit default  = 10)
6. Operators : http://localhost:3000/products?price_gte=2000&price_lte=6000 (less than greater than equal to)
               http://localhost:3000/products?id_ne=1 (not equal to)
               http://localhost:3000/products?category_like=^f(start with 'f' ~ regex)
7. Full text search: http://localhost:3000/products?q=in (return data with in)
8. relationships: {child with parent} http://localhost:3000/reviews?_expand=product
                  {parent with child} http://localhost:3000/products?_embed=reviews 
9. (POST) http://http://localhost:3000/products
10. (PUT) http://http://localhost:3000/products/11 (send all data with the modified data)
11. (DELETE) http://http://localhost:3000/products/11



- credits : https://youtube.com/playlist?list=PLC3y8-rFHvwhc9YZIdqNL5sWeTCGxF4ya