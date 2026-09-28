# The Compound Click — Facilitator Guide

A 30-minute, laptop-based Scratch session for women in tech, 40+, with no prior coding experience. Participants leave having built a working programme: a clickable "savings" simulator that grows a number, plays a sound and gives a brief colour flash — the same event → logic → feedback pattern behind every banking app and trading screen.

Companion participant website: `index.html` (open in any browser, works on shared/locked-down school or venue machines, no install needed beyond Scratch itself).

**Nothing to prepare or upload.** Every sprite, backdrop and sound used in this build comes from Scratch's own free built-in library — there are no custom assets, files, or accounts to set up beforehand. Open Scratch on the day and go.

---

## Learning objective

By the end, every participant will have:
1. Built and run a working Scratch programme from scratch (pun intended)
2. Used a variable, an event block, and a sound/animation response
3. Heard, explicitly, how each block maps to something a junior developer in fintech does on day one

The goal is not "learn to code" — it's "prove to yourself in 30 minutes that you *can*."

## Session structure: PRIMM

The session opens with a short group demo before anyone touches their own laptop, structured around **PRIMM** — Predict, Run, Investigate, Modify, Make — a method for teaching complete beginners to programme, developed specifically because reading code (or blocks) cold and jumping straight to writing it is a big first ask. PRIMM breaks that jump into smaller ones:

- **Predict** — look at a tiny, unrun example and guess what it'll do, before finding out
- **Run** — watch it run, check the guess
- **Investigate** — name what each part is actually doing
- **Modify** — change one small thing and see the effect, so "editing code" stops feeling fragile
- **Make** — build your own, from scratch — this is the rest of the session (Steps 1–6)

Practically: Predict, Run and Investigate happen together, on your screen, with laptops closed — about 4 minutes. Then everyone opens their own laptop and rebuilds the exact same tiny example themselves (that's Modify, done hands-on rather than called out from their seat) — about 4 more minutes. Only then do laptops reset and Step 1 begins. This matters most for participants with zero prior exposure to any of this — by the time they build their own event-and-response script in Step 4, they've watched the pattern once, built it once already with their own hands on something trivial, and named its parts out loud. It costs eight minutes up front and should save more than that back in Step 4, where the same underlying pattern (event block on top, action underneath) shows up again — now something they've physically done before, not just watched.

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

The participant website has an **Open Scratch** button in the hero (linked to `https://scratch.mit.edu/projects/editor/`, opens in a new tab) that drops straight into a blank project — no homepage-browsing or account needed. Worth pointing people to it explicitly once the facilitator's watch-only demo ends (around 0:06, right before everyone rebuilds it themselves), rather than assuming everyone finds Scratch on their own — and worth asking laptops to stay closed or untouched before then, so the demo actually gets everyone's attention rather than competing with people already exploring on their own.

## About the participant website

A few things worth knowing before the day:

- **No on-page timer.** The site doesn't run a countdown or clock — that turned out to feel more like pressure than pacing for a room of first-timers. Keep time against this guide's timetable instead; each step still shows its own suggested duration on the site as a light badge, with no ticking clock attached.
- **Progress isn't saved between visits.** The step checkboxes track progress only for as long as the page stays open — closing the tab or reloading clears everything automatically. Nothing is written to the laptop's storage, so there's nothing left behind for the next person to use that machine.
- **"Reset progress" button.** If you want to clear a laptop's checkboxes without reloading — for instance, handing a laptop to a second participant later the same day — there's a small "Reset progress" link under the progress bar (in the side rail on desktop, and just under the top bar on mobile/narrow screens).
- **Certificate and trophy.** After Step 6 / the extension menu, the site shows a small trophy graphic and a printable certificate: participants type their name into a field, the date fills in automatically, and a "Print certificate" button prints just the certificate (not the rest of the page). Worth mentioning around the 0:28 mark so nobody skips past it.

---

## Timetable

| Time | Duration | Segment | What's happening |
|---|---|---|---|
| 0:00–0:02 | 2 min | Welcome & framing | Why this exercise, why it maps to real tech/finance careers |
| 0:02–0:06 | 4 min | Facilitator demo (watch) | Predict → Run → Investigate, on your screen, laptops closed |
| 0:06–0:10 | 4 min | Everyone rebuilds it (try) | Same two blocks, on their own laptop, then tweak one thing (Modify) |
| 0:10–0:13 | 3 min | Step 1 — Clear the stage | Delete the cat (this is also the demo's reset), add the Crystal sprite, pick a backdrop |
| 0:13–0:18 | 5 min | Step 2 & 3 — Give it a memory | Create the `Savings` variable, build the green-flag reset script, add a dedicated key-press reset, test both |
| 0:18–0:25 | 7 min | Step 4 — Make it respond | The main build: click → add money → sound → colour flash. This is where most support is needed |
| 0:25–0:27 | 2 min | Step 5 — Make it yours | Personalise backdrop, costume, click amount |
| 0:27–0:28 | 1 min | Step 6 — Stretch goal (flexible) | Milestone message when savings pass 100. **This is your buffer** — skip entirely if the room is behind |
| 0:28–0:30 | 2 min | Wrap-up | Career connection, what to try next, close |

Step 6 is deliberately the release valve: if the room needed longer on Step 4 (it usually does), spend the time there instead and treat the wrap-up conversation as covering the milestone idea verbally rather than building it. The demo (watch + try it) is the firmest minute count in the whole session — it's two fixed group activities, not self-paced, so it's the one place a facilitator running long should actively cut rather than let drift (see script below for what to cut first). If it does overrun, take the time from Step 5, not Step 4 — personalising is the most compressible part of the session; the core build isn't.

---

## Segment-by-segment script

### 0:00–0:02 — Welcome & framing
Open with the "why," not the "how." Something like:

> "In the next 30 minutes, every one of you is going to build a working piece of software. Not a toy — the actual pattern that runs inside banking apps, trading platforms, and every fintech product you've ever tapped a button on: something happens (you click), the system does something (it updates a number), and it tells you it happened (a sound, an animation). That's it. That's the job. Today you write it yourself."

Address the room directly: most people here have never written a line of code, and that's exactly who this is for. No prior experience needed, no "tech brain" required. Worth naming three things explicitly, right at the start:
- If a mouse, trackpad, or right-clicking feels unfamiliar, that's completely normal — nobody's starting behind. You'll get used to it in the first few minutes, because that's what Step 1 is for.
- You don't need to finish every step to leave with something real — even the smallest working version, one click that changes a number, is a complete piece of software. Everything after that is a bonus.
- If you've ever built a spreadsheet formula — a running total, an IF statement, anything that updates itself — you already have more of the underlying logic than you think, and you'll recognise it as you go. If spreadsheets aren't your thing either, that's completely fine too — nothing here depends on it.

### 0:02–0:06 — Facilitator demo: watch (Predict → Run → Investigate)
Everyone watches your screen; laptops stay closed or untouched. Open a completely fresh Scratch project (the default cat sprite is fine — you need nothing pre-built) and, without running it yet, drag in two blocks: **when this sprite clicked**, then **say "Hello!" for 2 seconds** underneath it.

**Predict (1 min).** Point at the two blocks, not yet run. Ask: "What do you think happens when I click the cat?" Take two or three guesses out loud — there's no wrong answer, the point is just having a guess in mind before you find out.

**Run (1 min).** Click the cat. Let the speech bubble show. Ask whether it matched what people guessed.

**Investigate (2 min).** Name what each block actually did, briefly:
- The top block (gold) is an **event** — it's listening for something to happen. Here, a click.
- The bottom block (purple) is the **action** — what happens in response.
- Point out the colour-coding in the block palette while you're here — it's not decorative, it groups blocks by what kind of job they do, and they'll be reading it all session.

Name the pattern explicitly: "Trigger, then response. Every single thing you build for the rest of today is a bigger version of exactly this." Then hand off: "Now you're going to build this exact thing yourselves — on your own laptop, on the same cat, nothing to add or delete yet."

### 0:06–0:10 — Everyone rebuilds it (Modify, hands-on)
Have everyone open their own laptop and go to the participant site — the **Open Scratch** button drops straight into a blank project with the same default cat sprite you just used. Ask everyone to build the identical two-block script: **when this sprite clicked** + **say "Hello!" for 2 seconds**, and click their own cat to test it.

Once most of the room has it working (a quick show of hands is enough — don't wait for everyone), give the Modify instruction: "Now change one thing — the message, or how long it shows for — and test it again. Make it something daft if you want, this one doesn't count for anything." This is deliberately unsupervised and low-stakes; there's nothing to get wrong here, which is exactly why it's a safe place to practise the physical mechanics (dragging, snapping, clicking to test) before those same mechanics matter in the real build. Inviting something silly here is worth doing on purpose, not just tolerating — a laugh at minute 8 does more for a nervous room than another reassurance would, and it costs nothing since this whole script gets deleted in a minute anyway.

Circulate during this — it's your best early signal for who's confident with the mouse/trackpad and who's going to need more attention in Step 1. Don't fix anyone's blocks for them here; point, and let them place it (see the "narrate the fix" principle in Scaffolding below — it starts applying from this moment, not just Step 4).

Close with the reset, explicitly: "Now we reset — right-click your cat and delete it. That's Step 1's first job anyway, so nothing here was wasted, it was just practice."

### 0:10–0:13 — Step 1: Clear the stage
Walk the room through deleting the cat sprite (the one they just practised on) and adding the **Crystal** sprite from the library (the "Choose a Sprite" button sits below the stage, on the right of the screen — search "crystal" if it isn't visible straight away), then picking any backdrop. Because everyone's just done a version of "delete the cat" a few minutes ago, this step should move quickly — it's a good moment to circulate and check everyone's laptop is actually on the participant site's Step 1 rather than re-checking basic Scratch orientation.

### 0:13–0:18 — Steps 2–3: Give it a memory
Creating the variable is the first slightly fiddly bit (Variables category → "Make a Variable"). Expect a few people to need a hand finding the button.

There are two reset scripts to build here, not one: the green-flag reset from before, plus a dedicated `when key r pressed` reset. Flag why explicitly — the green flag is a shared button that also restarts everything else in the programme, so a reset that's just a reset (and nothing else) is worth having on its own trigger. Once both are built, get everyone to test both together — click the green flag, then press R — a small synchronised "does it work" moment builds confidence before the harder step.

### 0:18–0:25 — Step 4: Make it respond (the main build)
This is the longest block of time for a reason — it's the step with the most new concepts (event block, change vs. set, sound, two "change color effect" blocks for the flash). Let people work at their own pace; this is where you and any co-facilitators should be circulating most.

Expect someone to ask why the `wait 0.1 seconds` block is there between the two colour-effect changes. Good question, worth having the answer ready: without it, the colour shifts on and back off in the same instant, so the flash would be invisible. The tiny pause is what makes it something the eye can actually catch.

If someone finishes early, that's what Step 6 is for — point them ahead rather than having them wait.

### 0:25–0:27 — Step 5: Personalise
Low-pressure and mostly self-directed: change the backdrop, swap the costume, change the click amount from 10 to something else. This step exists partly for pacing (it absorbs variance in how fast people finished Step 4) and partly because ownership of the output matters — "my programme," not "the programme."

### 0:27–0:28 — Step 6: Stretch goal / buffer
Only introduce this if the room is broadly on schedule. If you're behind, skip straight to wrap-up — better to finish with everyone confident in a working Step 4 build than rushed and confused by Step 6.

### 0:28–0:30 — Wrap-up
Close by naming the transfer explicitly:

> "What you just built — a trigger, a stored value, and a response — is the core loop of software engineering. Every fintech app, every trading dashboard, every banking system is thousands of versions of what's on your screen right now. You already did the hard part: you proved to yourself you can pick this up."

Point people to the certificate section on the site — type your name in, print if you'd like a copy — and to where they can go next (see Appendix C).

---

## Common issues & quick fixes

| Problem | Fix |
|---|---|
| Accidentally deleted a sprite | No confirmed way to bring back a deleted sprite specifically — just re-add Crystal from the library, no real harm done (it takes seconds) |
| Accidentally deleted or moved a block | Right-click in the scripts area and choose **Undo** (or press **Ctrl+Z**, **Cmd+Z** on Mac) — this reverts the last change to the code. Worth knowing yourself and passing on; it covers most in-script slip-ups |
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

**1. The buddy system.** Seat people in loose pairs from the start, ideally mixing anyone who's more nervous with anyone who's confident with logical or structured tools — that's not only "prior tech exposure." Someone who's spent years being the go-to for Excel at work will often pick this up just as fast as someone who's coded before, and pairing them with a first-timer works well for both: the confident one consolidates by explaining, the nervous one gets a patient, non-facilitator source of help. Frame it once, early: "If you finish a step, the fastest way to help is to turn to your neighbour before waving me over — I'll always come, but you'll get unstuck faster with someone right next to you." This also takes pressure off you as the only source of help in the room.

**2. The core-4 fallback.** If someone is visibly behind by the time the room reaches Step 5, give them permission to drop to a minimal version rather than rushing the full six-block build:

```
when this sprite clicked
change Savings by 10
```

That's it — two blocks. It's still a real, working, testable programme: click the crystal, watch the number go up. Say this explicitly: *"That's a complete build. The sound and the colour flash are polish, not the point — you've already written the part that matters."* People who came in anxious about "not being technical" need to hear that a small working thing counts as a win, not a shortfall. They can add the sound and flash back in during Step 5's personalise time if they want to, with no pressure to.

**3. Narrate the fix, don't just make it.** When you sit with someone, resist doing the click-and-drag for them. Point at the gap between two blocks, or name the block they're missing ("you need one more block from the Sound category") and let them place it. The 30-minute win is "I did this," not "it got done."

**Language that helps, generally:** avoid "it's easy" — for someone who's never done this, it isn't, and being told it is makes struggling feel like personal failure. Better: "this is the fiddliest step in the whole thing, everyone slows down here," which is true and normalises it.

**Reading the room: three patterns you'll likely see.** You don't need to label anyone, but it helps to recognise these shapes of participant in advance, because they need quite different things from you:
- **The nervous first-timer.** Hesitates before clicking anything, apologises for "silly questions," may be worried about breaking the laptop. Needs reassurance before instruction — a quick "you can't break anything here, everything's undoable" goes further than another explanation of the block itself.
- **The confident logical thinker — often someone respected for spreadsheet or analytical work, even with zero coding background.** Moves through Steps 1–4 quickly, may look for the "real" challenge, is at risk of feeling patronised by over-explanation. Best used two ways: point them at the compound-interest extension by name (it maps almost exactly onto a self-updating spreadsheet formula, and telling them that up front lands well), and/or pair them with someone who needs more support once they're done — they're usually a better second teacher than you'd expect.
- **Someone who actively avoids using a computer, even at work.** This is different from ordinary nerves — the gap here is often mechanical rather than conceptual. Right-clicking, dragging, and finding small buttons on screen can all be genuinely unfamiliar physical skills, not just unfamiliar ideas, and this is usually the person most likely to visibly freeze at Step 1 specifically, before any of the "coding" content even starts. Don't assume any reference point — not spreadsheets, not apps, nothing. The most useful thing you can do is stay physically close through Step 1 (the first right-click and first drag), rather than the later steps: once someone's cleared that hurdle once, the rest of the session tends to go much better than the start suggested it would.
- **The curious dabbler.** Not nervous at all — this is the person who reads about AI, fintech, and "the future of work" in their news feed and came along specifically to see what's actually behind the headlines. Mechanically they're often at the same starting point as the nervous first-timer (little or no hands-on experience), but emotionally they need the opposite thing: they don't need reassurance, they need the "why it matters" content and the career/pivot conversation leaned into, not softened. This is the person most likely to ask "so could I actually do this for a job?" — treat that as the real question it is (see the new pivot note in Appendix D) rather than a throwaway.

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
5. Drag: `when this sprite clicked` + `change Savings by 10` + `play sound` (pick whatever sound is already on your sprite, in the Sounds tab — or add any short one from the sound library) + `change color effect by 25` + `wait 0.1 seconds` + `change color effect by -25`. Click the crystal to test.
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

## Appendix D: "could I actually pivot into tech from here?"

Several people in a room like this are attending precisely because they're weighing this question, quietly, about their own career — and 30 minutes of Scratch doesn't answer it on its own. If someone asks directly (or looks like they want to but haven't), it's worth having a genuine, specific answer ready rather than just general encouragement. A few real, well-trodden routes from a bank operations/finance background into a tech-adjacent role, roughly ordered by how close they are to skills already being used day-to-day:

- **Business analyst / Data analyst.** The closest jump. Spreadsheet fluency, understanding a process end-to-end, and knowing what "the business" actually needs are the core of this role — SQL and basic reporting tools are usually the only new technical skill, and are learnable in months, not years.
- **QA / Test analyst.** Rewards exactly the kind of careful, rule-following, "what happens if I do this instead" thinking this session just practised. Increasingly automatable-skills-adjacent (some test scripting), but plenty of roles are still largely manual testing against requirements.
- **Low-code / no-code development.** Tools like Power Apps, Power Automate, or Airtable let people build real internal tools — the same trigger→logic→response pattern from today — without full programming. A genuinely common route for people from operations backgrounds inside large companies, including banks, who already know a business process cold.
- **Scrum / Delivery / Project support.** Doesn't require coding at all, but sits inside tech teams and benefits enormously from understanding roughly how software gets built — which is exactly what today covered in miniature.
- **Compliance/risk-adjacent tech roles** (e.g. RegTech, fraud analytics). For anyone already in compliance, fraud, or risk, some banks have teams doing exactly that work but with more technical tooling — often an internal move rather than a new employer.

Keep this light and factual rather than a pitch — the honest answer for most people is "yes, but it's a real path with real learning, not a weekend's worth." That's still a genuinely useful thing to hear from someone who wasn't sure it was possible at all.
