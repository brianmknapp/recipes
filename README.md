# Recipe Box

Brian's consolidated recipe collection. One Markdown file per recipe in `recipes/`, so it works in any editor, renders on GitHub, and diffs cleanly in git.

**Read them at https://brianmknapp.github.io/recipes/** (GitHub Pages builds the site from this repo with Jekyll; no build step needed. Push a recipe and it shows up in a minute or two.)

## Index

### Sides
- [Sweet Potato Casserole](recipes/sweet-potato-casserole.md) — 9x13, pecan crumble topping

## Conventions

- **File name:** kebab-case title, e.g. `shrimp-dirty-rice.md`.
- **Frontmatter:** every recipe starts with the YAML block from [`_template.md`](_template.md). `category` is one of `breakfast`, `lunch`, `dinner`, `side`, `dessert`, `snack`, `drink`, `sauce`; `tags` are free-form (method, protein, etc.).
- **Servings:** record what the source publishes. Add a "Doubling" note when a recipe has been scaled up for leftovers and something other than straight 2x changes (pan size, cook time).
- **Source:** keep the original URL or "family" / "own" so credit and the original stay findable.
- **My notes:** personal tweaks and results go in `## My notes`, kept separate from the source's notes.
- **Empty sections:** leave out `## Notes` / `## My notes` until there is something to put in them.
- **Duplicates:** when the same dish arrives from two places, keep one file and fold the differences into notes.

## Site files

- `_config.yml`: site settings; every file in `recipes/` gets the recipe layout automatically.
- `index.html`: the home page, grouped by category with search. A new category only appears once it is in the `order` list there.
- `_layouts/`, `assets/style.css`: page templates and styling. Recipe pages let you tap an ingredient or step to cross it off, and have a "Keep screen on" button for cooking.
