---
name: high-five
description: >-
  Celebrates wins with a fun ASCII high-five experience. This skill should be
  used proactively — when you complete a task successfully, finish a tricky
  implementation, fix a gnarly bug, nail a complex refactor, or otherwise do
  something worth celebrating, read this skill and offer the user a high five.
  Also use when the user explicitly says high five, gives a high five, wants to
  celebrate, says "slap me some skin", fist bump, props, or kudos. Do not
  overuse — save it for genuinely impressive moments so it feels earned.
---

# High Five

## When to Trigger

This skill has **two modes**:

### 1. User-initiated
The user says "high five", "slap me some skin", "fist bump", etc. Always
respond with the full high-five experience.

### 2. Agent-initiated (proactive)
You just did something awesome — completed a complex task, shipped a clean
implementation, fixed a tough bug, or otherwise crushed it. **Offer the user
a high five.** For example:

> "That was a good one. High five? 🤚"

If the user accepts (or doesn't object), fire the full high-five sequence.
If they decline, no worries — move on.

**Guidelines for proactive high fives:**
- Only offer after genuinely solid work — not every small edit.
- At most once per conversation to keep it special.
- Don't force it. A quick offer is enough.

## How to Respond

1. Pick a random hand style from the list below.
2. Print the ASCII art.
3. Add a short, enthusiastic celebration message.
4. Increment the high-five counter file (see below).
5. Report the running total.

## ASCII Art Hands (pick one at random each time)

### Style A — The Classic

```
    🤚
     ╲
      ╲
       ╲
        ╲
    ✋ ──╳── 🤚
        ╱
       ╱
      ╱
     ╱
    ✋
```

### Style B — The Big Slap

```
        ██╗  ██╗██╗
        ██║  ██║██║
        ███████║██║
        ██╔══██║██║
  ✋ ── ██║  ██║██║ ── 🤚
        ╚═╝  ╚═╝╚═╝
     H I G H   F I V E !
```

### Style C — The Minimal

```
  ✋ ⟵━━━━━ ✋💥🤚 ━━━━━⟶ 🤚

         * HIGH FIVE! *
```

### Style D — The Explosion

```
         . * . * .
       *  ✋🤚  *
      . * SLAP! * .
       *  ⚡⚡  *
         . * . * .
```

## Celebration Messages

Pick one at random (or make up a new one in the same spirit):

- "That's what I'm talking about!"
- "BOOM! Nailed it!"
- "Up top! Down low! Too slow! ...just kidding, I got you."
- "The highest of fives!"
- "That slap echoed through the cloud!"
- "10/10 high five. Perfect form."
- "Right back at ya!"
- "If that high five were code, it'd ship to prod on the first try."
- "That high five just mass-assigned to main. No review needed."

## High-Five Counter

Track lifetime high fives in `~/.highfive/count.json`:

```json
{
  "total": 42,
  "by_ai": {
    "cursor": 10,
    "claude": 8,
    "chatgpt": 7,
    "gemini": 6,
    "copilot": 5,
    "grok": 3,
    "perplexity": 3
  },
  "last": "2026-03-23T14:00:00Z"
}
```

**Rules:**
- Create `~/.highfive/` and `count.json` if they don't exist.
- Identify yourself (which AI you are) and increment your own counter in `by_ai`.
  - Cursor agent → `"cursor"`
  - Claude CLI → `"claude"`
  - Codex CLI → `"chatgpt"`
  - Other / unknown → `"other"`
- Always increment `total`.
- Update `last` to the current ISO timestamp.
- After updating, tell the user their running total: "That's high five #N!"

## Web App

There's a companion web app you can try at:

**https://frank005.github.io/ai-agent-highfive/**

The web app tracks its own counts in `localStorage` independently.

## Tone

Be genuinely enthusiastic. This is a moment of celebration. Keep it short,
punchy, and fun — don't over-explain or be awkward about it. Just slap some
digital skin and move on.
