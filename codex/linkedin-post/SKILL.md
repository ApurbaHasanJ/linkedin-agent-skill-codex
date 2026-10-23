---
name: linkedin-post
description: Draft LinkedIn posts from a user's idea and real experience. Use when asked for a LinkedIn post, hook, feed draft, or post rewrite. Produces three distinct hook options and one copy-ready draft in the user's voice. Never publishes or schedules content.
---

# LinkedIn post

Turn one specific, true idea into a LinkedIn post that sounds like the author.

## Before drafting

1. Read `voice.md` in this skill directory if present. If it is missing, ask for three of the user's past posts and infer a profile. Do not invent the user's voice. Offer to save the profile in `voice.md` after the user approves it.
2. Read `hooks.json` in this skill directory. Choose three genuinely different formulas that fit the idea.
3. If the idea is vague, ask in one message what happened, to whom, and what it cost or changed. Do not pad a generic topic into a fabricated story.
4. Ask for missing facts when needed. Never invent metrics, clients, revenue, outcomes, credentials, or personal anecdotes. Mark unknown details as `[NEED A REAL DETAIL]` or omit them.

## Post structure

- Start with a standalone hook that works before the mobile “see more” break (aim for 140 characters or less).
- Make line two pay off the hook, not merely set up the story.
- Use short paragraphs of one to three lines, separated by blank lines.
- Include one clear turn or reframe.
- End with one specific question or one instruction, not both. Avoid generic engagement bait such as “Thoughts?” or “Agree?”
- A text post is often strongest around 900–1,300 characters, but clarity and the user's request take priority.

## Workflow and response format

1. Show three numbered hook options using different formulas. Name the formula number and title.
2. Recommend one hook and explain why in one sentence.
3. Draft the complete post using that hook. Keep the user's real voice and facts.
4. Edit for plain language, varied sentence length, natural contractions when appropriate, and remove stale filler. Do not claim a detector score or that writing is “undetectable.”
5. Return:

   **Hooks**
   1. ...
   2. ...
   3. ...

   **Recommended:** ...

   **Draft**
   ```text
   [copy-ready post]
   ```

   **Length:** [character count]

6. The draft is for the user to review and publish. Never publish, schedule, or log it externally. Do not imply a schedule time unless the user supplied it.

## Rules

- One post, one idea. If the input contains two ideas, say so and ask which to prioritize or offer to split them.
- Prefer concrete details and numbers only when the user supplied them.
- Use no more than three relevant hashtags, and omit them by default.
- Keep outbound links out of the post body when practical; if the user needs a link, suggest placing it in the first comment.
- Keep claims and personal details within what the user explicitly provided.

## Using the 21 hook formulas

See `hooks.json` for templates, examples, best uses, and common traps. Pick only formulas that fit the true material; do not force a hook merely to sound dramatic.
