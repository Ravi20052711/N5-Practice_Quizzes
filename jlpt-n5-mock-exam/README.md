# JLPT N5 Mock Exam — 日本語能力試験 N5 模擬試験

A browser-based JLPT N5 practice exam that generates unique questions
every time from live vocabulary data. No backend required.

## 🔗 Live Demo
👉 **[Take the exam here](https://<username>.github.io/jlpt-n5-mock-exam/)**

> Replace `<username>` with your GitHub username after deployment.

## Features
- 35 dynamically generated questions (Vocabulary, Grammar, Reading)
- All content fetched live from public JLPT APIs — zero hardcoded questions
- Fisher-Yates randomization — different exam every refresh
- Timed exam with progress tracking
- Full score breakdown with per-question review and explanations
- Keyboard accessible (arrow keys, A/B/C/D shortcuts)
- Mobile responsive

## How It Works
1. On page load, fetches N5 vocabulary from public APIs
2. Categorizes words into nouns, verbs, adjectives using heuristics
3. Generates 15 vocabulary + 12 grammar + 8 reading questions
4. Each question's content (text, options, explanations) is built
   entirely from fetched word data at runtime

## Deploy Your Own
1. Fork this repository
2. Go to **Settings → Pages**
3. Under "Source", select **GitHub Actions**
4. The site deploys automatically on every push to `main`
5. Access at `https://<your-username>.github.io/jlpt-n5-mock-exam/`

## Tech Stack
- HTML5 + CSS3 + Vanilla JavaScript
- No frameworks, no build tools, no dependencies
- Fetches data from: jlpt-vocab-api.vercel.app (with fallbacks)

## License
MIT
