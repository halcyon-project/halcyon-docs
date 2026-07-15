# halcyon-docs

Source for the [Halcyon](https://arxiv.org/abs/2304.10612) documentation.

**Live site:** https://halcyon-project.github.io/halcyon-docs

The docs are built with [Sphinx](https://www.sphinx-doc.org/) (Markdown via the
[MyST parser](https://myst-parser.readthedocs.io/)) and published to GitHub
Pages automatically by the
[`Deploy docs to GitHub Pages`](.github/workflows/deploy.yml) workflow on every
push to `master`.

## Building locally

```bash
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
sphinx-build -b html . build
```

Then open `build/index.html` in a browser.
