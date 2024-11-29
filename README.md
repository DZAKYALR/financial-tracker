

---

# Financial Tracker

**A modern, serverless app for managing loans, tracking expenses, and organizing income—all in one place.**

![Version](https://img.shields.io/github/v/release/DZAKYALR/financial-tracker)
![License](https://img.shields.io/github/license/DZAKYALR/financial-tracker)
![Stars](https://img.shields.io/github/stars/DZAKYALR/financial-tracker)
![Contributors](https://img.shields.io/github/contributors/DZAKYALR/financial-tracker)

## Features
- **Loan Management**: Keep track of your loans, including amounts, due dates, purposes, and percentages allocated to others.
- **Expense Tracking**: Organize and categorize your spending to stay on top of your budget.
- **Income Management**: Record and manage all income sources for better financial insights.
- **User-Specific Data**: Your data is securely stored locally on your machine or in the cloud using a unique user ID.

### **Tech Stack**
- **Frontend**:  
  - [React](https://reactjs.org/) with [TypeScript](https://www.typescriptlang.org/).  

- **Backend**:  
  - [Cloudflare Workers](https://developers.cloudflare.com/workers/) for serverless function execution.  

- **Storage**:  
  - **Local**: [IndexedDB](https://developer.mozilla.org/en-US/docs/Web/API/IndexedDB_API) or [LocalForage](https://localforage.github.io/localForage/).  
  - **Cloud**: [Firebase Realtime Database](https://firebase.google.com/products/realtime-database) for real-time data synchronization with a free tier.  

- **Styling**:  
  - [Tailwind CSS](https://tailwindcss.com/) for efficient and customizable UI design.  

- **Hosting**:  
  - [Cloudflare Pages](https://pages.cloudflare.com/) for fast, scalable, and reliable hosting of the app.  

---

## Installation
### Prerequisites
- Node.js (v16+)
- npm or yarn

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/DZAKYALR/financial-tracker.git
   ```
2. Install dependencies:
   ```bash
   cd financial-tracker
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```
---

## Data Storage Strategy
### Serverless Storage Options
1. **Local Storage**:  
   - Use **IndexedDB** for offline-first capabilities to ensure the app works seamlessly without internet access.  
   - Simplify IndexedDB usage with [LocalForage](https://localforage.github.io/localForage/).  

2. **Cloud Storage**:  
   - Use **Firebase Realtime Database** for secure, real-time synchronization of user-specific data.  
   - Leverage `userId` as the key to segregate and organize data for each user.  

3. **Hybrid Solution**:  
   - Sync local data stored in IndexedDB with **Firebase Realtime Database** periodically.  
   - This ensures offline-first capabilities while keeping cloud data updated for multi-device access.  

---

## Contributing
We welcome contributions! Please check out the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```
