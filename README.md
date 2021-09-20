# flutter_firebase

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

### About the project 
This is a grocery system application. 
It has two kinds of users: buyer and seller 

SignUp and Login: 
    1. Shows error message when input wrong credentials
    2. Uses firebase authentication

Features for buyer: 
    1. Add to cart
    2. Set quantity of products
    3. View Cart
    4. Delete product from cart

Features for seller:
    1. Add products to database
    2. Remove products from database
    3. Edit products (ex. product name, price, weight)

All products and actions are connected to firebase realtime database:
    1. When user deletes product, data at the firebase will also be deleted according to the database. Cart for products in cart and products for products in the shop. 

    2. When seller edits a product, data at database will also be changed. 

Firebase Realtime Database: 
    1. Different users will have different products in their cart depending on their userId. 

    2. For example, buyer login as user1 and add orange and mango to their cart. Then user1 logout and login as user2. User2 can add new products in the cart and it will only show user2's cart and not user1. 

    3. This is filtered by userId of each user. 
