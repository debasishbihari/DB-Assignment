1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.
   
Ans 1: The relationship between the "Product" and "Product_Category" entities in the diagram can be described as a one-to-many relationship. A product category can have many products. This is reflected by the foreign key category_id in the product table. This foreign key references the primary key (id) of the product_category table. A product can belong to only one category. This is enforced by the foreign key constraint in the database. In simpler terms, a product category can group many products under it, but a product can only be classified under a single category based on the tables you described.

2. How could you ensure that each product in the "Product" table has a valid category assigned to it?

Ans 2: There is a way too ensure that each product in the "Product" table has a valid category assigned to it Foreign Key Constraint: This is the most common approach. The category_id in the product table is already defined as a FOREIGN KEY referencing the primary key (id) of the product_category table. This enforces a database-level rule that any value assigned to category_id must exist in the product_category table. When attempting to insert a product with a non-existent category ID, the database will throw an error preventing invalid data entry. 
