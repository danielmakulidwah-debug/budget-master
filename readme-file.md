# Budget Master - Personal Finance Management App

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)

A comprehensive personal finance management application designed for Malawians to track income, expenses, and budgets across multiple accounts including TNM Mpamba, Airtel Money, and bank accounts.

## 🌟 Features

### 💰 Multi-Account Balance Tracking
- Manual balance entry
- TNM Mpamba integration via SMS
- Airtel Money integration via SMS
- Bank account tracking
- Real-time balance updates with timestamps

### 📊 Transaction Management
- Record income and expenses
- OCR receipt scanning (auto-fill from photos)
- Transaction history with delete functionality
- Category-based organization
- Date and account tracking

### 📈 Budget Planning
- Category-based budgets
- Visual progress bars
- Real-time spending alerts
- Monthly budget tracking
- Expense item breakdown

### 🎯 Savings Goals (NEW)
- Create multiple savings goals
- Progress tracking with visual indicators
- Daily/Weekly/Monthly savings targets
- Smart notifications and reminders
- Status indicators (On Track, Behind, Ahead)

### 📱 SMS Balance Integration
- Parse balance from SMS notifications
- Auto-detect TNM Mpamba and Airtel Money
- Manual account selection for ambiguous messages
- USSD code quick-dial helpers

### 📊 Reports & Analytics
- Income vs Expense summary
- Net savings calculation
- Transaction overview statistics
- Export to CSV format

### 💾 Data Management
- Complete backup (JSON format)
- Restore from backup
- Export transactions (CSV)
- Clear all data option

## 🚀 Getting Started

### Files Required
Make sure you have these files in your hosting directory:

```
budget-master/
├── index.html              # Main overview page
├── add-transaction.html    # Transaction entry page
├── budget.html            # Budget planner page
├── savings-goals.html     # Savings goals tracker
└── README.md             # This file
```

### Installation

1. **Download all files** to your computer

2. **Upload to web hosting:**
   - Use any web hosting service (GitHub Pages, Netlify, Vercel, etc.)
   - Or use a local web server for testing

3. **No dependencies required:**
   - Pure HTML, CSS, and JavaScript
   - All libraries loaded from CDN
   - Works offline after first load

### Local Testing

Open `index.html` in any modern web browser:
- Chrome (recommended)
- Firefox
- Safari
- Edge

## 📖 User Guide

### Setting Up Balance

1. Click the **balance dropdown** on the overview page
2. Select your account (Manual, TNM Mpamba, Airtel Money, Bank)
3. Click **"Update Balance"** or **"Check USSD"**
4. For USSD:
   - Dial the provided code (*444# for Mpamba/Airtel)
   - Copy the SMS with your balance
   - Paste into the app

### Adding Transactions

1. Go to **"Add Transaction"** tab
2. Optional: Use camera/upload to scan receipt (OCR)
3. Fill in:
   - Type (Income/Expense)
   - Amount
   - Category
   - Description
   - Date
   - Account
4. Click **"Add Transaction"**

### Creating Budgets

1. Go to **"Budgets"** tab
2. Select a category
3. Set budget limit
4. Add expense items
5. Click **"Add to Overview"**
6. Track progress on the home page

### Setting Savings Goals

1. Click **hamburger menu (☰)** → **"Goals & Savings"**
2. Click **"Create New Savings Goal"**
3. Enter:
   - Goal name (e.g., "Emergency Fund")
   - Target amount
   - Current savings
   - Target date
   - Category
4. View daily/weekly/monthly targets
5. Add savings anytime with the **+** button

### Exporting Data

1. Menu → **"Export Data"**
2. Options:
   - **Export as CSV**: Download all transactions
   - **Backup All Data**: Full JSON backup
   - **Restore from Backup**: Upload previous backup

## 🔧 Technical Details

### Technologies Used
- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Custom CSS with modern design patterns
- **Icons**: Font Awesome 6.5.1
- **Storage**: localStorage (browser-based)
- **OCR**: OCR.space API (for receipt scanning)

### Browser Support
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Data Storage
All data is stored locally in the browser using localStorage:
- Transactions
- Account balances
- Category budgets
- Savings goals
- Settings

**Important**: Data is device-specific. Use the backup feature to transfer data between devices.

## 🌍 Localization

Currently supports:
- **Currency**: MWK (Malawian Kwacha)
- **Language**: English
- **Mobile Money**: TNM Mpamba, Airtel Money
- **Banks**: Standard Bank, National Bank, FDH Bank, NBS Bank

## 🔐 Privacy & Security

- **No server**: All data stays on your device
- **No login required**: No personal information collected
- **No tracking**: No analytics or third-party scripts
- **Offline capable**: Works without internet after first load
- **PIN protection**: Optional PIN lock (coming soon)

## 📞 Support

**Developer**: Daniel Makulidwa  
**Title**: IT Technician  
**Location**: Malawi  
**Email**: danielmakulidwah@gmail.com  
**Phone**: +265 886 872 397 / +265 881 381 486  
**WhatsApp**: +265 886 872 397

## 🐛 Known Issues

1. **SMS Parsing**: May not work with all SMS formats
2. **OCR**: Requires internet connection
3. **PDF Export**: Coming in future update
4. **Excel Export**: Coming in future update

## 🔄 Version History

### Version 1.0.0 (January 2026)
- Initial release
- Multi-account balance tracking
- Transaction management
- Budget planning
- Savings goals tracker
- SMS integration
- Export functionality

## 📜 License

MIT License - Free to use and modify

## 🙏 Acknowledgments

- Font Awesome for icons
- OCR.space for receipt scanning API
- Cloudflare CDN for hosting libraries

## 🚀 Deployment Options

### GitHub Pages (Free)
1. Create GitHub repository
2. Upload files
3. Enable GitHub Pages in settings
4. Access at: `https://username.github.io/budget-master`

### Netlify (Free)
1. Drag and drop folder to Netlify
2. Get instant URL
3. Custom domain optional

### Vercel (Free)
1. Import from GitHub
2. Auto-deploy on push
3. Custom domain support

---

**Built with ❤️ in Malawi**  
© 2026 Budget Master - Daniel Makulidwa