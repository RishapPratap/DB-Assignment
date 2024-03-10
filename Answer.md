## Question : Explain the relationship between the "Product" and "Product_Category"

**Answer:**
The relationship between Product table and Product_category is ONE-TO-MANY relationship
Each product belongs to one and only one product category,
while a product category can have multiple associated products.
This relationship is established through a foreign key in the "Product" table. 
The category_id column in the "Product" table acts as a foreign key referencing the id column of the "Product_Category" table.


## Question : How could you ensure that each product in the "Product" table has a valid category assigned to it?

**Answer:**

To ensure that each product in the "Product" table has a valid category assigned to it, we enforce referential integrity using a foreign key constraint.
This foreign key constraint ensures that every value entered into the category_id column of the "Product" table must exist in the id column of the "Product_Category" table.
If a product category is deleted or modified, the foreign key constraint ensures that any associated products are either updated or deleted accordingly, maintaining data integrity.
