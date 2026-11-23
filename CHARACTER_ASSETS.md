# Dr Bones — character assets and voice guide

Dr Bones is DinoMath's original, fictional palaeontologist, fossil expert and gentle maths guide. He is an approachable companion, not an authority figure who scores or judges children. Artwork is original AI-assisted game illustration created for this project.

## Ready-to-use art

All images have transparent backgrounds and are served locally from `assets/dr-bones/`. They are compressed WebP files, with the same wardrobe and appearance in every pose.

| File | Role | Suggested use |
| --- | --- | --- |
| `welcome.webp` | Open-palmed greeting, holding a field notebook | Home screen, joining a new expedition |
| `thinking.webp` | Calm, reflective expression | Hints, planning, pauses |
| `explaining.webp` | Friendly open-hand gesture | Maths workshops, worked examples |
| `pointing.webp` | Fossil brush used to point | Demonstrating a number line or visual model |
| `discovery.webp` | Excited about a fossil | Fossil discoveries, new field-journal entries |
| `egg.webp` | Gently holding a dinosaur egg | Egg found / egg hatching reward |
| `investigating.webp` | Magnifying glass and ground inspection | Fossil dig, skeleton identification |
| `puzzled.webp` | Wondering about a result | Incorrect answers, checking a method |
| `portrait.webp` | Cropped head-and-shoulders portrait | Compact dialogue panels and guidance |

The art is designed for display around 60–220 pixels. Do not stretch it or use `object-fit: cover` on full-body poses: that can cut off hands, brushes or boots. Display at natural aspect ratio with `object-fit: contain` and transparent padding. Don't use the character's facial expression as a correctness judgement.

### Suggested later assets

A restrained 3–5 frame blink, a slow wave, a small head nod, a 'reading quietly' idle pose, a transparent larger teaching-board pose, and optional profile variants. Animation must respect the reduced-motion setting. These are **planned**, not yet included.

## Voice and feedback

- **Curious, not corrective:** “That result doesn't quite fit. Let's examine the steps.”
- **Method-specific:** “The number line shows a move through zero. Which way did we travel?”
- **Unhurried:** “Your notes are saved. We can come back whenever you like.”
- **Specific rewards:** “A Baryonyx fossil! See how the claw curves?”
- **Respect learner agency:** “Would you like a hint, a model, or a different puzzle?”

Avoid “Wrong!”, “You failed”, performative applause, constant compliments and unhelpful “Try harder” messages. If a child is frustrated, give a shorter explanation and offer a different task or the freedom to stop.

## Accessibility and interaction

A small portrait is decorative when adjacent to text identifying Dr Bones (`alt=""`), while the home hero has an informative alt description. The dialogue itself should always be readable without the illustration. Keep maths as the main visual focus on narrow phones and never cover errors or worked examples with a pop-up. Most poses remain static; discoveries are shown only when opened by the learner.

## Character originality

Dr Bones is not a DNA helix mascot or a specific film character. Avoid recognisable costume or scene references from existing franchises. An independent art and factual review is advisable before wider public promotion or commercial use.
