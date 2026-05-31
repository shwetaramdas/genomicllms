# BDBio 2026 — LLMs in Genomics · Workshop Resource Page

A resource hub for the workshop on large language models in genomics, plus the hands-on
tutorial notebook students run.

## Files

| File | What it is |
|------|------------|
| `index.html` | The page, fully self-contained (no build step). **This is what GitHub Pages serves by default.** |
| `index.md` | Same content as Markdown, with Jekyll front matter — use this instead if you prefer editing Markdown / a Jekyll theme. |
| `latest-bdbio-may30.ipynb` | The tutorial notebook (Part 1: using DNA LMs; Part 2: LoRA fine-tuning). The page links to it. |

> If both `index.html` and `index.md` are present, GitHub Pages serves `index.html`.
> Keep the one you want as the homepage and delete or rename the other.

## Deploy to GitHub Pages (5 minutes)

1. Create a repo (e.g. `bdbio-llm-genomics`) and add these files to the root.
2. **Settings → Pages → Build and deployment → Source → Deploy from a branch.**
3. Branch `main`, folder `/ (root)`, Save. Live in ~1 min at
   `https://<username>.github.io/<repo>/`.

## Edit before sharing — search for `EDIT ME` (4 spots)

| # | What | Where |
|---|------|-------|
| 1 | Page title + workshop date/venue/instructors | `<head>` + `.meta` card (HTML) / top table (MD) |
| 2 | (same meta block) | hero |
| 3 | **Colab / Kaggle / slides links** for the tutorial | the dark "tutorial" panel in section 00 |
| 4 | Contact email + repo link + "last reviewed" date | footer |

All `[ bracketed ]` text and `href="#"` links are placeholders.

## Adding the Colab / Kaggle "Open in…" links

- **Kaggle:** upload the notebook as a Kaggle Notebook, then copy its public URL into the
  "Open in Kaggle" link.
- **Colab:** once the repo is public, the notebook opens at
  `https://colab.research.google.com/github/<username>/<repo>/blob/main/latest-bdbio-may30.ipynb`
  — paste that into the "Open in Colab" link. (Replace `<username>/<repo>`.)
- The **Download notebook** link already works — it points to the `.ipynb` in the repo.

## Accuracy note

Links were verified current at build time, but the field moves fast — AlphaGenome and Evo 2
both reached *Nature* and changed access terms within the last few months. **Click through each
link once before sharing**, and update the "last reviewed" date.

A few links in sections 02/06 (Caduceus, GENA-LM, ESM-3) come from general knowledge rather than
a fresh check — worth a quick confirm.

## Editing tips (HTML)

- To add a resource, copy an `<article class="card">…</article>` block and edit it.
- Colours/fonts live in the CSS `:root` variables at the top of `<style>`.
- `class="card flag"` adds a left accent bar; `<span class="used">tutorial</span>` adds the
  small badge marking models used in the notebook.
