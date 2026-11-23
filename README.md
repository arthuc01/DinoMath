# 🦕 DinoMath

**A low-pressure dinosaur maths adventure for learners working across England's KS1–KS3 curriculum.**

DinoMath combines adaptive practice with playful exploration, helpful explanations from **Dr Bones**, dinosaur eggs and fossils to discover, and a museum where children can assemble skeletons. It was designed with children who find traditional worksheets stressful in mind, but is intended to be enjoyable and useful for a wide range of learners.

> **Status:** Experimental prototype (v0.5). Not a validated teaching or assessment programme. Mathematical content and accessibility need further educator and learner testing.

## Play

Open `index.html` on a local web server or a static hosting service. **No build tools, accounts, API keys or backend are required.**

### Run locally

```bash
git clone https://github.com/arthuc01/DinoMath.git
cd DinoMath
python -m http.server 8000
```

Then open **http://localhost:8000**.

You can also download the repository and open `index.html` directly in many desktop browsers. For Android, serving it over HTTPS is more reliable than opening a local HTML file. This initial GitHub version uses a self-contained JavaScript bundle; dinosaur portraits are embedded so the game does not request images from external services.

### Publish with GitHub Pages

In the repository, go to **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, select **main / (root)** and save. After publication, the site should be accessible at:

**https://arthuc01.github.io/DinoMath/**

Pages publication must be enabled separately; committing the code does not automatically activate it.

## Dr Bones — new guide and character art

The original DNA mascot has been replaced by **Dr Bones**, a welcoming cartoon palaeontologist. Nine species-independent character assets now provide distinct poses for welcome, thinking, maths explanations, fossil discoveries, egg rewards, investigating and gentle support after mistakes.

The language throughout the game has been revised to be calmer, more specific and less repetitive, without changing mathematical answers or the underlying progression rules. See [CHARACTER_ASSETS.md](CHARACTER_ASSETS.md) for the asset list, display guidance and voice style.

## What children can do

- **Explore eight maths regions:** Nest Valley, Fernwood Grove, Tidal Cliffs, Crystal Caverns, Jurassic Quarry, Volcano Ridge, Research Station and Migration Plains.
- **Choose Discovery Trails or Skill Focus:** mixed expeditions or structured practice in one specific skill.
- **Try varied puzzle interactions:** calculations, number lines, fraction models, number ordering, spotting errors and more.
- **Get help from Dr Bones:** hints, worked solutions and hands-on workshops, including signed numbers, fractions, balancing equations and proportional reasoning.
- **Build a collection:** find dinosaur eggs, hatch species-matched dinosaurs, reveal portraits in pieces, and collect repeatable fossils and tools.
- **Assemble skeletons:** reconstruct simplified Baryonyx, Iguanodon, Scelidosaurus and Triceratops museum displays using seven sections each, without needing to grind for parts.
- **Play at their own pace:** no timers, public rankings, punishment streaks or compulsory long sessions.

The dinosaur collection includes species from Britain and Europe as well as some better-known international favourites. The stylised portraits are matched to their respective species.

## Learning approach

The current curriculum outline maps **65 micro-skills** across KS1–early KS3; **32 have playable question generators**, each with four challenge tiers. The pathway emphasises small steps, prerequisite knowledge, visual representations and gentle explanations.

A challenge tier opens after **10 completed attempts and at least 7 of the latest 10 answered independently**. This is an adjustable *prototype rule*, not a proven mastery threshold. Mistakes do not erase previous progress. An incorrect question is not repeatedly presented until the learner clicks the correct answer: the game explains the mistake and schedules a changed version after other questions.

The full skill map and planned curriculum gaps are described in [CURRICULUM_PLAN.md](CURRICULUM_PLAN.md).

## Parent controls

Parents can select a mathematical topic and challenge tier, switch expedition modes, view skill progress, choose shorter sessions and review prerequisites. Parent controls are **not yet protected by a PIN**.

Progress is stored in the browser's **localStorage**. There are no accounts, cloud-sync features or advertising. Progress may not automatically transfer between browsers, devices or downloaded copies; a parent-facing JSON export is available for backup, but import is not yet implemented.

## Repository structure

```text
index.html           Game entry point
styles.css           Responsive interface and animations
app.js               Playable JavaScript bundle (including embedded dinosaur artwork)
CURRICULUM_PLAN.md   Curriculum design, progression and known gaps
README.md            Project guide
LICENSE              Unlicense
```

This deployment uses the consolidated v0.5 browser bundle. A future maintenance step is to restore its separately maintained curriculum, maths-engine, teaching, reward and museum modules to the repository, with automated tests and a reproducible build process.

## Educational and technical limitations

- This is a prototype, **not a replacement for a teacher or specialist assessment**.
- Puzzle generators have been checked programmatically in development, but the complete curriculum has not had an independent mathematics-education review.
- Dinosaur skeletons are simplified interaction diagrams, not anatomically accurate scientific reconstructions; AI-assisted species portraits also need a scientific review.
- The website is designed for mobile screens but has not had a complete Android-device or accessibility audit.
- The current ten-question progression rule should be tuned using learner feedback, not treated as an assessment standard.

## Curriculum and teaching references

- [DfE mathematics programmes of study](https://www.gov.uk/government/publications/national-curriculum-in-england-mathematics-programmes-of-study)
- [DfE teaching mathematics at KS3](https://www.gov.uk/government/publications/teaching-mathematics-at-key-stage-3)
- [EEF: Improving Mathematics in Key Stages 2 and 3](https://educationendowmentfoundation.org.uk/education-evidence/guidance-reports/maths-ks-2-3/)
- [Natural History Museum dinosaur directory](https://www.nhm.ac.uk/discover/dino-directory.html)

## Licence

Released under the [Unlicense](LICENSE), as specified by this repository. DinoMath is not affiliated with Kumon, Jurassic Park, Pokémon or any other entertainment franchise.
