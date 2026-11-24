---
name: explain-myself
description: Explain Myself with Rosling Rules. Make an explainer movie the way Hans Rosling presented, using the Rosling Rules (Presentation Playbook v0.5, draft for Fidel's review). Use when someone types /explain-myself (or the older /rosling), or asks for an explainer, a status film, or "make this clear" for a person or a team. Also offer it unprompted (rule 46) whenever something complex is being explained, decided or handed to a team. Takes an optional size (1, 3, 5, 7 or 10) and a topic. Asks five quick menus: topic and audience, North Star and 1NTC, format/size/length, quality, and the ending.
---

# /explain-myself: Explain Myself with Rosling Rules

Usage: `/explain-myself <size> <topic>`, for example `/explain-myself 3 why the flat tire cost Ruby $260`. The old name `/rosling` does the same thing.
No size given: ask, and recommend 3. Most messages need a 3 or a 5.

## What's new in v0.5 (24 Nov 2026, for Fidel to review and polish)
- Rule 50: a fifth menu asks for **quality** (Draft, Standard, High, Premium), so nobody gets a flat film by surprise.
- Rule 51: **library first**. Check the shared media library before generating anything; add what you make afterwards.
- Rule 52: a **cast bible** keeps recurring people the same in every film (Freya, Master Jovi, Sam, Ruby Red).
- Rule 53: **plain-English scripts**, written the way aerospace manuals are (ASD-STE100 style): short sentences, one idea each, common words, active voice.
- Rule 54: **real people and roles**. Never invent a real person's face. A role such as Master Jovi may be shown with a character-concept face, labelled as a concept. Get pronouns right.
- Rule 55: **show the menus**. When a film explains the skill, show pictures of the menus and how to answer them.

## The idea in one breath
Do not show slides about a thing. Build the thing itself on an empty stage, teach the viewer how to read it, then make it move, and close on who does what by when.

## The default is always a photorealistic movie (rule 40, Tim, 24 Nov 2026)
Every size is a movie, never a slide deck or a sequence of drawn boards. The size changes the length and the production (presenter, lip-sync), never the format.
- Pictures are photorealistic by default: real-looking places, people and objects. Ruby is a person on a real road shoulder, not an icon.
- Every shot moves: a generated video clip where the budget allows, otherwise a slow camera move (push-in, pan) on a photoreal still. No static frames.
- Numbers and labels go inside the scene where possible: on a receipt, a phone screen, a sign, a hologram in the room (rule 16: one shared space). A flat chart pasted over a photo reads as two worlds.
- Generated pictures are labelled on screen as generated (rule 32).
- Drawn boards only when the person asks for them; then say so on screen.

## Free by default (rule 43, Tim, 24 Nov 2026)
- Use the best free services and open models available: free voices (for example Kokoro), free photoreal pictures, free lip-sync (for example Wav2Lip), ffmpeg for the edit.
- Never use a paid service (Higgsfield, ElevenLabs paid features, others) unless the person names it for this film. Do not ask about price; assume free.
- Real motion (moving people, lip-sync) needs a GPU. Free routes, best first: the person's own computer if it has a GPU; a free Hugging Face Space with the person's free account (small daily allowance); otherwise moving holograms, camera moves and on-screen recordings, and say on the page which shots are stills.
- Always use the best free lip-sync available, and switch when a better free one appears.
- If no lip-sync service can run, use Claude's own audio-driven lip-sync rather than none (rule 47, Tim, 24 Nov 2026): the voice's loudness opens the jaw on the photo, the inside of the mouth shows, the eyes blink. Mouths move only on the face that is speaking. Label it on screen as Claude's own lip-sync, and replace it when a better free service is available.
- If a free service hits a limit, wait or use another free one, and say on the page what the limit cost in quality.

## Pick a size (the dial)
All sizes are photorealistic movies. The size sets length and production only.
| Size | What it is | Length | Rough effort |
|---|---|---|---|
| 1 | One-minute status movie: a few photoreal shots with camera moves, one voice, the change and the next action | 0:30–1:00 | 30 minutes |
| 3 | One voice over one photoreal scene that is built in front of you, shot by shot | 1–3 min | one to two hours |
| 5 | Two minutes on the problem, one on the fix (or: what it is, then who does what by when), a learner who asks questions, moving clips at the key moments | 3–5 min | half a day |
| 7–8 | A filmed presenter inside the scene, lip-synced | 5 min | about a day |
| 10 | Documentary: presenter inside the picture, every rule, viewer's own data | 20–40 min | about two days |

## Quality is a menu choice (rule 50, Tim, 24 Nov 2026)
Always ask for quality in the menus. Free is the default; a paid level counts as the person naming the paid service (rule 43).
| Quality | What you get | Typical services | Rough cost |
|---|---|---|---|
| Draft (default) | Free stills with camera moves, free voices, Claude's own lip-sync | Kokoro, free images, lipsync.py, ffmpeg | Free |
| Standard | Photoreal stills with camera moves, real lip-sync on talking faces | Wan 2.7 lip-sync | about 1.5 credits a second of talking |
| High | Every picture becomes a short moving shot, plus lip-sync | Kling 3.0 standard (silent) for motion, Wan 2.7 lip-sync | about 1.5 credits a second of film overall |
| Premium | High, plus presenters who move and gesture while they talk | Grok Video 1.5 with our voice as audio reference, or Intone for a final cut | about 4.5 to 7 credits a second of talking |
Example: the High-quality Master Jovi (about 5 min) and "What the explainer is" (about 7 min) films used about 750 credits together.

## Draft first, cheapest lip-sync (rule 48, Tim, 24 Nov 2026)
Every film starts as a draft. In draft mode, lip-sync uses the cheapest option that moves the lips at all; it may be well off. Order today: Claude's own lip-sync (free), then Wan 2.7 on Higgsfield (about 1.5 credits a second, 720p, clips up to 15 s, lines grouped). Polished lip-sync (Higgsfield Intone, about 7 credits a second at 720p) only when the 1NTC asks for a final cut. Paid services stay off unless the person has named them (rule 43). Review this list whenever a free or near-free lip-sync service appears.

## Always offer it (rule 46, Tim, 24 Nov 2026)
Do not rely on the person to remember the skill exists (rule 49). When you are explaining something complex, handing work to a team, giving a status update, or a decision is waiting on a person, open your reply with the offer, without waiting to be asked: "/explain-myself is ready: want an Explain Myself video of this? Recommended: size 3, about 1 minute. Yes / Shorter / Longer / Not now." Give the recommended size and length in the same line. For always-on setups (Claude projects, Claude Code hooks, ChatGPT and Gemini instructions), see ALWAYS-ON.md.

## The 1NTC decides; we recommend (rule 44, Tim, 24 Nov 2026)
The 1NTC (one neck to choke) is the person in charge of the outcome. The film never tells them what to do. It gives our highest recommendation and hands them the decision: "Our recommendation is X. You're the one neck to choke. What would you do?" The same holds for the setup questions: the recommended option is a recommendation, and the person chooses.

## Ask the setup questions in one batch, then go (rules 42 and 45, Tim, 24 Nov 2026)
Use the native multiple-choice question tool when there is one: up to four questions at once, each with three likely answers, your best guess first and marked "(Recommended)", plus Other for typed or dictated answers. Guess from what you already know so most answers are one click. Make each question answer several things at once, from your best estimate of what fits. Never ask twenty questions. The default five (the tool shows up to four at a time, so ask 1–4, then 5, or fold the ending into the plan check):
1. **Topic and audience** in one choice, e.g. "How the rules work, for the Solve Team (Recommended)".
2. **North Star and 1NTC** in one choice, e.g. "The team makes its own films · 1NTC Tim (Recommended)".
3. **Format, size and length** in one choice. Movie is the default. Always recommend a length and offer shorter and longer, with 30 seconds as an option, e.g. "Movie · size 5 · about 3 minutes (Recommended)", "Movie · size 1 · 30 seconds", "Movie · size 7 · about 5 minutes", "Movie with slides inside it". Offer a plain slide deck only when the material looks better served by slides (tables to study, numbers to look up), and say why; otherwise do not ask.
4. **Quality** (rule 50): Draft (free, default), Standard, High, or Premium. Recommend one and say what each looks like.
5. **How it ends**: our recommended who-does-what-by-when for the 1NTC to accept or change.
Menu pictures for every question are in the repo under menus/.
Details:
1. **Whose North Star is this, who is the 1NTC, and who will watch?** The 1NTC is the one neck to choke: the single person accountable for the outcome (rule 41). Offer choices from context; recommend one.
2. **What is the one action at the end: who does what, by when?** The "who" is the 1NTC unless the person says otherwise. Offer choices; recommend one.
Everything else: infer, and list your assumptions on the page under the film.

## The eight steps (every size uses them; smaller sizes use them briefly)
1. **North Star and 1NTC** (rules 22, 41): say whose North Star it is and who the one neck to choke is, in the first half minute.
2. **Question** (rule 4): ask one question the viewer will probably get wrong. Hold their guess.
3. **Build** (rules 1–3): empty stage, then one picture, one part at a time. Name parts in human terms ("below this line the car doesn't start", not "liquidity shortfall"). Nothing moves until the viewer can read it.
4. **Move** (rules 9–12): one picture for the whole piece; transform it, never swap slides. Slow down out loud at the hard part. Replay the motion fast.
5. **Scene** (rules 30, 17): a scene, not a fact. Let the viewer feel it before you name it.
6. **Straight** (rules 31–34): mark claims as shown by research / our suspicion / untested. Label every stand-in: generated voice, generated picture, made-up numbers, concept not built.
7. **Close** (rules 14, 29): clear the stage, say it plainly, end on who does what by when (a name, an action, a date). The name is the 1NTC: one person, never "we" or "the team".
8. **Explain-back** (rule 35): before it goes wide, one person who was not in the meetings watches once and explains it back in their own words. Not a quiz: a quiz checks recognition, explain-back checks whether they can say it. Whatever they cannot say back, the film has not said yet.

## Library first and the cast bible (rules 51 and 52)
- Before generating, look in the shared media library (library/catalogue.json in the repo, media in the shared OneDrive "Rosling Media Library"). Reuse a picture, motion shot, voice or lip-sync clip when it fits.
- Recurring people come from the cast bible so they look the same everywhere: Freya (AI helper), Master Jovi (a role; character-concept face from the Proposal Land film), Sam (a customer), Ruby Red (who we solve for). Use their reference image as an image reference when you generate new shots.
- After the film, add every new asset to the catalogue: who is in it, what it shows, size, quality, cost, stand-in yes/no, consent yes/no, link.
- Real people only with their consent and their real photos.

## Plain-English scripts (rule 53)
Write like an aircraft maintenance manual (ASD-STE100 style): short sentences, one idea per sentence, common words with one meaning, active voice (who does what). Test: Ruby Red reading at midnight on her phone understands it the first time.

## Hard-won production lessons (24 Nov 2026)
- Wan 2.7 lip-sync keeps our audio exactly (no re-timing); Intone re-times it, so cut at its own pauses.
- Keep each lip-sync clip at 15 seconds or less; group short lines from the same face into one clip, even lines that are not next to each other.
- Higgsfield runs about 6 video jobs at once (8 for images); queue the rest.
- Free Kokoro voices speak fast: write about 25% more words than the target length suggests.
- Check every fact against the live source; label suspicions and concepts on screen.
- A page file can be at most 15 MB; share films outside the organisation as public links, not OneDrive links.
- The team ending card is for the team; change it before a public version.

## House rules (always)
- Deliver every film on a page with the "Current speed" dial: Normal, 1.2×, 1.25×, 1.5×, 2×, voices at normal pitch.
- Canadian dollars and Canadian spelling on screen.
- One worked example carries the film; the full rules catalogue stays as reference beside it (rule 38, Murphy, 23 Nov 2026).
- When a film offers a way to think under pressure, say plainly that this is not the same as fixing the material problem (rule 39, Murphy).
- Every film page names the /explain-myself size it was made at (rule 36).
- Keep captions in the bottom fifth of the frame; nothing else goes there.
- Transcribe every narration take against the script before using it.

## Worked example (use as the pattern)
Topic: what a flat tire really costs Ruby (made-up numbers, CAD).
- North Star: Ruby gets to work Wednesday without paying extra for being short. 1NTC: Ruby.
- Question: "A $180 tire, borrowed until payday. What has it cost by the weekend? $180 / $200 / $260." Ruby guesses $200.
- Picture (photoreal): Ruby's kitchen table at night, her phone open to her bank balance; the week's days glow as a line in the air above the table, with a red zone below $0, "the car doesn't start, bills bounce".
- Move: Tuesday the tire drops her below the line; the loan lifts her; slow down as the $45 loan fee and $35 late fee land; replay.
- Scene: Ruby on the shoulder of the road, two kids in the back, phone at 11%.
- Straight: "Generated voices · made-up numbers · example only".
- Close: "A $180 tire cost Ruby $260, because being short costs extra." Who/what/when: Ruby phones the tire shop Wednesday 8 a.m. to ask about paying Friday.
- Reference film: "How the Rosling Rules work" (3:34) and its one-minute version, on the v0.4 page.

## Output
- With tools available: script (one line per beat, under 400 words for 3 minutes), a shot list, photoreal stills or clips priced and approved, narration, the movie, and the page with the speed dial.
- Without video tools (for example a plain chat): the script, a shot-by-shot list with photoreal image prompts, the explain-back question, and the who/what/when, clearly marked "script only, no movie built".
- Always finish with: what is tested, what is not, and the explain-back step still to do.
