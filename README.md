
# QuikMart - Project Structure

## 📂 Project Creation Steps

1. **Install Node.js**  
   Install Node.js from [here](https://nodejs.org/).

2. **Install Android Studio & SDK**  
   Download and install Android Studio along with its SDKs.

3. **Initialize React Native Project**  
   Run the following command to create a new React Native project:  
   ```
   npx react-native init <ProjectName>
   ```
   If you're facing issues with `react-native-cli`, you can uninstall it globally:  
   ```
   npm uninstall -g react-native-cli
   ```
   Then, run:  
   ```
   npx @react-native-community/cli init <ProjectName>
   ```

4. **Folder Structure**  
   Once the project is created, navigate to the project folder and organize it as follows:
   
   ```
   QuikMart
   ├── android/               # Android-specific files
   ├── ios/                   # iOS-specific files
   ├── src/                   # All app-related code
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
   │   ├── App.tsx            # Root component (move App.tsx to src folder)
   ├── .gitignore             # Git ignore file
   ├── package.json           # Dependencies & scripts
   ├── tsconfig.json          # TypeScript config (if using TypeScript)
   ├── babel.config.js        # Babel config
   ├── metro.config.js        # Metro bundler config
   ├── README.md              # Project documentation
   ```

---

## 📂 Detailed Explanation

1️⃣ **src/assets/** (Static Files)  
   - **images/**: Store images such as logos, banners, etc.  
   - **fonts/**: Store custom fonts.  
   - **icons/**: Store icon files.

   Example:
   ```
   src/assets/
   ├── images/
   │   ├── logo.png
   │   ├── banner.jpg
   ├── fonts/
   │   ├── Roboto-Regular.ttf
   ├── icons/
   │   ├── cart.png
   ```

2️⃣ **src/components/** (Reusable UI Components)  
   Reusable components like buttons, input fields, product cards, etc.

   Example:
   ```
   src/components/
   ├── CustomButton.tsx
   ├── InputField.tsx
   ├── ProductCard.tsx
   ```

3️⃣ **src/screens/** (Screens for Navigation)  
   Screens for different sections of the app like Home, Cart, etc.

   Example:
   ```
   src/screens/
   ├── HomeScreen/
   │   ├── index.tsx
   │   ├── styles.ts
   ├── CartScreen/
   │   ├── index.tsx
   │   ├── styles.ts
   ```

4️⃣ **src/navigation/** (Navigation Logic)  
   Navigation setup (React Navigation) for app routing.

   Example:
   ```
   src/navigation/
   ├── AppNavigator.tsx    # Main navigator
   ├── AuthNavigator.tsx   # Authentication flows
   ├── TabNavigator.tsx    # Bottom tab navigation
   ```

5️⃣ **src/redux/** (Redux State Management)  
   Redux-related files if using Redux or Redux Toolkit for state management.

   Example:
   ```
   src/redux/
   ├── store.ts
   ├── slices/
   │   ├── authSlice.ts
   │   ├── cartSlice.ts
   │   ├── productSlice.ts
   ```

6️⃣ **src/hooks/** (Custom Hooks)  
   Custom React hooks to encapsulate logic.

7️⃣ **src/utils/** (Helper Functions)  
   Utility functions like formatters, constants, etc.

8️⃣ **src/services/** (API Calls & Async Storage)  
   Functions to handle API calls and manage async storage.

9️⃣ **src/context/** (Context API)  
   If using React Context API for state management.

🔟 **src/config/** (App Configurations)  
   Store configurations such as themes, API keys, and constants.

   Example:
   ```
   src/config/
   ├── theme.ts
   ├── constants.ts
   ├── env.ts
   ```

---

