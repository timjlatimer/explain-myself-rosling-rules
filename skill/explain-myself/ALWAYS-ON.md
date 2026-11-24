# Explain Myself with Rosling Rules: always-on prompting

Rule 49 (Tim, 24 Nov 2026): the assistant offers an Explain Myself video whenever it fits, so nobody has to remember the skill exists. Pick the block for the tool you use. Each one does the same job.

## The offer line (used by every block below)
> **/explain-myself is ready.** Want an Explain Myself video of this? Recommended: size 3, about 1 minute. Yes / Shorter / Longer / Not now.

Offer it when the reply explains something complex, hands work to someone, gives a status update, or a decision is waiting on a person. Do not offer it for quick facts, small edits, or when the person said "not now" in this conversation.

## 1. Claude projects (claude.ai) and Claude Code: add to project instructions or CLAUDE.md
```
Explain Myself with Rosling Rules is installed as /explain-myself.
When your reply explains something complex, hands work to someone, gives a status update,
or a decision is waiting on a person, start the reply with one line:
"/explain-myself is ready. Want an Explain Myself video of this? Recommended: size <n>, about <length>. Yes / Shorter / Longer / Not now."
Choose the size and length yourself. Skip it for quick facts, small edits, or after "not now".
If they say yes, run /explain-myself with the topic already filled in.
```

## 2. Claude Code: a hook that reminds on every prompt
Add to `~/.claude/settings.json` (all projects) or `.claude/settings.json` (one project). The reminder goes into Claude's context before each reply; Claude still decides whether the offer fits.
```json
{
  "hooks": {
    "UserPromptSubmit": [
      { "hooks": [ { "type": "command",
        "command": "echo 'Explain Myself check: if this request is a complex explanation, a hand-off, a status update or a pending decision, open your reply by offering /explain-myself with a recommended size and length. Skip it for quick facts or after not now.'" } ] }
    ]
  }
}
```

## 3. ChatGPT (Custom GPT or Project instructions) and Gemini (Gem instructions)
```
You can make Explain Myself videos using the Rosling Rules (see the attached SKILL.md).
When your reply explains something complex, hands work to someone, gives a status update,
or a decision is waiting on a person, start with one line:
"Explain Myself is ready. Want an Explain Myself video of this? Recommended: size <n>, about <length>. Yes / Shorter / Longer / Not now."
If yes, ask the four setup questions from SKILL.md as multiple choice with your best guess picked, then write the script and shot list.
```
