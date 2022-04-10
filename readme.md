http://localhost:4000/products?_sort=price&_order=desc -For Sorting
http://localhost:4000/products?_sort=price,category&_order=desc,asc -For desc price and category=asc
http://localhost:4000/products -For getting all the products
http://localhost:4000/products/1 -For getting Specific Products
http://localhost:4000/products?category=electronics - For Filtering according to category
http://localhost:4000/products?category=electronics&discount.type=shipping -For Filtering Category and discount
http://localhost:4000/products?_page=1&_limit=5 -For Pagination 
http://localhost:4000/products?price_gte=2000&price_lte=6000 -For getting the products greater than 2000 and less than 6000 price.
http://localhost:4000/products?id_ne=1 -Getting all the products except 1.
http://localhost:4000/products?category_like=^f -For getting the category starting with f.
http://localhost:4000/products?q=in -Full Text Search
http://localhost:4000/products?_embed=reviews -Relationship between Products and Child Reviews.
http://localhost:4000/products/1?_embed=reviews -For getting Specific Product Related Reviews.
http://localhost:4000/reviews?_expand=product -RelationShip Between Reviews and Child Product
For Post Request 
       {
        "id": 11,
        "title": "Product 9",
        "category": "accessories",
        "price": 4000,
        "description": "This is description about product 9"
} -Pass The data as a body in http://localhost:4000/products
For Put Request 
       {
        "id": 11,
        "title": "Product 11",
        "category": "accessories",
        "price": 4000,
        "description": "This is description about product 11"
} -Pass The data as a body in http://localhost:4000/products/11
For Patch Request 
       {
        "price": 8000,
}
http://localhost:4000/products/12 -For delete Request
For SignUp:-]
{
  "email": "test@mail.com",
  "password": "best123"
}-Pass the data as a body in http://localhost:4000/signup
For SignIn:-
{
  "email": "test@mail.com",
  "password": "best123"
}-Pass the data as a body in http://localhost:4000/ signin