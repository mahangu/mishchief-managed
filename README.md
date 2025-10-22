# ⚡ Mischief Managed ⚡

A beautiful, interactive web app for testing your Harry Potter knowledge! Features 500 verified trivia questions from the books, with multiple study modes and progress tracking.

![Mischief Managed](https://img.shields.io/badge/Questions-500-gold?style=for-the-badge)
![Pure Vanilla JS](https://img.shields.io/badge/Framework-None-burgundy?style=for-the-badge)
![Mobile Optimized](https://img.shields.io/badge/Mobile-Optimized-green?style=for-the-badge)

## ✨ Features

### 📚 Browse Mode
- View flash cards one at a time with 3D flip animation
- Filter by difficulty (Easy, Medium, Hard) and category
- Navigate with Previous/Next buttons or keyboard arrows
- Shuffle questions for random order
- Track progress through the deck

### 🎯 Quiz Mode
- Take quizzes with 10 random questions
- Self-score your answers (Got it right / Got it wrong)
- View detailed results with correct answers
- Automatic tracking of missed questions

### 🔍 Review Mode
- Study questions you've marked wrong in previous quizzes
- See how many times you've missed each question
- Clear individual questions once mastered
- Persistent storage across sessions

### 📊 Statistics
- Track total quizzes completed
- View overall accuracy percentage
- See accuracy breakdown by category and difficulty
- Review your top 5 most missed questions
- Reset all progress when needed

### ⌨️ Keyboard Shortcuts
- **Arrow Keys**: Navigate previous/next
- **Space/Enter**: Flip card
- Works in all modes!

### 📱 Mobile Optimized
- Fully responsive design (320px to desktop)
- Touch-friendly buttons (44px+ tap targets)
- Smooth 3D card flips optimized for mobile performance
- No horizontal scrolling on any screen size

## 🚀 Quick Start

### Local Setup
1. Download or clone this repository
2. Open `index.html` in any modern web browser
3. That's it! No installation or build process required.

```bash
cd hp-flashcards
open index.html
# or just double-click index.html in your file browser
```

## 🌐 Deployment Options

### Option 1: Netlify (Drag & Drop - Easiest!)
1. Go to [app.netlify.com](https://app.netlify.com)
2. Sign up or log in
3. Drag the entire `hp-flashcards` folder into the Netlify browser window
4. Your site is live! Netlify gives you a URL like `https://your-site-name.netlify.app`

**No GitHub account required!**

### Option 2: Vercel (Drag & Drop)
1. Go to [vercel.com](https://vercel.com)
2. Sign up or log in
3. Click "Add New Project" → "Deploy without Git"
4. Upload your `index.html` and `trivia_data.json` files
5. Your site is live! You get a URL like `https://your-site-name.vercel.app`

**No GitHub account required!**

### Option 3: Surge.sh (CLI - Super Fast)
1. Install Surge globally:
   ```bash
   npm install -g surge
   ```

2. Deploy from your project directory:
   ```bash
   cd hp-flashcards
   surge
   ```

3. Follow the prompts. Your site is live at `https://your-chosen-name.surge.sh`

**No GitHub account required!**

### Option 4: GitHub Pages (If You Want Git)
1. Create a new GitHub repository
2. Push your files to the repository
3. Go to Settings → Pages
4. Select your main branch as the source
5. Your site will be live at `https://username.github.io/repo-name`

### Option 5: Neocities (Old School!)
1. Go to [neocities.org](https://neocities.org)
2. Create a free account
3. Upload `index.html` and `trivia_data.json` via the dashboard
4. Your site is live at `https://yourname.neocities.org`

**No GitHub account required!**

## 📁 Project Structure

```
hp-flashcards/
├── index.html          # Complete single-file app
├── trivia_data.json    # 50 trivia questions
└── README.md           # This file
```

## 🎨 Tech Stack

- **HTML5** - Semantic structure
- **CSS3** - Custom styling with CSS Grid/Flexbox
- **Vanilla JavaScript** - No frameworks or dependencies
- **Google Fonts** - Cinzel (headings) & Crimson Text (body)
- **localStorage** - Progress persistence

## 📝 Trivia Questions

The app includes 500 Harry Potter trivia questions:
- **~200 Easy** (40%) - Basic HP knowledge
- **~200 Medium** (40%) - Requires good book knowledge
- **~100 Hard** (20%) - Deep cuts and detailed facts

**Categories:**
- Spells
- Potions
- Characters
- Locations
- History
- Creatures
- Quidditch
- Hogwarts

### ⚠️ Important: Verify Questions
The questions are marked as `"verified": true` in the JSON file, but **you should verify them yourself** by cross-referencing with the [Harry Potter Wiki](https://harrypotter.fandom.com/) to ensure 100% accuracy. Each question includes a book citation to help with verification.

## 🎮 How to Use

### Browse Mode
1. Use filters to narrow down questions by difficulty or category
2. Click/tap the card to flip and reveal the answer
3. Navigate with Previous/Next buttons or arrow keys
4. Click Shuffle to randomize the order

### Quiz Mode
1. Click "Start Quiz" to begin a 10-question quiz
2. Read the question, flip to see the answer
3. Click "✓ Got it right" or "✗ Got it wrong"
4. View your results and review wrong answers

### Review Mode
1. Access questions you've marked wrong in previous quizzes
2. Study them like browse mode
3. Clear individual questions once you've mastered them

### Statistics
1. View your overall performance metrics
2. See which categories and difficulties you excel at
3. Review your most missed questions
4. Reset all progress if you want to start fresh

## 🛠️ Customization

### Adding More Questions
Edit `trivia_data.json` and add new questions following this format:

```json
{
  "id": 501,
  "question": "Your question here?",
  "answer": "The answer here",
  "category": "Spells",
  "difficulty": "medium",
  "source": "Book Title, Chapter X",
  "verified": true
}
```

### Changing Colors
Edit the CSS variables in `index.html` around line 19:

```css
:root {
    --burgundy: #722F37;    /* Primary color */
    --gold: #D4AF37;        /* Accent color */
    --dark-brown: #3E2723;  /* Background color */
    --light-cream: #F5F1E8; /* Text color */
}
```

### Changing Fonts
Replace the Google Fonts link in the `<head>` section and update the `font-family` in CSS.

## 📱 Browser Compatibility

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🐛 Troubleshooting

**Questions not loading?**
- Make sure `trivia_data.json` is in the same directory as `index.html`
- Check browser console for errors (F12 → Console tab)

**Filters not working?**
- Clear your browser cache and reload
- Make sure JavaScript is enabled

**Progress not saving?**
- Check that localStorage is enabled in your browser
- Private/Incognito mode may not persist data

**Cards not flipping on mobile?**
- Make sure you're tapping directly on the card
- Try a different mobile browser

## 📄 License

This project is open source and available for personal and educational use. Harry Potter and all related characters and elements are trademarks of Warner Bros. Entertainment Inc.

## 🙏 Credits

- **Trivia Questions**: Based on the Harry Potter book series by J.K. Rowling
- **Design Inspiration**: Gryffindor house colors
- **Fonts**: Google Fonts (Cinzel & Crimson Text)

## 🚀 Future Enhancements

Potential features to add:
- [ ] Timer mode for speed challenges
- [ ] Multiplayer quiz mode
- [ ] Question difficulty voting
- [ ] Export quiz results as PDF
- [ ] Dark mode toggle
- [ ] Custom quiz length (5, 10, 20 questions)
- [ ] Leaderboard (with backend)

## 📧 Questions?

If you encounter any issues or have suggestions, feel free to open an issue or submit a pull request!

---

Made with ⚡ and magic by a Harry Potter fan
