```markdown
# EchoLedger

A public, transparent follower ledger that visualizes Instagram followers as immutable entries sourced from a repository file.

[![License](https://img.shields.io/badge/License-ESAL--1.0-blue.svg)](LICENSE)
[![Netlify](https://img.shields.io/badge/Deployed_on-Netlify-00C7B7.svg)](https://echo-ledger.netlify.app)

## ✨ Features

- **Public Ledger Interface** – Clean, card-based display of followers with avatars and badges
- **Real-time Search & Filtering** – Sort by date, alphabetical order, or follower type (OG/SPC/KF)
- **Focus Mode** – Temporarily dims animated username lanes to focus on ledger content
- **Expanding Entry Cards** – Click any card to expand it for detailed view
- **Theme System** – Dark/light themes with distinct visual personalities
- **Removal Request System** – Respectful interface for users to request removal from the ledger
- **Privacy & Safety Pages** – Clear documentation of data practices and platform rules
- **Client-side Analytics** – Visit counter using localStorage (no external tracking)
- **Responsive Design** – Works across desktop and mobile devices
- **Source-Available License** – ESAL-1.0 with clear attribution requirements

## 📁 Folder Structure

```
echoledger/
├── index.html              # Main ledger page
├── removalreq.html         # Removal request page
├── dnp.html                # Data & privacy policy
├── ps.html                 # Platform safety rules
├── LICENSE                 # License & authorship page
├── followers/
│   └── index.txt          # Data source (username m/f OG/SPC/KF)
└── assets/
    ├── avatar/
    │   ├── m.png          # Male avatar
    │   └── f.png          # Female avatar
    └── badge/
        ├── OG.png         # Early supporter badge
        ├── SPC.png        # Special follower badge
        └── KF.png         # Known follower badge
```

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/ximantaxyz/echoledger.git
   cd echoledger
   ```

2. **Add your data**
   - Create `followers/index.txt`
   - Format: `username m/f OG/SPC/KF` (one per line)
   - Example: `johndoe m OG KF`

3. **Deploy**
   - The project is static and ready to deploy
   - Upload all files to any static hosting service
   - No build process or dependencies required

## 📋 Data Format

`followers/index.txt` uses space-separated values:
```
username gender badge1 badge2...
```

**Fields:**
- `username`: Instagram username (exact)
- `gender`: `m` (uses `assets/avatar/m.png`) or `f` (uses `assets/avatar/f.png`)
- `badges`: Zero or more of: `OG` (first 100), `SPC` (special), `KF` (known follower)

**Example lines:**
```
alicewonder f OG SPC
bobbuilder m KF
charliech f OG KF
```

## 🎨 Design System

- **Dark Theme**: Electric cyan accent (`#00e6ff`) with subtle glow effects
- **Light Theme**: Warm pink accent (`#ff4d8d`) with clean, editorial feel
- **Typography**: Inter font family with deliberate weight hierarchy
- **Motion**: Cubic-bezier easing, subtle hover lifts, disciplined animations
- **Layout**: Card-based grid with consistent spacing and border radius

## 📄 Pages

### `index.html` – Main Ledger
- Displays all followers from `followers/index.txt`
- Interactive sorting (Oldest → Latest, A → Z, filter by badge type)
- Expandable cards with detailed view
- Animated username lanes

### `removalreq.html` – Removal Request
- Search interface to find usernames
- Optional screenshot upload for verification
- Telegram bot integration for request submission
- Success confirmation flow

### `dnp.html` – Data & Privacy
- Clear explanation of what data is/is not collected
- Removal rights and process
- Data retention policy

### `ps.html` – Platform Safety
- Usage guidelines and restrictions
- Reporting procedures
- Community expectations

### `LICENSE` – License & Authorship
- ESAL-1.0 license terms
- Author profile with social links
- Attribution requirements

## ⚖️ License

EchoLedger is released under the **EchoLedger Source-Available License (ESAL-1.0)**.

**Key terms:**
- ✅ Personal, educational, and non-profit use allowed
- ✅ Modifications permitted with clear attribution
- ✅ Public deployment allowed with visible credit
- ❌ Commercial use prohibited
- ❌ Removal of attribution prohibited
- ❌ Rebranding or white-labeling prohibited

**Required attribution:** `EchoLedger by Ximanta`

See [LICENSE](LICENSE) for complete terms.

## 👨‍💻 Author

**Ximanta Bhuyan**

- Portfolio: [about.ximanta.space](https://about.ximanta.space)
- Instagram: [@ximanta.xyz_](https://instagram.com/ximanta.xyz_)
- Telegram: [@ximantaxyz](https://t.me/ximantaxyz)
- X: [@ximantaxyz](https://x.com/ximantaxyz)
- Email: ximanta.official@gmail.com

## 🌐 Deployment

The project is configured for deployment on **Netlify**:

1. Push to GitHub
2. Connect repository to Netlify
3. Deploy with default settings

No build command required – deploy as static files.

## 🤝 Contributing

While EchoLedger is a personal project, feedback and respectful suggestions are welcome. Please review the platform safety guidelines before engaging.

## ⚠️ Disclaimer

EchoLedger displays publicly available Instagram usernames only. No private data is collected or displayed. Users can request removal at any time via the removal request page.

--- 

<a href="https://buymeacoffee.com/tukuexe" target="_blank">
  <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" 
       alt="Buy Me A Coffee" 
       style="height: 60px; width: 217px;">
</a>

---

*EchoLedger by Ximanta – An open ledger of real followers*
```