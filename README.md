# nukrax.cr

> A minimal, secure cryptocurrency deposit portal with a focus on precision and user experience.

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![HTML](https://img.shields.io/badge/HTML-80.2%25-E34F26?logo=html5)](https://github.com/CosmoLanex/.cr)
[![JavaScript](https://img.shields.io/badge/JavaScript-19.8%25-F7DF1E?logo=javascript)](https://github.com/CosmoLanex/.cr)

## 🌟 Overview

**nukrax.cr** is a deposit-only crypto portal designed for simplicity and security. It provides users with instant access to verified deposit addresses across multiple cryptocurrencies and blockchain networks—no account required, no withdrawals, no trading.

Built with a focus on the **XRP ecosystem**, nukrax.cr supports multiple popular cryptocurrencies while maintaining a clean, minimal interface that prioritizes user experience.

### ✨ Key Features

- **🔐 Secure & Non-Custodial** - View deposit addresses only, with no withdrawal or trading capabilities
- **🚫 No Account Required** - Access deposit addresses instantly without registration
- **🎯 Multi-Asset Support** - XRP, SOL, USDT, USDC, BTC, ETH, MATIC, BNB, TRX, TWT, ADA
- **🌐 Multi-Network** - Support for various blockchain networks per asset
- **📱 Responsive Design** - Optimized for desktop, tablet, and mobile devices
- **🎨 Modern UI** - Clean, dark-themed interface with smooth animations
- **⚡ Fast & Lightweight** - Pure HTML/CSS/JS with no framework dependencies

## 🚀 Quick Start

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- A local web server (optional, for development)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/CosmoLanex/.cr.git
   cd .cr
   ```

2. **Serve the application**
   
   Using Python:
   ```bash
   python -m http.server 8000
   ```
   
   Using Node.js:
   ```bash
   npx http-server -p 8000
   ```
   
   Or simply open `index.html` in your browser.

3. **Access the portal**
   ```
   http://localhost:8000
   ```

## 📁 Project Structure

```
.cr/
├── index.html          # Main landing page with asset selection
├── crypto.html         # Deposit address display page
├── redirect.html       # Transition page between selection and display
├── data.js            # Cryptocurrency data configuration
└── assets/            # Static assets (logos, icons)
```

## 🎯 Usage

### For Users

1. **Select an Asset** - Choose from the available cryptocurrencies on the main page
2. **Select a Network** - Pick the appropriate blockchain network for your deposit
3. **View Address** - Copy the generated deposit address or scan the QR code
4. **Send Funds** - Use the address in your wallet to send funds

### For Developers

#### Adding a New Cryptocurrency

Edit `data.js` to add new cryptocurrencies:

```javascript
CRYPTO_DATA['SYMBOL'] = {
  name: 'Cryptocurrency Name',
  ticker: 'SYMBOL',
  icon: '🪙',
  networks: [
    {
      name: 'Network Name',
      badge: 'NETWORK',
      tag: 'best', // or 'suggested' or null
      address: 'your_deposit_address_here'
    }
  ]
};
```

#### Customizing the Theme

CSS variables are defined in `:root` in `index.html`:

```css
:root {
  --bg: #000000;
  --layer1: #0d0d0d;
  --text: #bfbfbf;
  --white: #ffffff;
  /* ... more variables */
}
```

## 🛠️ Technology Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Fonts**: Inter, Space Grotesk, Space Mono
- **QR Generation**: QRCode.js library
- **Animation**: CSS animations and transitions
- **Canvas**: Particle background effect

## 🎨 Design Philosophy

nukrax.cr follows a minimalist design philosophy:

- **Dark Theme** - Easy on the eyes with reduced eye strain
- **Glassmorphism** - Subtle frosted glass effects for depth
- **Smooth Animations** - Polished transitions and micro-interactions
- **Accessibility** - High contrast ratios and readable typography
- **Mobile-First** - Responsive design that works on all screen sizes

## 🔒 Security Features

- **Read-Only Access** - No private keys or sensitive data stored
- **Client-Side Only** - All operations happen in the browser
- **No Backend** - No server-side processing or data collection
- **No Tracking** - Privacy-focused with no analytics
- **Static Hosting Ready** - Can be deployed on any static host

## 📝 Supported Assets

| Asset | Networks | Status |
|-------|----------|--------|
| XRP   | XRP Ledger | ✅ Active |
| SOL   | Solana | ✅ Active |
| USDT  | Multiple | ✅ Active |
| USDC  | Multiple | ✅ Active |
| BTC   | Bitcoin | ✅ Active |
| ETH   | Ethereum | ✅ Active |
| MATIC | Polygon | ✅ Active |
| BNB   | BSC | ✅ Active |
| TRX   | Tron | ✅ Active |
| TWT   | Multiple | ✅ Active |
| ADA   | Cardano | ✅ Active |

## 🚧 Roadmap

- [ ] Add more cryptocurrency options
- [ ] Implement network status indicators
- [ ] Add transaction fee estimates
- [ ] Multi-language support
- [ ] Dark/Light theme toggle
- [ ] Address verification features
- [ ] Enhanced QR code customization

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

**IMPORTANT**: nukrax.cr is a deposit portal interface only. 

- This is **not a wallet** and does not store any funds
- Always verify addresses before sending any cryptocurrency
- The developers are not responsible for any lost or misdirected funds
- Use at your own risk

## 📧 Contact

- **Project**: [github.com/CosmoLanex/.cr](https://github.com/CosmoLanex/.cr)
- **Issues**: [github.com/CosmoLanex/.cr/issues](https://github.com/CosmoLanex/.cr/issues)

## 🙏 Acknowledgments

- Built around the **XRP ecosystem** and the **nukrax** project
- Inspired by minimal crypto infrastructure principles
- Thanks to all contributors and supporters

---

<div align="center">
  <strong>nukrax.cr</strong> — Deposit Portal<br>
  Secure · Non-custodial · Read-only
</div>
