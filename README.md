# EON Focus Finder V2

This is a UI-focused duplicate of the original Finder. The original dataset and Focus Score are preserved.

## Added
- Executive KPI cards
- Fit vs Readiness decision lens
- 2x2 action matrix (Contact Now / Monitor / Review Fit / Research)
- Search + segment + subvertical + trigger + action filters
- Sort by Focus, Fit, Readiness, or company name
- Click-through company decision drawer
- Better mobile layout

## Important methodology note
The original Focus Score is not changed. The new Fit and Readiness scores are explicitly provisional UI lenses:
- Fit: training evidence 25 + safety evidence 25 + expansion evidence 20 + subvertical 15 + enrichment 15 - profile-review penalty 30, clamped to 0-100.
- Readiness: `(existing tier points + existing signal points) / 59 * 100`.

These formulas should be reviewed by the team before being treated as a final EON scoring methodology.

## Run
GitHub Pages: upload both `index.html` and `focus-dataset.json` to the same directory.

Local preview:
```bash
python -m http.server 8000
```
Then open http://localhost:8000/.
