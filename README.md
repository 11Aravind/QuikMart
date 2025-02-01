Project creation steps
1. install node
2. install android studio and install its sdk's
3. npx react-native init <Project name> then npx react-native init <Project name> OR npm uninstall -g react-native-cli
and  npx @react-native-community/cli init <Project name>
4. goto project folder and then create folder structue like following
QuikMart
│── android/               # Android-specific files
│── ios/                   # iOS-specific files
│── src/                   # All app-related code
│   ├── assets/            # Images, fonts, icons, etc.
│   ├── components/        # Reusable UI components
│   ├── screens/           # All screen components
│   ├── navigation/        # App navigation (React Navigation)
│   ├── redux/             # Redux store, slices, actions (if using Redux)
│   ├── hooks/             # Custom hooks
│   ├── utils/             # Helper functions, constants
│   ├── services/          # API calls, async storage
│   ├── context/           # React Context API (if used)
│   ├── config/            # Configurations (API keys, themes)
│   ├── styles/            # Global styles (if using Styled Components)
│   ├── App.tsx            # Root component[move app.tsx to src folder]
│── .gitignore             # Git ignore file
│── package.json           # Dependencies & scripts
│── tsconfig.json          # TypeScript config (if using TypeScript)
│── babel.config.js        # Babel config
│── metro.config.js        # Metro bundler config
│── README.md              # Project documentation



📂 Detailed Explanation

1️⃣ src/assets/ (Static Files)

src/assets/
├── images/
│   ├── logo.png
│   ├── banner.jpg
├── fonts/
│   ├── Roboto-Regular.ttf
├── icons/
│   ├── cart.png


2️⃣ src/components/ (Reusable UI Components)


src/components/
├── CustomButton.tsx
├── InputField.tsx
├── ProductCard.tsx

3️⃣ src/screens/ (Screens for Navigation)

src/screens/
├── HomeScreen/
│   ├── index.tsx
│   ├── styles.ts
├── CartScreen/
│   ├── index.tsx
│   ├── styles.ts


4️⃣ src/navigation/ (Navigation Logic)

src/navigation/
├── AppNavigator.tsx    # Main navigator
├── AuthNavigator.tsx   # Authentication flows
├── TabNavigator.tsx    # Bottom tab navigation

5️⃣ src/redux/ (Redux State Management) if we use redux/redux toolkit

src/redux/
├── store.ts
├── slices/
│   ├── authSlice.ts
│   ├── cartSlice.ts
│   ├── productSlice.ts

6️⃣ src/hooks/ (Custom Hooks)

7️⃣ src/utils/ (Helper Functions)

8️⃣ src/services/ (API Calls & Async Storage)

9️⃣ src/context/(am not using context if use then create it)

🔟 src/config/ (App Configurations)

src/config/
├── theme.ts
├── constants.ts
├── env.ts


