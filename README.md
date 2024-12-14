# rental-website

# QuickRent - Rent Gadgets Hassle-Free

QuickRent is an application designed to allow users to rent gadgets like laptops, cameras, and gaming consoles at affordable rates. The app provides a platform to explore gadgets, place rental orders, and manage rental details seamlessly.

---

## Features

- **Browse Gadgets**: Users can view a wide selection of gadgets available for rent.
- **Rent Gadgets**: Users can rent gadgets for a specified duration at competitive prices.
- **Quick Delivery**: Fast and reliable delivery of gadgets right to your doorstep.
- **Payment Integration**: Secure payment processing through Stripe (or PayPal).
- **Responsive UI**: Fully responsive design to cater to both mobile and desktop users.

---

## Technologies Used

- **Front-End**:
  - Flutter (for mobile app development)
  - Dart
  - HTTP package for API communication

- **Back-End**:
  - Node.js (Server)
  - Express.js (Framework)
  - MongoDB (Database)
  - Stripe or PayPal (Payment Integration)

---

## Getting Started

### Prerequisites

Before you start, you’ll need to have the following installed:

1. **Flutter SDK**: [Flutter Installation](https://flutter.dev/docs/get-started/install)
2. **Node.js**: [Node.js Download](https://nodejs.org/)
3. **MongoDB**: Either [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) for cloud hosting or [local MongoDB installation](https://www.mongodb.com/docs/manual/installation/).

---

### Back-End Setup (Node.js + MongoDB)

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/quickrent.git
    cd quickrent
    ```

2. Navigate to the `backend` directory:

    ```bash
    cd backend
    ```

3. Install dependencies:

    ```bash
    npm install
    ```

4. Set up MongoDB:
   - If you're using **MongoDB Atlas**, replace the MongoDB URI in `server.js` with your Atlas connection string.
   - If you're using **local MongoDB**, ensure it's running and accessible at `mongodb://localhost:27017`.

5. Start the Node.js server:

    ```bash
    node server.js
    ```

The server will now be running on `http://localhost:5000`.

---

### Front-End Setup (Flutter)

1. Navigate to the `frontend` directory:

    ```bash
    cd frontend
    ```

2. Install dependencies:

    ```bash
    flutter pub get
    ```

3. Update the API base URL in `lib/services/gadget_service.dart` to match your back-end URL (e.g., `http://localhost:5000/gadgets`).

4. Run the app on your device or emulator:

    ```bash
    flutter run
    ```

Your Flutter app will now run on your device, and you can interact with the backend API.

---

## Deployment

### Deploying the Back-End (Node.js)

You can deploy the back-end to cloud platforms like **Heroku**, **AWS**, or **DigitalOcean**. Here's an example of how to deploy to Heroku:

1. Initialize a git repository in the backend folder:

    ```bash
    git init
    ```

2. Create a Heroku app:

    ```bash
    heroku create
    ```

3. Deploy the app:

    ```bash
    git push heroku master
    ```

4. Set up MongoDB (if not using MongoDB Atlas).

---

## Payment Integration

### Stripe (or PayPal) Integration

To integrate payment processing:

1. Sign up for **Stripe** or **PayPal** and get the API keys.
2. Implement the payment API in your app following the respective SDK documentation:
   - [Stripe Flutter SDK](https://stripe.com/docs/payments/accept-a-payment?platform=flutter)
   - [PayPal REST API](https://developer.paypal.com/docs/api/overview/)

---

## Testing

### Back-End Testing

You can test the back-end API using tools like **Postman** to verify that the endpoints are working correctly.

### Front-End Testing

For Flutter, you can use the built-in testing framework to write unit and widget tests.

---

## Contributing

We welcome contributions! If you'd like to help improve the project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to your branch (`git push origin feature-branch`).
5. Create a new Pull Request.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- [Flutter](https://flutter.dev/) for the front-end development.
- [Node.js](https://nodejs.org/en/) for the back-end development.
- [MongoDB](https://www.mongodb.com/) for database management.
- [Stripe](https://stripe.com/) for payment processing.

