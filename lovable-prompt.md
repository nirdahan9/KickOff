# Kickoff — Lovable Build Prompt

## What is Kickoff?
A social sports betting app (points-based, no real money). Users bet points on football (soccer) games — results, scorers, live events. Think Fabula Football but more modern.

---

## Design System

- **Mode:** Light / Bright
- **Style:** Minimal, modern, lots of whitespace — like Revolut or Cash App meets sports
- **Colors:**
  - Primary green: `#4CAF50`
  - Background: `#FFFFFF`
  - Card / secondary bg: `#F5F5F5`
  - Text: `#1A1A1A` (primary), `#757575` (secondary)
  - Interactive / CTA: `#4CAF50`
- **Typography:** Bold headings, clean body text
- **Components:** Rounded cards with soft shadows, pill-shaped buttons, clean tab bar
- **Language:** Hebrew (RTL layout) — all UI text in Hebrew

---

## App Screens to Build

### 1. Home / Feed
- Top bar: app logo (left in RTL), user points balance (right)
- "Games today" section — horizontal scroll of game cards
- Each game card shows: team logos, time, competition name, "Bet Now" button
- "My active bets" section below — cards showing open bets with status
- Bottom tab bar: Home | Leagues | Bet Slip | Quiz | Profile

### 2. Game Detail / Bet Screen
- Game header: team A vs team B, date + time, competition
- Bet questions (2-3 per game):
  - Q1: "מי ינצח?" — options: Team A / Draw / Team B (always first)
  - Q2: e.g., "כמה קרנות יהיו?" — options as buttons
  - Q3: e.g., "מי יכבוש?" — player list as selectable cards
- Points input field (how many points to bet)
- "הוסף לתלוש" (Add to bet slip) button
- Live badge if game is in progress

### 3. Bet Slip
- List of selected bets
- Parlay toggle (combine bets)
- Total points at risk
- Potential winnings
- "אשר הימור" (Confirm Bet) CTA button

### 4. Private Leagues
- "הליגות שלי" — list of joined leagues with rank + points
- "צור ליגה" (Create League) button → form:
  - League name
  - Access: Open / Invite only
  - Format: Pool (winner takes all) / Per-game fee
  - Duration: Full season / Single round / Tournament
  - Minimum bet amount
  - Allowed competitions (multi-select)
- League detail screen: leaderboard, member list, settings (for manager)
- Invite via link button

### 5. Quiz / Trivia
- Daily card style: question about upcoming games or general football trivia
- 4 answer options as large tap buttons
- Points reward shown after answer
- "שאלה הבאה" (Next Question) to keep going
- Score / streak counter at top

### 6. AI Betting Advisor (Chat)
- Floating button on Game Detail screen: "שאל את הAI" with a small robot/sparkle icon
- Opens a chat drawer / bottom sheet
- User types a question in Hebrew: e.g., "כדאי לי להמר על ברצלונה היום?"
- AI responds with a short analysis: recent form, head-to-head history, key stats
- Response style: friendly, data-driven, always includes a disclaimer like "בהתבסס על נתוני העבר בלבד"
- Chat history persists per game
- Placeholder response for Lovable: mock a realistic AI answer card

### 7. Leaderboard
- Tabs: Global | Friends | My Leagues
- Row per user: rank, avatar, name, points
- Highlight current user's row

### 8. Profile
- Avatar + username
- Total points, bets won/lost stats
- Bet history list
- Settings: notifications, language (Hebrew/English), logout

### 9. Auth / Onboarding
- Splash screen with Kickoff logo
- Login options: Google | Facebook | Email
- Age confirmation checkbox (18+)
- Short onboarding tutorial (3 slides): how points work, how to bet, how leagues work

---

## Key Interactions
- Tap a game → opens Game Detail
- Swipe on game card → quick-add result bet
- Long press on league → share invite link
- Quiz answer tap → instant feedback (green ✓ / red ✗) then next question

---

## Notes for Lovable
- All text RTL (Hebrew)
- No real money anywhere — only "נקודות" (points)
- Start with these screens: Home, Game Detail, Bet Slip, Private Leagues
- Use placeholder data for teams/games (real API connected later)
- Mobile-first, iOS look and feel
