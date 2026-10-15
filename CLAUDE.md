# ICT Quizzes

O/L ICT lesson quizzes for Nilupul's online class, hosted on GitHub Pages.

- Repo: https://github.com/Nilupul-byte/ict-quizzes (public; Pages serves `main` from root)
- Live: https://nilupul-byte.github.io/ict-quizzes/
- Pushing to `main` redeploys in about a minute. Check with
  `gh api repos/Nilupul-byte/ict-quizzes/pages/builds/latest --jq .status`

## Files
- `index.html`: home page listing every quiz. Add a link here for each new quiz.
- `lessonNN.html`: Sinhala medium quiz for lesson NN (two-digit number, e.g. `lesson09.html`).
- `lessonNN-en.html`: English medium version of the same lesson.

Keep existing filenames stable, since students already have the links.

## Quiz format
Each quiz is one self-contained HTML file with no build step and no external JS (only Google Fonts).
New quizzes follow `lesson09.html`:
- Questions are in O/L Paper I MCQ style, with 4 options numbered (1)–(4).
- Questions are grouped under scenarios (`S`) that show sample tables. Each question (`Q`) has
  `s` (scenario), `q`, optional `st`/`q2` (statement-style questions), `o` (options),
  `a` (0-based correct index) and `e` (explanation).
- There is a 60s timer per question. Faster answers score more, and 3+ correct in a row gives a streak bonus.
- At the end, students copy their result text and paste it into the class chat.
- The footer shows Nilupul's name and contact number.
