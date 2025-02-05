## 🚀 **Summary**  
This PR implements the authentication flow using **Clerk** with **React Native (Expo)**.  
The authentication system includes **Sign-up, Sign-in, Reset Password, and Set Password flows**, utilizing **Clerk API** for authentication and **expo-secure-store** for secure token storage.  

---

## 🔥 **What’s Included?**  

### 📂 **`auth/` (Authentication Screens)**  
✅ `_layout.tsx` → Defines layout for authentication screens.  
✅ `sign-in.tsx` → Handles user sign-in using Clerk authentication.  
✅ `sign-up.tsx` → Manages user sign-up with Clerk authentication.  
✅ `reset-password.tsx` → Initiates password reset via email verification.  
✅ `set-password.tsx` → Allows users to set a new password after verification.  

### 📂 **`welcome/` (User Navigation Screens)**  
✅ `_layout.tsx` → Defines layout for welcome-related screens.  
✅ `index.tsx` → Handles redirection logic based on authentication status.  
✅ `Dashboard.tsx` → Main screen after successful login.  

---

## 🔑 **Token Management & Security**  
- Implemented **`expo-secure-store`** for securely storing Clerk authentication tokens.  
- `tokenCache` manages token retrieval and storage across app sessions.  

---

## 📄 **Environment Variables (.env.example)**  
This PR includes an **`.env.example`** file to specify required environment variables:  

```env
EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY=your-clerk-publishable-key
```

### **How to Use:**  
1. Create a **`.env`** file in the project root.  
2. Copy the values from `.env.example` and replace with your actual credentials.  
3. Restart the Expo development server after setting up the `.env` file.  

---

## ⚠️ **Notes **  
- **No backend is required for authentication**, as Clerk API handles it.  
- **Ensure the `.env` file is set up correctly** to prevent runtime errors.  
