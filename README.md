# eCommerceApp

eCommerceApp is a Flutter-based mobile application designed to provide a seamless shopping experience. It features product listing with pagination, category-based search and filters, cart management, and secure payments using Stripe. The app supports offline functionality using Hive and integrates push notifications with OneSignal. Firebase is used for authentication and storing user orders in Firestore.

## Features

- **Product List Fetching**: Displays a list of products with pagination.
- **State Management**: Managed using Riverpod for efficient state handling.
- **Offline Functionality**: Integrated Hive for storing data offline.
- **Search & Filter**: Includes search functionality with category-wise filtering.
- **Cart Management**: SQLite is used to manage products added to the cart.
- **Payment Integration**: Stripe is integrated for secure payments.
- **Push Notifications**: OneSignal is used for sending push notifications.
- **User Authentication**: Firebase Authentication is used for user login and sign-up.
- **Order Management**: Firebase Firestore is used for storing user orders.

## Screenshots

### ProductList
<img src="https://github.com/Priya129/eCommerceApp/blob/main/assets/Images/productlist.jpg" alt="Product List" height="300"/>)

### Product Detail
<img src="https://github.com/Priya129/eCommerceApp/blob/main/assets/Images/product_detail.jpg" alt="Product Detail" height="300"/>)

### CartPage
<img src="https://github.com/Priya129/eCommerceApp/blob/main/assets/Images/cartpage.jpg" alt="CartPage" height="300"/>)

### Profile
<img src="https://github.com/Priya129/eCommerceApp/blob/main/assets/Images/profile.jpg" alt="Profile" height="300"/>)

### Payment
<img src="https://github.com/Priya129/eCommerceApp/blob/main/assets/Images/payment.jpg" alt="Payment" height="300"/>)

### Notification
<img src="https://github.com/Priya129/eCommerceApp/blob/main/assets/Images/notification.jpg" alt="Notification" height="300"/>)

### OneSignal Platform
<img src="https://github.com/Priya129/eCommerceApp/blob/main/assets/Images/onesignal.png" alt="OneSignal Platform" height="300"/>)

### Stripe
<img src="https://github.com/Priya129/eCommerceApp/blob/main/assets/Images/stripe.png" alt="Stripe" height="300"/>)

### Firebase
<img src="https://github.com/Priya129/eCommerceApp/blob/main/assets/Images/firebase.png" alt="Firebase" height="300"/>)



## Demo Video

Watch a demo of the ToDo App here: [eCommerce Video](https://youtu.be/yEeQl5p0e_U?si=cmmF0fqYu5jGFEvO)

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/Priya129/eCommerceApp.git
cd eCommerceApp
```


### 2. Install Dependencies
Ensure you have Flutter installed. Then, install the necessary packages:

``` bash
Copy code
flutter pub get
```

### 3. Setup Firebase
- **Create a Firebase project and add your Android/iOS app.
= **Download google-services.json (for Android) or GoogleService-Info.plist (for iOS) and place them in the respective folders.
- **Enable Firebase Authentication, Firestore, and Firebase Storage.

### 4. Setup Hive
Hive is used for offline data storage. Run the Hive generator after making any changes to the data model:

```bash
Copy code
flutter pub run build_runner build
```

### 5. Stripe Setup
Follow the official Stripe documentation to get your API keys. Add your publishableKey in the Stripe configuration in the app.

### 6. OneSignal Setup
- **Create an account on OneSignal, configure your app, and get your app_id.
- **Initialize OneSignal in the app using the app_id.


### 7. Run the App

```bash
Copy code
flutter run
```

# Packages Used
dependencies:
  - flutter_riverpod: ^2.5.1
  - cached_network_image: ^3.4.1
  - hive: ^2.2.3
  - hive_flutter: ^1.1.0
  - dio: ^5.7.0
  - shimmer: ^3.0.0
  - shared_preferences: ^2.2.0
  - sqflite: ^2.3.3+1
  - path: ^1.8.2
  - flutter_stripe: ^4.0.1
  - http: ^0.15.0
  - firebase_auth: ^5.2.1
  - firebase_core: ^3.4.1
  - firebase_storage: ^12.3.0
  - image_picker: ^1.1.2
  - cloud_firestore: ^5.4.1
  - intl: ^0.18.0
  - onesignal_flutter: ^5.2.5

dev_dependencies:
  - hive_generator: ^1.0.0
  - build_runner: ^2.1.5
  - flutter_launcher_icons: ^0.13.1
