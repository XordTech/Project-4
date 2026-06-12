# Algebra Champions - Educational Game Specification

## 1. Project Overview

**Project Name:** Algebra Champions - Quest for Mathematical Heroism

**Project Type:** Multi-page interactive educational web game

**Core Functionality:** An adventure-themed algebra learning game where elementary school students (ages 8-12) solve mathematical challenges to progress through magical worlds, earn rewards, and become "Algebra Champions."

**Target Users:** Basic school students beginning algebra (grades 3-6), parents, and educators

---

## 2. Site Structure

### Pages
1. **index.html** - Home page with game introduction and play button
2. **about.html** - About the game, learning objectives, features
3. **contact.html** - Contact form for feedback
4. **game.html** - Main game interface with all levels

---

## 3. UI/UX Specification

### Color Palette
- **Primary Blue:** #3B82F6 (buttons, headers)
- **Primary Green:** #22C55E (success, correct)
- **Primary Orange:** #F97316 (stars, coins, rewards)
- **Primary Yellow:** #FBBF24 (highlights, badges)
- **Primary Purple:** #8B5CF6 (magical elements)
- **Background Dark:** #1E1B4B (space world)
- **Background Forest:** #064E3B (forest world)
- **Background Castle:** #4C1D95 (castle world)
- **Background Ocean:** #0E7490 (island world)
- **Text Light:** #F8FAFC
- **Text Dark:** #1E293B
- **Error Red:** #EF4444

### Typography
- **Primary Font:** 'Fredoka One', cursive (headings, headings)
- **Secondary Font:** 'Nunito', sans-serif (body text)
- **Heading Sizes:** H1: 48px, H2: 36px, H3: 28px
- **Body Size:** 18px (large for children)
- **Button Text:** 20px bold

### Spacing System
- **Section Padding:** 60px
- **Card Padding:** 30px
- **Button Padding:** 16px 32px
- **Gap Between Elements:** 20px

### Visual Effects
- **Card Shadows:** 0 10px 40px rgba(0,0,0,0.2)
- **Button Hover:** scale(1.05), brightness increase
- **Animations:** bounce, fadeIn, slideIn, pulse
- **Transitions:** all 0.3s ease

### Responsive Breakpoints
- **Mobile:** < 768px
- **Tablet:** 768px - 1024px
- **Desktop:** > 1024px

---

## 4. Page Specifications

### 4.1 Home Page (index.html)
**Header:**
- Animated logo "Algebra Champions" with crown icon
- Navigation: Home | About | Contact | Play Now (button)

**Hero Section:**
- Large hero image showing game character (Algebra Hero mascot)
- Headline: "Embark on an Epic Math Adventure!"
- Sub-headline: "Learn algebra while saving magical worlds"
- CTA Button: "START ADVENTURE" (large, orange, animated)
- Floating math symbols animated in background

**Features Section:**
- 4 icon cards showing game features
- Icons: Star (rewards), Globe (worlds), Brain (learn), Trophy (win)
- Brief descriptions for each

**Preview Section:**
- Screenshot carousel of game levels
- "See the Adventure" mini-gallery

**Footer:**
- Copyright info
- Social links (icons)

### 4.2 About Page (about.html)
**Header:** Same as home

**Hero:**
- Title: "About Algebra Champions"
- Subtitle: "Making math magical for young learners"

**Learning Objectives:**
- Grid of 8 topic cards with icons
- Variables, Letters, Expressions, Like Terms
- Equations, Substitution, Word Problems, Real-Life Apps

**Game Features:**
- List of interactive activities
- Matching, Drag-drop, Puzzles, Mazes, Quizzes

**Levels Overview:**
- World map preview
- 5 worlds: Forest 1-5, Village 6-10, Castle 11-15, Space 16-20, Island 21-25

**Rewards System:**
- Visual display of rewards: Stars, Coins, Badges, Trophies

### 4.3 Contact Page (contact.html)
**Header:** Same as home

**Form Section:**
- Name input (required)
- Email input (required)
- Role selector: Student | Parent | Teacher | Other
- Message textarea
- Submit button

**Info Section:**
- Contact information
- FAQ link

### 4.4 Game Page (game.html)
**Main Layout:**
- Full-screen game container
- Top bar: Coins | Stars | Level | Timer
- Left sidebar: Character guide (animated mascot)
- Center: Game play area
- Right panel: Problems/Answers

**Game Worlds (5):**
1. **Whispering Woods** (Levels 1-5) - Forest theme, learn variables
2. **Crystal Village** (Levels 6-10) - Village theme, expressions
3. **Enchanted Castle** (Levels 11-15) - Castle theme, equations
4. **Space Station Alpha** (Levels 16-20) - Space theme, substitution
5. **Treasure Island** (Levels 21-25) - Island theme, word problems

**Activity Types:**
- Multiple Choice
- Drag and Drop Tiles
- Fill in Missing
- Equation Solver
- Maze Navigation
- Mini-games

**Reward System:**
- Stars: Correct answers (1-3 per problem)
- Coins: Level completion
- Badges: Achievement unlocks
- Trophies: World completion

**Feedback System:**
- Correct: Green checkmark, celebratory animation, motivational message
- Incorrect: Red X, hint appearance, step-by-step explanation, retry option

**Accessibility:**
- Voice read button for problems
- Difficulty selector: Easy | Medium | Hard
- Text size: Normal | Large | Extra Large
- High contrast mode toggle

---

## 5. Game Content Specification

### Level Structure
Each world has 5 levels with increasing difficulty:

**Whispering Woods (Variables):**
- Level 1: What is a variable? (intro)
- Level 2: Matching letters to numbers
- Level 3: Finding values
- Level 4: Understanding x
- Level 5: Forest Boss Challenge

**Crystal Village (Expressions):**
- Level 6: Simple expressions
- Level 7: Adding like terms
- Level 8: Subtracting like terms
- Level 9: Combining terms
- Level 10: Village Boss Challenge

**Enchanted Castle (Equations):**
- Level 11: What is an equation?
- Level 12: Balance两边
- Level 13: Solving for x
- Level 14: Multi-step equations
- Level 15: Castle Boss Challenge

**Space Station Alpha (Substitution):**
- Level 16: What is substitution?
- Level 17: Substituting into expressions
- Level 18: Real-world substitution
- Level 19: Advanced substitution
- Level 20: Space Boss Challenge

**Treasure Island (Word Problems):**
- Level 21: Shopping problems
- Level 22: Age problems
- Level 23: Distance problems
- Level 24: Sharing problems
- Level 25: Final Boss Challenge

---

## 6. Functionality Specification

### Core Features
1. **Level Selection:** Click on world/level to play
2. **Problem Display:** Show algebra problem with visual representation
3. **Answer Input:** Multiple choice, text input, or drag-drop
4. **Feedback System:** Instant correct/incorrect feedback
5. **Progress Tracking:** Save progress to localStorage
6. **Reward System:** Award stars, coins, badges
7. **Leaderboard:** Display high scores (localStorage)
8. **Hints System:** Show animated hints after mistakes
9. **Retry System:** Allow unlimited retries without penalty

### Navigation
- Single page application for game
- Smooth transitions between levels
- World map for level selection
- Back to home button

### Data Handling
- localStorage for: progress, coins, stars, unlocked levels
- Session storage for: current level state
- No external database required

---

## 7. Acceptance Criteria

### Visual Checkpoints
- [ ] All pages load without errors
- [ ] Colors match specification exactly
- [ ] Animations are smooth and child-friendly
- [ ] Text is large and readable
- [ ] Buttons are minimum 48px height
- [ ] All icons/images display properly

### Functional Checkpoints
- [ ] Home page navigation works
- [ ] About page displays all learning objectives
- [ ] Contact form validates inputs
- [ ] Game loads with level selection
- [ ] Problems display correctly
- [ ] Answer selection works
- [ ] Feedback shows on answer
- [ ] Progress saves to localStorage
- [ ] Rewards display correctly

### Accessibility Checkpoints
- [ ] Voice read button works (using Web Speech API)
- [ ] Text size options work
- [ ] Difficulty options work
- [ ] High contrast mode works

---

## 8. Technical Implementation

### File Structure
```
/my projects/
  index.html      (Home page)
  about.html     (About page)
  contact.html   (Contact page)
  game.html      (Main game)
  /css/
    style.css    (All styles)
  /js/
    game.js     (Game logic)
    data.js     (Problem data)
  /assets/
    /images/
    /sounds/
  SPEC.md
```

### External Dependencies
- Google Fonts: Fredoka One, Nunito
- Font Awesome 6.x for icons
- No external JS frameworks

### Browser Support
- Chrome (latest)
- Firefox (latest)
- Edge (latest)
- Safari (latest)