# Mirror Archetype Quiz

A lightweight static quiz prototype for GitHub Pages.

## What it includes
- 15-question transformation quiz
- 5 family tracks: Hearth, Spark, Glass, Moon, Kaleido
- 19 end-state archetypes
- gradual mirror checkpoints after question 5 and question 10
- result cards with placeholder blurbs for UI testing
- debug score display at the end

## GitHub Pages setup
1. Create a new GitHub repository.
2. Upload these files to the repository root:
   - `index.html`
   - `styles.css`
   - `script.js`
   - `README.md`
3. Commit and push.
4. In GitHub, open **Settings > Pages**.
5. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
6. Choose the `main` branch and `/root` folder.
7. Save.
8. Wait a minute or two and GitHub will publish the site.

## Editing notes
- All quiz logic and content live in `script.js`.
- `QUESTIONS` contains the questionnaire.
- `RESULT_CARDS` contains title, subtitle, test blurb, and image hints.
- `buildFinalResult()` resolves the final archetype.
- `renderCheckpoint()` controls the interim transformation reveals.

## Known follow-up tasks
- replace placeholder blurbs with final result prose
- tune any overlapping archetypes after playtesting
- add local save state if desired
- add image generation hooks or prompt templates if you want result art generated automatically later
