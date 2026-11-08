# Cafeteria Mobile App

A cross-platform mobile app for ordering food from a university cafeteria, built with **React Native (Expo)** and **Firebase**. Students browse the menu and place orders. Caterers manage menu items and incoming orders from a separate admin interface.

## Features

### Customers
- Sign up and log in
- Browse food by category and search the menu
- View item details and place orders with a quantity and delivery address
- Track orders on the **My Orders** screen
- Receive **push notifications** about order updates

### Caterers (admin)
- Separate admin navigation (drawer and bottom tab bar)
- Add and manage food items
- View incoming orders in real time and update their status

## Tech stack

| Area | Tools |
|------|-------|
| Mobile | React Native, Expo |
| Navigation | React Navigation (stack, drawer, bottom tabs) |
| UI | React Native Paper, NativeBase, vector icons |
| Backend | Firebase Authentication, Cloud Firestore (real-time listeners) |
| Notifications | Expo Notifications |
| Monitoring | Firebase Crashlytics, Firebase Performance |

## Project structure

```text
├── App.js
├── Screens/       # StartPage, Login, SignUp, Home, FoodCategoryList, ItemDes,
│                  # Search, MyOrders, Notifications, AdminHome, AddItems, AdminOrders
├── Components/    # Navigation stacks, drawers, headers
├── Firebase/      # Firebase configuration
├── Globals/       # Shared values
└── firestore.rules
```

**Firestore collections:** `clients`, `caterers`, `foods`, `orders`, `notifications`

## Getting started

**Prerequisites:** Node.js 16+, Expo CLI, a Firebase project, and the Expo Go app or an Android/iOS emulator.

```bash
git clone https://github.com/SamithaPrabath/cafeteria-mobile-app.git
cd cafeteria-mobile-app
npm install
```

1. Create a Firebase project and enable **Authentication** and **Cloud Firestore**.
2. Add your Firebase config to `Firebase/` and your Android `google-services.json` to the project root.
3. Start the app:

   ```bash
   npm start          # then scan the QR code with Expo Go
   npm run android    # or run on an Android emulator
   ```

## Contributors

Built as a team project by:

- **Samitha Prabath**: [GitHub](https://github.com/SamithaPrabath)
- **Venura Warnasooriya**
