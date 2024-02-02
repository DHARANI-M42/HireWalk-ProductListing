Admin Credentials:

- Email: admin@yopmail.com
- Password: TestUser@123

Customer Credentials:

- Email: customer@yopmail.com
- Password: TestUser@123

To register, users can utilize the default Laravel registration form. Upon registration, they will be added as customers automatically. Use the provided admin credentials to access admin functionalities.

Task Overview:

1. Utilized Laravel's default registration and login functionality.
2. Employed auth middleware to restrict customers from accessing admin menus.
3. Admins can perform CRUD operations on products, while customers can only view available active products.
4. Implemented category seeding with 10 predefined categories using the seeder method. To seed these categories, use the command: "php artisan db:seed --class=CategorySeeder".
5. For product management, administrators can add, edit, and delete products. They can also manage tags and suppliers associated with each product.
6. During creation and editing of products, proper JavaScript validation is added to ensure data integrity and accuracy.
7. Administrators can enter product price and profit price, with the total price of the product calculated automatically.

Database Setup:
- Ensure a database named "product_listings" exists in your MySQL or compatible DBMS.
- Update the `.env` file with the correct database name if using a different one.
Migration:
- Run migration to create necessary tables:
  ```
  php artisan migrate
  ```
Seed Categories:
 php artisan db:seed --class=CategorySeeder
