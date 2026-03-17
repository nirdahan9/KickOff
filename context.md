# Kickoff - Project Context

## Overview
A social sports betting app (points-based, no real money) similar to Fabula Football and playfootball.games.
Users bet with points on sports games - results, stats, and live in-game events.

---

## App Name
**Kickoff**

---

## Target Audience
- Age: Young adults to adults (18+, age verification required)
- Knowledge: Basic sports background
- Language: Hebrew first, English support added later
- Region: Israel initially, international expansion planned

---

## Platform
- **Phase 1:** iOS (React Native)
- **Phase 2:** WhatsApp bot for managing leagues inside group chats

---

## Core Features

### Betting
- Bet types: Final result / winner (always included), + 1-2 additional options per game (corners, scorers, lineups, etc.)
- **2-3 bet questions per game minimum**
- Live betting: Yes — all bet types available both pre-game and in-game (same as standard sportsbooks)
- Parlays: Yes (combined bets across multiple games)
- Sports: **Football (soccer) only** in Phase 1, more sports added later

### Points System
- Currency: Points (no real money)
- Ways to earn points:
  - Winning bets
  - Inviting friends (referral)
  - Sports quizzes (playfootball.games style)
- Points usage: Betting only (no in-app store for now)
- Real money purchase: Not in Phase 1, may be added later

### Private Leagues
**(Highest priority feature)**
- Create private leagues with invite links
- League manager controls:
  - Open/invite-only access
  - Minimum bet amount
  - Allowed competitions (e.g., Champions League only)
- **Two league formats:**
  1. **Pool format:** Fixed entry fee → winner takes all (or most) of the pool at season end
  2. **Per-game format:** Fixed fee per game
- **Duration options:** Full season, single round, cup-style tournament — all available

### Leaderboards & Social
- General leaderboard (global)
- Private league leaderboards
- Friends competition

---

## Authentication
- Google login
- Meta (Facebook) login
- Email + password
- Age verification: Must confirm 18+

---

## Onboarding
- First-time user onboarding flow / tutorial screen

---

## Notifications (Push)
- Bet result: win or loss notification
- Game starting soon
- Other relevant updates

---

## Sports Data API
- Real-time football data via a **free API** (to be selected)
- Candidates: football-data.org, API-Football (free tier), TheSportsDB
- Bet questions generated **automatically** from API data
- Always includes final result or winner as one of the options

---

## Admin Panel
- Access: Developers only
- Full analytics:
  - Total users
  - Active users (DAU/MAU)
  - User geographic distribution
  - Bets placed (by time range, type, game)
  - Detailed logs and statistics — as comprehensive as possible

---

## Future Plans
- English language support
- Additional sports (basketball, tennis, NFL, etc.)
- WhatsApp bot for league management
- Potential points purchase with real money
- Potential real-money betting (depends on regulation)

---

## Design Preferences
- TBD (to be discussed)

---

## Open Questions
- Design style: dark/light mode? color palette? reference apps?
- Monetization: ads? premium league features?
- Quiz format: how exactly do sports quizzes work — timed? daily? tied to upcoming games?

---

*Last updated: 2026-03-17*
