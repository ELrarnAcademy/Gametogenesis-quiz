# EasyLearn Quiz (GitHub Pages)

This is a **ready-to-publish** quiz template for GitHub Pages. Content is loaded from `config.json` and `questions.json`.

## Quick Publish (5 steps)
1. Create a new repository on GitHub (e.g. `easylearn-quiz`).
2. Upload **all files and folders** from this package (`index.html`, `config.json`, `questions.json`, and the `assets/` folder).
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**. Select branch **main** and folder **/** (root). Save.
5. Wait for deployment. Your quiz will be live at `https://<username>.github.io/<repo>/`

> If updates don’t appear right away, refresh with `Ctrl+F5`. The app also adds a small cache-busting token when fetching JSON.

## Edit Content
- `config.json`: change university name, quiz title, time per question, shuffle settings, and logo path/URL.
- `questions.json`: replace with your own questions (array of objects). Supports MathJax (`\( ... \)` for inline LaTeX).

Each question:
```json
{
  "q": "Your question text",
  "options": ["A", "B", "C", "D"],
  "answer": "Correct option text",
  "explanation": "Shown after answering."
}
```

## Tips
- Total time is calculated automatically as `secondsPerQuestion × numberOfQuestions`.
- You can set `logoSrc` in `config.json` to any URL (PNG/JPG/SVG on the web) or a file in `assets/`.
- To keep questions private, use a private repo and share a zip, or host on an internal Pages alternative.
