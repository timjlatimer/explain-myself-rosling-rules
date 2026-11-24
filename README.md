# Explain Myself with Rosling Rules

Type `/explain-myself`, answer five quick menus, and get a short, honest, photoreal film that explains your idea to the people who need to act on it. The rules come from the way Hans Rosling presented: show, don't just tell; one big idea at a time; real numbers; honest about what we don't know; end with who does what, by when.

**Status:** v0.5 draft, 24 November 2026. Fidel reviews, polishes and decides whether it becomes the skill (he is the 1NTC for this).

## Start here
| What | Where |
|---|---|
| The guide (web page with both films, the menus and every rule) | `docs/index.html` (turn on GitHub Pages: Settings → Pages → main / docs) |
| The skill | `skill/explain-myself/SKILL.md` |
| Make Claude offer it by itself | `skill/explain-myself/ALWAYS-ON.md` |
| All the rules | `RULES.md` |
| The five menus, with pictures | `MENUS.md` and `menus/` |
| The shared media library and cast bible | `library/` |
| The films | `FILMS.md` |

## Install
**Claude Code:** copy `skill/explain-myself/` into `~/.claude/skills/` (just for you) or `.claude/skills/` in a project (for everyone on it). Then type `/explain-myself`.

**claude.ai:** Settings → Capabilities → Skills → upload a zip of the `skill/explain-myself/` folder. Or paste SKILL.md into a project's instructions.

**ChatGPT or Gemini:** paste SKILL.md into custom instructions or a custom GPT / Gem. They can write the script and shot list; making the film needs image, voice and video tools.

To have it offered without asking, add block 1, 2 or 3 from ALWAYS-ON.md.

## The five menus, in one line each
1. **Topic and audience**: the one idea, and who it is for.
2. **North Star and 1NTC**: what the film must achieve, and the one person who owns the decision.
3. **Format, size and length**: always a photoreal movie unless you ask for slides; size 1 (30 s) to 10 (documentary).
4. **Quality** (new): Draft (free, the default), Standard, High, Premium.
5. **Ending**: who does what, by when. The film recommends; the 1NTC decides.

## Honesty, always
Generated pictures and voices are labelled. Concepts are labelled "not built". Real people's faces are never invented. Untested things are named.

Made for Business as a Force for Good. Solve for Ruby Red: if a film is clear for her, at midnight, on her phone, it is clear for everyone.
