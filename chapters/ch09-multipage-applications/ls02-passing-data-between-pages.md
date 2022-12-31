---
id: ls02-passing-data-between-pages
title: Passing Data Between Pages
---

Before we learn more advance techniques like state management, in this chapter we will practice how we can pass data from one widget to another.

## Projects

### 1. Authenticate

Build a Flutter App with two page, one for login and one for home. Login page should have a form with two text fields, one for email and one for password. When the user clicks on the login button, the app should navigate to the home page and display the email and password in a text widget.

> Do this twice, once with passing data using the constructor and `Navigator.push` and once with passing data using the `Navigator.pushNamed` method and extracting arguments using `ModalRoute`.

### 2. Shopping Cart

Build a Flutter where the home page displays a list of products with name, image, price and add to cart Icon button. Once the add to cart is clicked, it should add the product to the cart (a list of products maintained using stateful widget). Display floating action button with cart icon and tapping that should navigate to the cart page. The cart page should display the list of products added to the cart as well as the sum total of the price of all the products at the bottom.

## Resources

- [Passing Data Between Pages](https://flutter.dev/docs/cookbook/navigation/passing-data)
- [Passing Data](https://flutter.dev/docs/cookbook/navigation/navigate-with-arguments)
- [ModalRoute](https://api.flutter.dev/flutter/widgets/ModalRoute-class.html)
