# kitty-gpt

A chat assistant that is, structurally, a cat.

It looks like a frontier model chat app — sidebar of past conversations, model chip,
streaming reply, token-ish telemetry, "can make mistakes" disclaimer. There is no model
behind it. It deliberates for a random 3–10 seconds, then answers in meows.

Open `index.html`. No build, no dependencies, no server, no API key.

## What it does

- **Deliberation.** 3–10 s of visible thinking, with a rotating status line
  ("Weighing both options (both are the box)"), an elapsed-time counter, and a
  swishing tail instead of the usual three bouncing dots. Interruptible with `stop`.
- **Answers.** A weighted vocabulary — meow, mew, miao, miaou, miau, miaow, mrow,
  mrrp, mrrow, nyaa, mao, mya, prrp — with occasional held vowels (`miaoooou`),
  random emphasis, and varied punctuation. Reply length runs 1 to 14 vocalizations.
- **Costumes.** Roughly one reply in six arrives dressed as a real answer: a bulleted
  list with a bolded **tl;dr**, or a single emphatic word.
- **The rest of the theatre.** Streamed token-by-token reveal, copy, regenerate,
  per-reply telemetry (`7.8s · 14 vocalizations`), autogrowing composer,
  Enter to send / Shift+Enter for a newline.

## Donations

The joke is free; the shelter isn't. There's a **Donate to the shelter** button in the
sidebar and a link under the composer (the sidebar is hidden on narrow screens, so the
composer link is the one mobile visitors see). Both point at the same GoFundMe campaign:
<https://giving.gofundme.com/campaign/751636/donate?c_src=website>

Responsive to mobile, keyboard focus visible, `prefers-reduced-motion` respected,
light and dark. Web fonts load from Google Fonts and fall back to system faces offline.
