# OrderNotifier
This project is designed to handle order management for e-commerce platforms, incorporating real-time push notifications using Firebase. It facilitates creating orders, updating order stages, and notifying users and shops about order statuses, including delivery updates.
#Project Structure
project-folder/
├── controllers/          # Handles business logic for orders
│   └── orderController.js
├── models/               # Database schemas (future expansion)
├── routes/               # API routes
│   └── orderRoutes.js
├── services/             # External service integrations
│   └── notificationService.js
├── utils/                # Helper functions for database operations
│   └── queryHelper.js
├── app.js                # Entry point of the application
├── .env                  # Environment variables (not committed)
└── package.json          # Project metadata and dependencies

#Features
  #1.Order Management
      Create a new order.
      Update order stages dynamically.
      Notify users and shops via Firebase Cloud Messaging (FCM).

  #2.Push Notifications
      Real-time updates to users and shops using Firebase Admin SDK.
      Notifications for events like order creation, stage updates, and delivery completion.

  #3.Environment Configuration
      Uses .env for sensitive configuration like Firebase credentials.

#Prerequisites
  1.Node.js: Ensure Node.js is installed on your system.
  2. MongoDB: Set up a MongoDB instance and configure its URI in the .env file.
  3.Firebase Project: Set up a Firebase project and download the service account key.

.env File
PORT=3000
FIREBASE_SERVICE_ACCOUNT_KEY={Your Firebase Service Account JSON String}
MONGO_URI=mongodb://localhost:27017/your_database

