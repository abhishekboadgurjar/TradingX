<div align="center">
  
  <h1>📈 TradingX - Full-Stack Web and App Trading Platform</h1>
  <p><strong>A comprehensive multi-platform stock trading application with real-time market data, advanced security, and seamless user experience</strong></p>
  
  ![Status](https://img.shields.io/badge/status-active-success.svg)
  ![License](https://img.shields.io/badge/license-MIT-blue.svg)
  ![Node](https://img.shields.io/badge/node-%3E%3D18.0.0-brightgreen.svg)
  ![React](https://img.shields.io/badge/react-19.1.0-blue.svg)
</div>

---

## 🎯 Project Vision & Aim

**TradingX** is designed to democratize stock trading by providing a professional-grade, yet accessible trading platform that combines the power of real-time market data with an intuitive user interface. Our mission is to:

- **Empower Individual Investors**: Provide retail traders with institutional-grade tools and real-time market insights
- **Ensure Security First**: Implement multi-layered authentication including biometric, PIN, and OAuth to protect user assets
- **Enable Cross-Platform Trading**: Seamless experience across web and mobile devices with synchronized data
- **Promote Financial Literacy**: Offer transparent portfolio tracking and comprehensive order history
- **Deliver Real-Time Performance**: WebSocket-based live updates ensuring traders never miss market movements

### 🌟 What Makes TradeX Unique?

1. **Multi-Factor Authentication System**: Combines traditional password, 4-digit PIN, biometric authentication (RSA), and OAuth for maximum security
2. **Real-Time Market Simulation**: Automated price updates every 5 seconds with realistic market behavior during trading hours (9:30 AM - 3:30 PM)
3. **Intelligent Account Protection**: Automatic account lockout after 3 failed attempts with 30-minute cooldown period
4. **Cross-Platform Synchronization**: Real-time data sync between web and mobile apps using WebSocket technology
5. **Production-Ready Architecture**: Scalable microservices design with comprehensive error handling and API documentation

---

## 🚀 Key Features

### 🔐 Advanced Security & Authentication
- ✅ **JWT-based Authentication** with access and refresh token mechanism
- ✅ **Email OTP Verification** for account registration and sensitive operations
- ✅ **Biometric Authentication** using RSA encryption for mobile devices
- ✅ **4-Digit PIN System** for quick and secure app access
- ✅ **OAuth Integration** (Google, Apple) for social login
- ✅ **Account Lockout Protection** after failed login attempts
- ✅ **Password & PIN Reset** with email verification
- ✅ **Secure Token Refresh** mechanism for persistent sessions

### 📊 Real-Time Trading Features
- ✅ **Live Stock Price Updates** via WebSocket (5-second intervals)
- ✅ **Interactive Price Charts** with 1-minute and 10-minute candlestick data
- ✅ **Buy/Sell Operations** with instant order execution
- ✅ **Portfolio Management** with real-time profit/loss tracking
- ✅ **Order History** with complete transaction details
- ✅ **Balance Management** with ₹50,000 initial virtual balance
- ✅ **Trading Hours Validation** (9:30 AM - 3:30 PM, weekdays only)
- ✅ **Market Holiday Support** with configurable holiday calendar

### 💼 Portfolio & Holdings
- ✅ **Real-Time Holdings View** with current market value
- ✅ **Profit/Loss Calculation** with percentage changes
- ✅ **Average Buy Price Tracking** for each stock
- ✅ **Quantity Management** with partial sell support
- ✅ **Portfolio Diversification** insights
- ✅ **Transaction History** with timestamps and prices

### 📱 User Experience
- ✅ **Responsive Web Design** optimized for all screen sizes
- ✅ **Native Mobile App** for iOS and Android
- ✅ **Dark/Light Mode** support (configurable)
- ✅ **Smooth Animations** and transitions
- ✅ **Intuitive Navigation** with bottom tabs (mobile) and sidebar (web)
- ✅ **Real-Time Notifications** for order confirmations
- ✅ **Offline Support** with data caching (mobile)

### 🛠 Developer Features
- ✅ **RESTful API** with comprehensive endpoints
- ✅ **Swagger Documentation** for easy API testing
- ✅ **WebSocket Events** for real-time subscriptions
- ✅ **Error Handling** with descriptive error messages
- ✅ **Input Validation** on both client and server
- ✅ **CORS Configuration** for secure cross-origin requests
- ✅ **Environment-based Configuration** for different deployment stages

---

## 🏗 System Architecture

```
TradeX/
├── server/                 # Backend API & WebSocket Server
│   ├── controllers/        # Business logic handlers
│   ├── models/            # MongoDB schemas (User, Stock, Order, Holding)
│   ├── routes/            # API route definitions
│   ├── middleware/        # Auth, error handling, validation
│   ├── services/          # Cron jobs, email service
│   └── docs/              # Swagger API documentation
│
├── client-web/            # Next.js Web Application
│   ├── src/
│   │   ├── app/           # Next.js 15 app router pages
│   │   ├── components/    # Reusable React components
│   │   ├── store/         # Zustand state management
│   │   └── lib/           # Utility functions & API clients
│   └── public/            # Static assets
│
└── client-app/            # React Native Mobile App
    ├── screens/           # Mobile app screens
    ├── navigation/        # React Navigation setup
    ├── store/             # Zustand state management
    ├── components/        # Reusable mobile components
    └── lib/               # Utility functions & API clients
```

---

## 🛠 Technology Stack

### 🌐 Frontend (Web)
| Technology | Version | Purpose |
|------------|---------|---------|
| **Next.js** | 15.5.4 | React framework with SSR and app router |
| **React** | 19.1.0 | UI library for building interfaces |
| **TypeScript** | 5.x | Type-safe JavaScript |
| **Tailwind CSS** | 4.x | Utility-first CSS framework |
| **Zustand** | 5.0.8 | Lightweight state management |
| **Lightweight Charts** | 5.0.9 | Professional financial charts |
| **Socket.IO Client** | 4.8.1 | Real-time WebSocket communication |
| **Axios** | 1.12.2 | HTTP client for API requests |
| **Lucide React** | 0.544.0 | Beautiful icon library |
| **Radix UI** | Latest | Accessible UI components |

### 📱 Mobile (React Native)
| Technology | Version | Purpose |
|------------|---------|---------|
| **React Native** | 0.81.4 | Cross-platform mobile framework |
| **Expo** | 54.0.13 | Development and build toolchain |
| **React Navigation** | 7.x | Navigation library for mobile |
| **Zustand** | 5.0.8 | State management |
| **React Native Paper** | 5.14.5 | Material Design components |
| **Socket.IO Client** | 4.8.1 | Real-time communication |
| **AsyncStorage** | 2.2.0 | Persistent local storage |
| **Expo Secure Store** | 15.0.7 | Encrypted storage for tokens |
| **React Native Reanimated** | 4.1.1 | Smooth animations |
| **Lucide React Native** | 0.545.0 | Icon library |

### ⚙️ Backend (Server)
| Technology | Version | Purpose |
|------------|---------|---------|
| **Node.js** | 18+ | JavaScript runtime |
| **Express.js** | 4.19.2 | Web application framework |
| **MongoDB** | 8.18.2 | NoSQL database |
| **Mongoose** | 8.18.2 | MongoDB ODM |
| **Socket.IO** | 4.7.5 | WebSocket server |
| **JWT** | 9.0.2 | Token-based authentication |
| **bcryptjs** | 3.0.2 | Password hashing |
| **node-cron** | 4.2.1 | Scheduled tasks |
| **Nodemailer** | 6.9.8 | Email service |
| **Swagger UI** | 5.0.0 | API documentation |
| **Google Auth Library** | 10.3.0 | OAuth authentication |
| **node-rsa** | 1.1.1 | RSA encryption for biometrics |

---

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v18.0.0 or higher) - [Download](https://nodejs.org/)
- **npm** or **yarn** - Package manager
- **MongoDB** (v6.0 or higher) - [Download](https://www.mongodb.com/try/download/community)
- **Git** - Version control
- **Expo CLI** (for mobile development) - `npm install -g expo-cli`

### 📦 Installation

#### 1️⃣ Clone the Repository
```bash
git clone https://github.com/abhishekgurjarin/TradingX.git
cd TradeX
```

#### 2️⃣ Setup Backend Server

```bash
cd server

# Install dependencies
npm install

# Run setup script to generate secure keys and .env file
npm run setup

# Seed stock data (optional)
npm run seed

# Start development server
npm run dev
```

**Server will run on:**
- API Server: `http://localhost:3003`
- WebSocket Server: `ws://localhost:4003`
- API Documentation: `http://localhost:3003/api-docs`

#### 3️⃣ Setup Web Client

```bash
cd ../client-web

# Install dependencies
npm install

# Create environment file
cp .env.local.example .env.local

# Update .env.local with your configuration:
# NEXT_PUBLIC_API_URL=http://localhost:3003
# NEXT_PUBLIC_SOCKET_URL=http://localhost:4003

# Start development server
npm run dev
```

**Web app will run on:** `http://localhost:3000`

#### 4️⃣ Setup Mobile App

```bash
cd ../client-app

# Install dependencies
npm install

# Create environment file
cp .env.example .env

# Update .env with your configuration

# Start Expo development server
npm start

# Run on specific platform
npm run android  # For Android
npm run ios      # For iOS
npm run web      # For Web preview
```

---

## 🔧 Environment Variables

### Server (.env)
```env
# Database
MONGO_URI=mongodb://localhost:27017/tradex

# Server Configuration
PORT=3003
SOCKET_PORT=4003
NODE_ENV=development

# JWT Secrets (auto-generated by setup script)
JWT_SECRET=your_jwt_secret
REFRESH_TOKEN_SECRET=your_refresh_secret
ACCESS_TOKEN_EXPIRY=15m
REFRESH_TOKEN_EXPIRY=7d

# Email Configuration
EMAIL_USER=your_email@gmail.com
EMAIL_PASSWORD=your_app_password
EMAIL_FROM=TradeX <noreply@tradex.com>

# OAuth (Optional)
GOOGLE_CLIENT_ID=your_google_client_id
APPLE_CLIENT_ID=your_apple_client_id
```

### Web Client (.env.local)
```env
NEXT_PUBLIC_API_URL=http://localhost:3003
NEXT_PUBLIC_SOCKET_URL=http://localhost:4003
```

### Mobile App (.env)
```env
API_URL=http://192.168.x.x:3003
SOCKET_URL=http://192.168.x.x:4003
```

---

## 📡 API Documentation

### Base URLs
- **REST API**: `http://localhost:3003`
- **WebSocket**: `ws://localhost:4003`
- **Swagger Docs**: `http://localhost:3003/api-docs`

### Authentication Endpoints

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| POST | `/auth/check-email` | Check if email exists | ❌ |
| POST | `/auth/send-otp` | Send OTP to email | ❌ |
| POST | `/auth/verify-otp` | Verify OTP code | ❌ |
| POST | `/auth/register` | Register new user | ❌ |
| POST | `/auth/login` | User login | ❌ |
| POST | `/auth/oauth` | OAuth authentication | ❌ |
| POST | `/auth/refresh-token` | Refresh access token | ❌ |
| GET | `/auth/profile` | Get user profile | ✅ |
| PUT | `/auth/profile` | Update profile | ✅ |
| POST | `/auth/set-pin` | Set login PIN | ✅ |
| POST | `/auth/verify-pin` | Verify PIN | ✅ |
| POST | `/auth/upload-biometric` | Upload biometric key | ✅ |
| POST | `/auth/verify-biometric` | Verify biometric | ✅ |
| POST | `/auth/logout` | User logout | ✅ |

### Stock & Trading Endpoints

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| GET | `/stocks` | Get all stocks | ✅ |
| GET | `/stocks/stock?symbol=AAPL` | Get stock by symbol | ✅ |
| POST | `/stocks/register` | Register new stock | ✅ |
| POST | `/stocks/buy` | Buy stock | ✅ |
| POST | `/stocks/sell` | Sell stock | ✅ |
| GET | `/stocks/holding` | Get user holdings | ✅ |
| GET | `/stocks/order` | Get order history | ✅ |

### WebSocket Events

#### Client → Server
```javascript
// Subscribe to single stock
socket.emit('SubscibeToStocks', 'AAPL');

// Subscribe to multiple stocks
socket.emit('subscribeToMultipleStocks', ['AAPL', 'GOOGL', 'MSFT']);
```

#### Server → Client
```javascript
// Receive stock updates
socket.on('AAPL', (stockData) => {
  console.log(stockData);
  // { symbol, currentPrice, priceHistory, candles, ... }
});
```

---

## 📱 Application Screenshots

### Web Application
- **Dashboard**: Real-time stock overview with charts
- **Stock Detail**: Interactive candlestick charts with buy/sell options
- **Portfolio**: Holdings with profit/loss tracking
- **Orders**: Complete transaction history

### Mobile Application
- **Home Screen**: Quick access to watchlist and portfolio
- **Trading Screen**: Easy buy/sell interface
- **Profile**: Account management and settings
- **Charts**: Touch-optimized chart interactions

---

## 🧪 Testing

### API Testing
```bash
cd server

# Test all endpoints
npm test

# Or use the provided test script
node test-api.js
```

### Manual Testing with cURL
See `server/API_TESTING_GUIDE.md` for comprehensive cURL examples.

### WebSocket Testing
```bash
cd server
node testSocket.js
```

---

## 🚀 Deployment

### Backend Deployment (Railway/Render/Heroku)
```bash
# Build command
npm install

# Start command
npm start

# Environment variables
# Set all variables from .env file in platform dashboard
```

### Web Deployment (Vercel/Netlify)
```bash
# Build command
npm run build

# Output directory
.next

# Environment variables
# Set NEXT_PUBLIC_* variables in platform dashboard
```

### Mobile Deployment
```bash
# Build for production
expo build:android
expo build:ios

# Or use EAS Build
eas build --platform android
eas build --platform ios
```

---

## 📚 Project Structure Details

### Database Models

#### User Model
- Email, password, name
- Login PIN (hashed)
- Phone number, date of birth, gender
- Biometric key (RSA public key)
- Balance (default: ₹50,000)
- Wrong attempt tracking
- Account lockout mechanism

#### Stock Model
- Symbol, company name
- Current price
- Price history (1-min intervals)
- Candle data (10-min intervals)
- Market cap, sector, description

#### Order Model
- User reference
- Stock symbol
- Order type (BUY/SELL)
- Quantity, price
- Total amount
- Timestamp

#### Holding Model
- User reference
- Stock symbol
- Quantity
- Average buy price
- Current value
- Profit/loss

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. **Commit your changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/AmazingFeature
   ```
5. **Open a Pull Request**

### Coding Standards
- Follow ESLint configuration
- Write meaningful commit messages
- Add comments for complex logic
- Update documentation for new features
- Test thoroughly before submitting PR

---

## 🐛 Known Issues & Roadmap

### Current Limitations
- Stock data is simulated (not connected to real market APIs)
- Limited to predefined stock list
- No options/futures trading
- No social features (chat, forums)

### Future Enhancements
- [ ] Integration with real-time market data APIs (Alpha Vantage, Yahoo Finance)
- [ ] Advanced charting with technical indicators (RSI, MACD, Bollinger Bands)
- [ ] Watchlist management with alerts
- [ ] News feed integration
- [ ] Social trading features
- [ ] Paper trading competitions
- [ ] Advanced order types (stop-loss, limit orders)
- [ ] Portfolio analytics and insights
- [ ] Tax reporting and statements
- [ ] Multi-language support

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Abhishek Gurjar**
- GitHub: [@abhishekgurjarin](https://github.com/abhishekgurjarin)

---

## 🙏 Acknowledgments

Special thanks to the open-source community and these amazing projects:

- **[TradingView Lightweight Charts](https://github.com/tradingview/lightweight-charts)** - Professional financial charts
- **[Next.js](https://nextjs.org/)** - The React framework for production
- **[React Native](https://reactnative.dev/)** - Cross-platform mobile development
- **[Socket.IO](https://socket.io/)** - Real-time bidirectional communication
- **[Zustand](https://github.com/pmndrs/zustand)** - Minimal state management
- **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS framework
- **[MongoDB](https://www.mongodb.com/)** - NoSQL database
- **[Express.js](https://expressjs.com/)** - Fast, unopinionated web framework

---

## 📞 Support

For questions, issues, or feature requests:

- **GitHub Issues**: [Create an issue](https://github.com/abhishekgurjarin/TradeX/issues)
- **Documentation**: [API Docs](http://localhost:3003/api-docs)

---

<div align="center">
  <p>Made with ❤️ by Abhishek Gurjar</p>
  <p>⭐ Star this repo if you find it helpful!</p>
</div>
