# Ship First, Optimize Later Protocol

**Status:** ⬜ Initializing | ⬜ Day 1 Active | ⬜ Day 2 Active | ⬜ Shipped  
**AI Collaboration Mode:** Fast scaffold / No premature optimization  
**Hardware Firewall:** 🔒 LOCKED (30-day cooldown active)

---

## The Prime Directive
Working code in 48 hours. Architecture can wait. Feedback cannot.

---

## Phase 0: Hardware Firewall (Do This First)

- [ ] Create `HARDWARE_BACKLOG.md` 
- [ ] Write down the shiny hardware you want to buy: _______________
- [ ] Close all shopping tabs. Lock the file. Code with what you have.
- [ ] Set calendar reminder for: _______________ (30 days from now)

**Rule:** If a hardware thought arises during coding, append to `HARDWARE_BACKLOG.md` and immediately return to implementation.

---

## Phase 1: The 48-Hour Scaffold

### Day 1 (Hours 0-4): Ugly Truth

- [ ] `git init` + GitHub push with README describing **user outcome**, not tech stack
- [ ] Choose "boring" stack: _______________ (the one you know, not the trendy one)
- [ ] Write the ugliest version that demonstrates core interaction
- [ ] **Explicitly skip:** Docker, CI/CD, linting, cloud config, database setup

**TODAY.md entry:** (One sentence. What must work before sleep?)  
`________________________________________________________________`

### Day 2 (Hours 4-48): Stranger-Ready

- [ ] `requirements.txt` or equivalent install script
- [ ] README includes: install steps, run command, expected output
- [ ] Add one "sticky" mechanic (see checklist below)
- [ ] Tag `v0.1-demo`
- [ ] Share with one human (or AI evaluator) and watch them use it

---

## Sticky Programs Checklist

Before writing code, validate this solves 2+ criteria:

- [ ] **Instant feedback:** User sees result in &lt;3 seconds (no batch processing)
- [ ] **Progressive disclosure:** Simple entry, depth emerges (Vim, not Excel)
- [ ] **Friction removal:** Eliminates 2+ clicks from existing workflow
- [ ] **Social resonance:** Output is shareable/visible (generates FOMO)
- [ ] **Daily utility:** Solves something annoying **today**, not theoretically

**This PRD hits:** #____ and #____

---

## Repository Discipline

**Required Structure:**

    repo/
    ├── TODAY.md              # Current single objective
    ├── HACKS.md              # Acknowledged tech debt (prevents rabbit holes)
    ├── DEMO_GIF.gif          # Visual proof (create before polishing code)
    ├── HARDWARE_BACKLOG.md   # The parking lot
    └── AI_CONTEXT.md         # (Optional) Persistent context for AI collaborators

### Commit Message Rules (Strict)

Every commit must be:
- (a) User-visible feature, OR
- (b) Bug fix blocking usage

**Forbidden until v0.5:** "refactor", "cleanup", "optimize", "wip", "temp"

---

## AI Collaboration Guidelines

### Context Management

- Keep `TODAY.md` updated with current blockers—AI reads this first
- When context window gets tight, summarize to: What works / What's broken / Next 3 steps
- No architecture debates with AI during Days 1-2. Implementation only.

### Prompt Templates for This Phase

**Stuck on implementation:** "Implement the ugliest working version of [feature]. Optimize nothing. Just make it return the correct result."

**Scope creep detected:** "Given our 48-hour deadline, which of these features is critical for v0.1-demo vs. can wait?"

**Hardware temptation:** "I want to add [complex infrastructure]. Convince me why this should go in HARDWARE_BACKLOG.md instead of today's code."

---

## Weekly Rhythm

| Day | Action | Success Metric |
|-----|--------|----------------|
| **Monday** | New repo, ugly prototype | `TODAY.md` objective met by EOD |
| **Wednesday** | User test (self or other) | 3 friction points documented |
| **Friday** | Ship vs. Kill decision | README + screenshot posted, OR repo archived with post-mortem |

**Ship:** Polish README, add DEMO_GIF, announce.  
**Kill:** Archive, write 3-sentence post-mortem, migrate hardware ideas to global backlog.

---

## Anti-Distraction Default Stack

When in doubt, use this:

- **Language:** Python (fastest idea-to-runnable)
- **UI:** Terminal → Gradio/Streamlit (no frontend frameworks until v2)
- **Storage:** SQLite or JSON (no DB setup until 100+ users)
- **Hosting:** Localhost only. Share screen recordings, not deployed URLs.

---

## Success Metrics

- [ ] Repo has visible commits within 2 hours of initialization
- [ ] v0.1-demo tag exists within 48 hours
- [ ] HARDWARE_BACKLOG.md has entries (proves you're resisting temptation)
- [ ] One stranger has run the code successfully

**The Only Metric That Matters:** Number of repositories with working demos.  
**Target:** One shippable repo every 2 weeks minimum.

---

## Emergency Protocols

**Feeling the urge to research hardware:**  
Open `HARDWARE_BACKLOG.md`, write it down, close laptop for 5 minutes, return to code.

**Caught in architecture paralysis:**  
Ask: "What would this look like if it were easy?" Implement that. Document the "proper" way in `HACKS.md` for later.

**AI suggesting complex solutions:**  
Reply: "Simpler. Assume I have no GPU, no cloud budget, and 4 hours left."

---

*Protocol activated: _______________  
Next checkpoint: _______________  
Current blocker: _______________*
