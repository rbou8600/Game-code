# 🎯 JUNIOR QC ANALYST - Training Quiz

A multilingual interactive quiz application for training Junior QC Analysts on Customer Service best practices.

## 🌍 Supported Languages
- **English** 🇬🇧
- **Français** 🇫🇷
- **Italiano** 🇮🇹

## ✨ Features
- 📝 **20 Quiz Questions** across 5 categories
- ⏱️ **30 seconds per question** time limit
- ✅ **Explanation after each answer** for better learning
- 🎲 **5 Categories:**
  - CS Workflow
  - Quality Standards
  - Service Behavior
  - Communication
  - All Categories (mixed)
- 🌐 **Multilingual Support** - Switch languages instantly
- 💾 **Language Preference Saved** - Your language choice is remembered

## 📁 Project Structure
```
Game-code/
├── index.html          # Main HTML file with multilingual support
├── styles.css          # Complete CSS styling (Tailwind utilities)
├── script.js           # Quiz logic and interactivity
├── translations.js     # Translation system (EN, FR, IT)
└── README.md           # Documentation
```

## 🚀 Getting Started

### Option 1: Use GitHub Pages (Live)
1. Go to your repository settings
2. Enable GitHub Pages from the `main` branch
3. Your quiz will be live at: `https://rbou8600.github.io/Game-code/`

### Option 2: Local Development
```bash
# Clone the repository
git clone https://github.com/rbou8600/Game-code.git

# Navigate to the folder
cd Game-code

# Open in your browser
open index.html
# or just double-click the index.html file
```

## 📝 File Descriptions

### `index.html`
- Main structure of the quiz application
- Language selector buttons (EN, FR, IT)
- Multilingual content with `data-i18n` attributes
- Responsive grid layout
- Category selection interface

### `styles.css`
- Complete styling based on Tailwind CSS utilities
- Responsive design (mobile-first)
- Gradient backgrounds
- Button hover states
- Animation transitions
- Language button styles

### `script.js`
- Quiz functionality
- Category selection logic
- Quiz start handler
- Tooltip functions from original code
- Event listeners for interactivity

### `translations.js`
- Translation system for 3 languages
- `setLanguage(lang)` function to switch languages
- Automatic language preference saving to localStorage
- Easy to extend with more languages

## 🔄 How to Add More Questions

Edit `script.js` and add your questions array:

```javascript
const questions = {
  workflow: [
    {
      question: "What is the first step?",
      options: ["Option A", "Option B", "Option C"],
      correct: 0,
      explanation: "Explanation here"
    }
  ],
  quality: [
    // Add more questions
  ],
  // ... etc
};
```

## 🌐 How to Add a New Language

1. Edit `translations.js`
2. Add a new language object:
```javascript
const translations = {
  en: { ... },
  fr: { ... },
  it: { ... },
  es: {  // Add Spanish
    title: "ANALISTA QC JUNIOR",
    subtitle: "Prueba tus conocimientos sobre el servicio al cliente",
    // ... etc
  }
};
```

3. Add language button in `index.html`:
```html
<button onclick="setLanguage('es')" class="lang-btn" data-lang="es">Español</button>
```

## 🎨 Customization

### Change Colors
Edit `styles.css` color classes:
- `.bg-indigo-600` - Primary button color
- `.from-blue-50` - Gradient start color
- `.to-indigo-100` - Gradient end color

### Change Categories
Update category buttons in `index.html` with different emojis and topics

### Change Time Limit
Update quiz configuration in `script.js`

## 👨‍💻 Credits
- **Created by**: Ramzi
- **AI Assistance**: DeepSeek & Claude AI
- **Styling**: Tailwind CSS framework

## 📄 License
This project is open source and available under the MIT License.

## 🤝 Contributing
Feel free to fork, modify, and contribute to this project!

---

**Happy Learning! 🚀**
