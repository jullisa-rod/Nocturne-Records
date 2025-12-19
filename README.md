# Nocturne Records
## API Project
### 🎧ྀི♪⋆.✮ Project Description
Vintage Vinyl's is a specialized music store API designed for vinyl enthusiasts and equipment collectors. As a backend developer, I took an existing Version 1 application and transformed it into a reliable, feature-rich platform. My work focused on stabilizing the product catalog, securing administrative routes, and building out the shopping cart and checkout experience.


Security: JWT (JSON Web Tokens) for authenticated sessions and role-based access.
### Bug Fixes
🐞 Catalog Stabilization
Search Accuracy: Resolved issues where the record search returned incorrect results. Now, customers can filter by category, price range, and subcategories.
The "Duplicate Product" Fix: Fixed a critical bug in the updateProduct method. Previously, editing a record's details created a duplicate entry; it now correctly updates the existing record using the product_id.

### API Reference
Method	Endpoint	Description	Access
GET	/products	Browse the vinyl collection	Public
PUT	/products/{id}	Update record details	Admin Only
GET	/categories	List all music genres	Public
POST	/cart/products/{id}	Add a record to your cart	User Only
POST	/orders	Complete purchase/checkout	User Only
