# The Compound Click — Facilitator Guide

A 30-minute, laptop-based Scratch session for women in tech, 40+, with no prior coding experience. Participants leave having built a working programme: a clickable "savings" simulator that grows a number, plays a sound and animates — the same event → logic → feedback pattern behind every banking app and trading screen.

Companion participant website: `index.html` (open in any browser, works on shared/locked-down school or venue machines, no install needed beyond Scratch itself).

**Nothing to prepare or upload.** Every sprite, backdrop and sound used in this build comes from Scratch's own free built-in library — there are no custom assets, files, or accounts to set up beforehand. Open Scratch on the day and go.

---

## Learning objective

By the end, every participant will have:
1. Built and run a working Scratch programme from scratch (pun intended)
2. Used a variable, an event block, and a sound/animation response
3. Heard, explicitly, how each block maps to something a junior developer in fintech does on day one

The goal is not "learn to code" — it's "prove to yourself in 30 minutes that you *can*."

---

## Before the day

- [ ] Confirm venue wifi can handle everyone hitting scratch.mit.edu at once — test with 2–3 devices beforehand if possible
- [ ] **Fallback:** install the [Scratch offline editor](https://scratch.mit.edu/download) on your own facilitator laptop in case wifi fails, and know how to talk people through installing it from a USB stick if needed
- [ ] Scratch accounts are **not required** — "See inside" / offline editor works anonymously, projects just won't autosave. Mention this up front so nobody panics about losing work; 30 minutes doesn't leave room for account creation anyway
- [ ] Test that laptop speakers/headphone jacks work — the sound block is part of the "wow" moment
- [ ] Open `index.html` on the projector/screen you'll present from
- [ ] Print 3–4 copies of the step list (Appendix A below) as a backup if any laptop or the projector fails
- [ ] Know your room's power situation — 30 minutes is short, but if laptops arrive at 20%, they may die mid-session

## What each participant needs

- A laptop with a modern browser (Chrome/Edge/Firefox)
- Internet access (or the offline editor pre-installed)
- Headphones optional but nice for the sound step

The participant website has an **Open Scratch** button in the hero (linked to `https://scratch.mit.edu/projects/editor/`, opens in a new tab) that drops straight into a blank project — no homepage-browsing or account needed. Worth pointing people to it explicitly at 0:00 rather than assuming everyone finds Scratch on their own.

---

## Timetable

| Time | Duration | Segment | What's happening |
|---|---|---|---|
| 0:00–0:03 | 3 min | Welcome & framing | Why this exercise, why it maps to real tech/finance careers |
| 0:03–0:07 | 4 min | Meet Scratch | Live demo tour: stage, sprite list, block palette, scripts area, green flag |
| 0:07–0:10 | 3 min | Step 1 — Clear the stage | Delete the cat, add the Crystal sprite, pick a backdrop |
| 0:10–0:15 | 5 min | Step 2 & 3 — Give it a memory | Create the `Savings` variable, build the green-flag reset script, add a dedicated key-press reset, test both |
| 0:15–0:22 | 7 min | Step 4 — Make it respond | The main build: click → add money → sound → pulse animation. This is where most support is needed |
| 0:22–0:26 | 4 min | Step 5 — Make it yours | Personalise backdrop, costume, click amount |
| 0:26–0:28 | 2 min | Step 6 — Stretch goal (flexible) | Milestone message when savings pass 100. **This is your buffer** — skip or shorten if the room is behind |
| 0:28–0:30 | 2 min | Wrap-up | Career connection, what to try next, close |

Step 6 is deliberately the release valve: if the room needed longer on Step 4 (it usually does), spend the time there instead and treat the wrap-up conversation as covering the milestone idea verbally rather than building it.

---

## Segment-by-segment script

### 0:00–0:03 — Welcome & framing
Open with the "why," not the "how." Something like:

> "In the next 30 minutes, every one of you is going to build a working piece of software. Not a toy — the actual pattern that runs inside banking apps, trading platforms, and every fintech product you've ever tapped a button on: something happens (you click), the system does something (it updates a number), and it tells you it happened (a sound, an animation). That's it. That's the job. Today you write it yourself."

Address the room directly: most people here have never written a line of code, and that's exactly who this is for. No prior experience needed, no "tech brain" required.

### 0:03–0:07 — Meet Scratch
Project your own screen. Point out, briefly:
- **Stage** (top left) — where the programme runs
- **Sprite list** (bottom right, below the stage) — the "characters" or objects in the programme
- **Block palette** (middle) — the vocabulary; colour-coded by category
- **Scripts area** (right) — where you snap blocks together like puzzle pieces
- **Green flag / red stop** (top right) — run and stop the programme

Don't dwell — this is orientation, not a lecture. They'll learn the interface by using it in the next steps.

### 0:07–0:10 — Step 1: Clear the stage
Walk the room through deleting the cat sprite and adding the **Crystal** sprite from the library (the "Choose a Sprite" button sits below the stage, on the right of the screen — search "crystal" if it isn't visible straight away), then picking any backdrop. This is a good moment to circulate and check everyone's laptop actually opened Scratch correctly before the real building starts.

### 0:10–0:15 — Steps 2–3: Give it a memory
Creating the variable is the first slightly fiddly bit (Variables category → "Make a Variable"). Expect a few people to need a hand finding the button.

There are two reset scripts to build here, not one: the green-flag reset from before, plus a dedicated `when key r pressed` reset. Flag why explicitly — the green flag is a shared button that also restarts everything else in the programme, so a reset that's just a reset (and nothing else) is worth having on its own trigger. Once both are built, get everyone to test both together — click the green flag, then press R — a small synchronised "does it work" moment builds confidence before the harder step.

### 0:15–0:22 — Step 4: Make it respond (the main build)
This is the longest block of time for a reason — it's the step with the most new concepts (event block, change vs. set, sound, two "change size" blocks for the pulse). Let people work at their own pace; this is where you and any co-facilitators should be circulating most.

Expect someone to ask why the `wait 0.1 seconds` block is there between the two size changes. Good question, worth having the answer ready: without it, the grow and shrink happen back to back so fast that Scratch never actually renders the bigger size on screen — the pulse would be invisible. The tiny pause is what makes the animation something the eye can actually catch.

If someone finishes early, that's what Step 6 is for — point them ahead rather than having them wait.

### 0:22–0:26 — Step 5: Personalise
Low-pressure and mostly self-directed: change the backdrop, swap the costume, change the click amount from 10 to something else. This step exists partly for pacing (it absorbs variance in how fast people finished Step 4) and partly because ownership of the output matters — "my programme," not "the programme."

### 0:26–0:28 — Step 6: Stretch goal / buffer
Only introduce this if the room is broadly on schedule. If you're behind, skip straight to wrap-up — better to finish with everyone confident in a working Step 4 build than rushed and confused by Step 6.

### 0:28–0:30 — Wrap-up
Close by naming the transfer explicitly:

> "What you just built — a trigger, a stored value, and a response — is the core loop of software engineering. Every fintech app, every trading dashboard, every banking system is thousands of versions of what's on your screen right now. You already did the hard part: you proved to yourself you can pick this up."

Point to where they can go next (see Appendix C).

---

## Common issues & quick fixes

| Problem | Fix |
|---|---|
| Accidentally deleted the wrong sprite | Right-click stage → nothing to undo in Scratch easily; just re-add the Crystal sprite from the library, no harm done |
| Can't find "Make a Variable" | It's a button inside the **Variables** category in the block palette, above the variable blocks themselves |
| Clicking the crystal does nothing | Almost always the "when this sprite clicked" hat block isn't at the top of the stack, or blocks aren't snapped together — check for a gap |
| No sound plays | Check system/laptop volume first; then check the sprite has a sound assigned in the Sounds tab |
| Variable not visible on stage | The checkbox next to the variable name in the palette needs to be ticked |
| Pressing R doesn't reset it | The key-press block defaults to "space" — check its dropdown was actually changed to "r" |
| Participant is ahead of the group | Point them to Step 6 or suggest they help a neighbour — both are fine outcomes |
| Participant is behind | Don't stop the room for one person — flag a helper (you or a co-facilitator) to sit with them while the group moves on |

---

## Scaffolding — support for anyone who's stuck

Some participants will hit Step 4 (the six-block build) and stall. That's expected — it's the step with the most new ideas at once. Three tools for this, roughly in order of how much intervention they need:

**1. The buddy system.** Seat people in loose pairs from the start, ideally mixing anyone who mentions prior tech exposure with anyone who's more nervous. Frame it once, early: "If you finish a step, the fastest way to help is to turn to your neighbour before waving me over — I'll always come, but you'll get unstuck faster with someone right next to you." This also takes pressure off you as the only source of help in the room.

**2. The core-4 fallback.** If someone is visibly behind by the time the room reaches Step 5, give them permission to drop to a minimal version rather than rushing the full six-block build:

```
when this sprite clicked
change Savings by 10
```

That's it — two blocks. It's still a real, working, testable programme: click the crystal, watch the number go up. Say this explicitly: *"That's a complete build. The sound and the wobble are polish, not the point — you've already written the part that matters."* People who came in anxious about "not being technical" need to hear that a small working thing counts as a win, not a shortfall. They can add the sound and animation back in during Step 5's personalise time if they want to, with no pressure to.

**3. Narrate the fix, don't just make it.** When you sit with someone, resist doing the click-and-drag for them. Point at the gap between two blocks, or name the block they're missing ("you need one more block from the Sound category") and let them place it. The 30-minute win is "I did this," not "it got done."

**Language that helps, generally:** avoid "it's easy" — for someone who's never done this, it isn't, and being told it is makes struggling feel like personal failure. Better: "this is the fiddliest step in the whole thing, everyone slows down here," which is true and normalises it.

## Extension activities — for anyone who finishes early

Don't let fast finishers sit idle waiting for the room — and don't force everyone through the same stretch goal at the same pace. Offer these as a menu once someone's done with Step 5, in roughly this order of difficulty. All of them build on blocks already introduced, so there's no new interface to explain — just point them at the relevant block category.

| Extension | What it adds | Blocks/concepts used |
|---|---|---|
| **Real returns** | Swap the fixed `change Savings by 10` for `change Savings by (pick random 5 to 15)` — no two clicks pay out the same, like an actual investment | Operators: `pick random` |
| **Real compound interest** | Add a second script: `forever` → `wait 2 seconds` → `change Savings by (Savings × 0.01)` — Savings now grows on its own, 1% at a time, exactly like the project's name promises | Control: `forever`, `wait`; Operators: multiply |
| **A second sprite: expenses** | Add a new sprite that *subtracts* from Savings when clicked — now there's income and outgoings, a first taste of a real budget | Everything from Step 4, applied to a new sprite |
| **Milestone upgrade** | Extend Step 6: when Savings crosses your threshold, also broadcast a message that swaps the backdrop and plays a fanfare sound, not just a text bubble | Events: `broadcast` / `when I receive`; Looks: `switch backdrop` |

If someone races through all four, the honest answer is "you've now covered variables, events, randomness, loops and messaging — that's most of what a first-term programming course covers." That's worth telling them.



---

## Appendix A: printable step list (backup handout)

1. Delete the cat. Click **Choose a Sprite** (below the stage, on the right) and add the **Crystal** sprite. Pick a backdrop.
2. Variables → **Make a Variable** → name it `Savings`.
3. Drag: `when green flag clicked` + `set Savings to 0`. Click the green flag to test.
4. Drag a second reset: `when key r pressed` + `set Savings to 0`. Press R to test.
5. Drag: `when this sprite clicked` + `change Savings by 10` + `play sound` (pick whatever sound is already on your sprite, in the Sounds tab — or add any short one from the sound library) + `change size by 10` + `wait 0.1 seconds` + `change size by -10`. Click the crystal to test.
6. Personalise: change the backdrop, the costume, or the click amount.
7. *(Stretch)* Add: `if Savings > 100 then` → `say "You just built your first fintech feature!"`.

## Appendix B: the "why this maps to a career" cheat sheet

Use these if you want a quick line while circulating and someone asks "does this actually relate to real jobs?":

- **Sprites & costumes** → UI components — the buttons and screens in every app
- **Variables** → exactly what a database field or app "state" is — your bank balance is a variable somewhere
- **Event blocks** (`when clicked`) → every button in every app you use is wired to an event handler like this
- **Sound/animation feedback** → this is UX design — telling the user something happened
- **If-blocks** (Step 6) → business logic — the rules that decide interest, fraud flags, eligibility

## Appendix C: where to go next

Suggested close-out line and links to have ready: scratch.mit.edu to keep experimenting (free), and — if the event has a call-to-action (a course, a mentoring scheme, a follow-up meetup) — that's the natural place to point people who want to keep going.
