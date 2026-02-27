# RED DEVILS 2026 FANTASY BASEBALL DRAFT
## Complete Project Documentation

**Created:** February 2026
**Draft Date:** Saturday, March 14, 2026 @ 12:00 PM Central
**Location:** The Farm
**Season:** 40th Year

---

# TABLE OF CONTENTS

1. [Project Overview](#project-overview)
2. [Files Created](#files-created)
3. [League Structure](#league-structure)
4. [Draft Order & Snake Format](#draft-order)
5. [Owner Scouting Profiles](#owner-profiles)
6. [Google Sheets Setup](#google-sheets-setup)
7. [HTML Dashboard Connection](#html-connection)
8. [Draft Day Workflow](#draft-day-workflow)
9. [Strategic Tools Built](#strategic-tools)
10. [What's Still Needed](#whats-needed)

---

# PROJECT OVERVIEW <a name="project-overview"></a>

## The Goal
Build a draft system where:
- **You** update picks in Google Sheets (dropdowns, auto-complete)
- **HTML Dashboard** automatically displays updated charts, standings, rosters
- **Claude** can read the Google Sheet to provide strategic recommendations

## The Three Components

| Component | Purpose | Who Uses It |
|-----------|---------|-------------|
| **Google Sheet** | Data entry (dropdowns for picks) | You during draft |
| **HTML Dashboard** | Visuals (charts, standings, rosters) | You during draft |
| **Claude** | Strategy (analysis, recommendations) | You ask when it's your turn |

---

# FILES CREATED <a name="files-created"></a>

## 1. RedDevils2026_DraftTracker.xlsx
**Primary draft tracking spreadsheet**

### Tabs:
| Tab | Purpose |
|-----|---------|
| **Players** | Master list of 150+ players with positions, teams, projected stats. Source for dropdowns. |
| **Draft Board** | All 161 picks in snake order. Your picks highlighted gold. Dropdowns in Column D. |
| **Owner Intel** | Quick-reference scouting report on all 7 owners. |
| **Team_Bubs** | Bubs's roster tracker |
| **Team_Furman** | Furman's roster tracker |
| **Team_Quickster** | YOUR roster tracker (highlighted) |
| **Team_Cone** | Cone's roster tracker |
| **Team_Vic** | Vic's roster tracker |
| **Team_TK** | TK's roster tracker |
| **Team_Rich** | Rich's roster tracker |
| **Keepers** | Place to log 2026 keeper announcements |
| **Non-Keepers** | 63 players who cannot be kept |

## 2. RedDevils2026Draft_v2.html
**Interactive dashboard with:**
- Live Intel box (who's on clock, predicted behavior)
- Roto standings table with color-coded rankings
- Owner Intel tab with scouting cards
- Strategy tab with "Will He Be There?" calculator
- Tier cliff alerts
- Charts (hitting points, pitching points)
- Your team panel with position needs

## 3. RedDevils_OwnerProfiles.md
**Detailed scouting report with:**
- 8 years of draft history analysis (2018-2025)
- Round-by-round tendencies for each owner
- "Their Guy" alerts
- Closer run predictions
- Championship history

---

# LEAGUE STRUCTURE <a name="league-structure"></a>

## Teams (7)
| Owner | 2026 Team Name | Championships |
|-------|----------------|---------------|
| Bubs | Missing in Action | 🏆 2019 |
| Furman (Tom) | FLY TO VICTORY | None |
| **Quickster (You)** | **Predictive Swamp Rabbits** | **🏆🏆 2020, 2021** |
| Cone (Holm) | LITTLE timmy'S TEAM | 🏆🏆 2023, 2024 |
| Vic (Tommy) | FAFO | 🏆🏆 2017, 2018 |
| TK | Cool Breezy | 🏆🏆🏆 2015, 2016, 2022 |
| Rich | Filthy Rich Boiler | 🏆 2025 |

## Roster (25 spots)
**Hitters (14):**
- C, 1B, 1B, 2B, 2B, 3B, SS, MI, CI, OF, OF, OF, OF, OF

**Pitchers (9):**
- SP, SP, SP, SP, SP, SP, RP, RP, RP

**Reserves (2):**
- UT, UT

## Scoring (8 Categories - Roto)
**Hitting:** BA, HR, R, RBI
**Pitching:** W, SV, ERA, WHIP

Each category ranked 1-7 (7 = best, 1 = worst)
Maximum possible points: 56

## Keeper Rules
- 2 keepers per team
- Must have been drafted Round 7 or later in 2025
- OR acquired as free agent during 2025 season
- Previous year's keepers cannot be kept again

## Financials
- Buy-in: $100 + $25 fees
- 1st Place: $303
- 2nd Place: $137
- 3rd Place: $110
- Category Winners: $15 each (8 categories)

---

# DRAFT ORDER <a name="draft-order"></a>

## Snake Draft Format
- 7 teams, 23 rounds (25 total minus 2 keepers each)
- 161 total picks

## 2026 Draft Order
| Pick | Owner |
|------|-------|
| 1 | Bubs |
| 2 | Furman |
| **3** | **Quickster (YOU)** |
| 4 | Cone |
| 5 | Vic |
| 6 | TK |
| 7 | Rich |

## Your Picks (Snake Format)
| Round | Overall Pick | Notes |
|-------|--------------|-------|
| 1 | 3 | Early - elite player |
| 2 | 12 | Late - 9 picks between |
| 3 | 17 | Early |
| 4 | 26 | Late |
| 5 | 31 | Early |
| ... | ... | Pattern continues |

---

# OWNER SCOUTING PROFILES <a name="owner-profiles"></a>

## BUBS (Pick #1)
**Threat Level:** 🟢 Low
**Championships:** 🏆 2019
**Key Patterns:**
- Takes elite OF in Round 1 (6 of 7 years)
- VERY late on closers (average: Round 14)
- Conservative drafter - follows rankings
- Will NOT start a closer run

**Prediction:** Will take Ohtani or best available OF at #1

---

## FURMAN (Pick #2)
**Threat Level:** 🟡 Medium
**Championships:** None (HUNGRY)
**Key Patterns:**
- Zero titles in 8 years - desperate to win
- Takes best hitter available (position agnostic)
- Gets closers earlier than most (Round 6)
- Loves veteran aces (drafted Verlander 3x)

**Prediction:** Might reach for "his guys" - unpredictable

---

## CONE (Pick #4)
**Threat Level:** 🔴 HIGH
**Championships:** 🏆🏆 2023, 2024 (BACK-TO-BACK)
**Key Patterns:**
- Takes OF Round 1 EVERY year (7 for 7)
- Balanced approach - hard to exploit
- Getting earlier on closers (R12 → R7 trend)
- Knows how to win

**Prediction:** Best available OF, or pivot to ace SP if picking late

---

## VIC (Pick #5)
**Threat Level:** 🟡 Medium
**Championships:** 🏆🏆 2017, 2018
**Key Patterns:**
- Identity crisis: was SP-first for 4 years, now taking hitters
- Unpredictable on closers (anywhere from R7 to R20)
- "FAFO" team name suggests aggressive mood
- Jose Ramirez obsession (drafted him 2 straight years)

**Prediction:** Wild card - could go SP or premium IF

---

## TK (Pick #6)
**Threat Level:** 🔴 HIGH
**Championships:** 🏆🏆🏆 2015, 2016, 2022 (MOST TITLES)
**Key Patterns:**
- Best player available - any position
- Won't panic during runs
- Mid-round closer timing (R6-12)
- Kyle Schwarber obsession (drafted him 5 TIMES)

**Prediction:** Impossible to predict - BPA approach

---

## RICH (Pick #7)
**Threat Level:** 🟡 Medium
**Championships:** 🏆 2025 (DEFENDING CHAMP)
**Key Patterns:**
- Late Round 1 specialist (picked 5th+ in 6 of 7 years)
- Hitter-first mentality
- Wild on closers (anywhere from R4 to R18)
- Raisel Iglesias favorite (drafted twice)

**Prediction:** Best available hitter at #7

---

## CLOSER RUN PREDICTIONS

**Will START a run (Round 6-7):**
- Cone (trending earlier)
- Furman (consistent R6 guy)

**Might JOIN a run:**
- Vic (unpredictable)
- Rich (variable timing)

**Will IGNORE the run:**
- Bubs (waits until R14+)
- TK (experienced, won't panic)

---

# GOOGLE SHEETS SETUP <a name="google-sheets-setup"></a>

## Step 1: Upload to Google Drive
1. Go to drive.google.com
2. Click "New" → "File Upload"
3. Select `RedDevils2026_DraftTracker.xlsx`
4. Wait for upload to complete

## Step 2: Convert to Google Sheets
1. Right-click the uploaded file
2. Select "Open with" → "Google Sheets"
3. It will create a Google Sheets copy
4. Rename it: `RedDevils2026_DraftTracker`

## Step 3: Test the Dropdowns
1. Go to "Draft Board" tab
2. Click any cell in Column D (Player column)
3. You should see a dropdown arrow
4. Click it - player list appears
5. Start typing to filter
6. If player not in list, just type manually (it allows this)

## Step 4: Publish to Web (For HTML Connection)
1. File → Share → Publish to web
2. Under "Link", choose:
   - "Entire Document" OR specific sheets
   - Format: "Web page" or "CSV"
3. Click "Publish"
4. Copy the link - you'll give this to Claude for the HTML

---

# HTML DASHBOARD CONNECTION <a name="html-connection"></a>

## How It Works

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│  Google Sheet   │────▶│  Published URL  │────▶│  HTML Dashboard │
│  (You update)   │     │  (Auto-updates) │     │  (Reads & shows)│
└─────────────────┘     └─────────────────┘     └─────────────────┘
```

1. **You update** the Google Sheet (click dropdown, select player)
2. **Google publishes** the data to a public URL automatically
3. **HTML file** fetches data from that URL using JavaScript
4. **Charts & standings** update based on the live data
5. **You refresh** the HTML page to see updates

## What Claude Will Build
An HTML file with JavaScript that:
- Fetches your Google Sheet data via the published URL
- Parses the pick data
- Calculates roto standings automatically
- Updates charts and rosters
- All happens in YOUR browser - no server needed

## The Flow During Draft
1. Pick happens → You update Google Sheet (2 seconds)
2. You refresh HTML dashboard → See updated visuals
3. Your turn → Ask Claude "Who should I pick?"
4. Claude fetches the Google Sheet, analyzes, gives 3 recommendations
5. You decide → Log it → Continue

---

# DRAFT DAY WORKFLOW <a name="draft-day-workflow"></a>

## Setup (Before Draft)
- [ ] Google Sheet open in one browser tab
- [ ] HTML Dashboard open in another tab
- [ ] Claude conversation open (this chat or new one)
- [ ] CBS draft room open for official picks

## During Draft
1. **Someone picks** → You type/select in Google Sheet
2. **Every few picks** → Refresh HTML to see updated standings
3. **Your turn** → Ask Claude: "It's my turn, pick #X, who should I take?"
4. **Claude analyzes** → Gives 3 recommendations with reasoning
5. **You decide** → Make pick in CBS → Log in Google Sheet
6. **Continue** → Repeat until draft ends

## Post-Draft
- Claude generates final recap
- Review roster, category projections
- Plan waiver wire targets

---

# STRATEGIC TOOLS BUILT <a name="strategic-tools"></a>

## 1. "Will He Be There?" Analysis
Predicts probability a player survives to your next pick based on:
- How many picks until your turn
- Who's picking before you
- Their historical tendencies

## 2. Closer Run Tracker
Shows who will start/join/ignore closer runs based on 8 years of behavior.

## 3. Tier Cliff Alerts
Warns when position quality is about to drop off:
- Catcher cliff after Rutschman/Contreras
- Closer cliff after top 5
- Position depth analysis

## 4. Punt Strategy Calculator
Math on whether punting saves could work:
- Lose 7 points (guaranteed last)
- But gain picks for better bats/arms
- Net gain if you dominate 5+ other categories

## 5. Owner "Their Guy" Alerts
Players each owner drafts repeatedly:
- TK → Kyle Schwarber (5x)
- Furman → Veteran aces
- Vic → Jose Ramirez
- Rich → Raisel Iglesias

---

# WHAT'S STILL NEEDED <a name="whats-needed"></a>

## Before Draft Day

### 1. Keeper Announcements
- [ ] Collect 2026 keeper selections from all 7 teams
- [ ] Update Keepers tab in Google Sheet
- [ ] Remove keepers from available player pool

### 2. 2026 Projections (Late February)
- [ ] Download Steamer/ZiPS/ATC projections
- [ ] Update Players tab with real projected stats
- [ ] Expand player list to 500+

### 3. HTML Dashboard Connector
- [ ] You publish Google Sheet to web
- [ ] Claude builds HTML that reads from published URL
- [ ] Test the live connection

### 4. Final Player List
- [ ] Add top 150 prospects
- [ ] Add fringe players who might get drafted late
- [ ] Add "MANUAL ENTRY" rows for unknowns

## Optional Enhancements
- [ ] Spring training injury tracker
- [ ] Statcast sleeper flags (high EV, low BABIP)
- [ ] Historical opponent draft patterns visualization

---

# QUICK REFERENCE

## Your 2025 Keeper Candidates (Round 7+)
| Round | Player | Position |
|-------|--------|----------|
| 7 | Devin Williams | RP |
| 8 | Christian Walker | 1B |
| 9 | Tyler Glasnow | SP |
| 10 | Lawrence Butler | OF |
| 11 | Max Fried | SP |
| 12 | George Kirby | SP |
| 13 | Riley Greene | OF |
| 14 | Hunter Greene | SP |
| 15 | Hunter Brown | SP |
| 16 | Vinnie Pasquantino | 1B |
| 17 | Ryan Walker | RP |
| 18 | Matt Chapman | 3B |
| 19 | Steven Kwan | OF |
| 20 | Jordan Romano | RP |
| 21 | Ian Happ | OF |

## Your 2025 Non-Keepers (Can't Keep)
Elly De La Cruz, Tucker, Harper, Devers, Albies, Rutschman, Devin Williams, O'Cruz, Skenes

## Key Dates
- **Late February:** Projections released, final prep
- **Week before draft:** Test run with Claude
- **March 14, 2026:** DRAFT DAY @ 12:00 PM Central

---

# CONTACT / NOTES

**League Commissioner:** Tom Furmankiewicz
**Draft Location:** The Farm
**Your Team:** Predictive Swamp Rabbits
**Your Titles:** 🏆 2020, 🏆 2021

---

*Documentation created by Claude • February 2026*
