# RPSC Hindi Guru – 2nd Grade Teacher Test Series

Free, open-source, mobile-first test series for **RPSC Senior Teacher (Grade-II) Hindi – Secondary Education**.

Live: GitHub Pages ready. Just enable Pages → Deploy from `main` / `/root`.

### Features
- 1200+ PYQ-pattern practice questions (20 modules × 60 Q)
- Paper I + Paper II full syllabus coverage
- Topic-wise tests (20 Q / Full)
- Full Mock: Paper II – 150 Q, 150 min, 300 marks • Paper I – 100 Q, 120 min, 200 marks
- RPSC real scoring: **+2 correct, -0.66 wrong**
- OMR sheet view, detailed review
- Hinglish UI, Dark mode
- Progress tracker, history, bookmarks, mark-for-review
- Funny result messages (Hindi) – motivate / scold 😄
- Offline PWA, 100% LocalStorage – no login, no backend
- PYQ Importer – paste your own JSON/CSV questions, merges into tests
- Mobile + Desktop responsive, < 150KB app shell

### Syllabus Covered

**Paper II – Hindi**
1. Varn Vichar
2. Shabd Vargikaran (Tatsam/Tadbhav)
3. Sangya / Sarvanam / Visheshan / Kriya
4. Ling, Vachan, Karak, Kaal
5. Sandhi, Samas, Upsarg, Pratyay
6. Paryayvachi / Vilom
7. Vakya Rachna / Shuddhi
8. Muhavare / Lokoktiyan
9. Kavya Shastra – Shabd Shakti, Gun, Dosh
10. Alankar, Chhand, Ras
11. Hindi Sahitya Itihas – Aadi / Bhakti / Reeti Kaal
12. Aadhunik Sahitya
13. Hindi Bhasha Udbhav, Boliyan, Lipi
14. Nirdharit Paath – Kabir, Tulsi, Sur, Meera, Bihari
15. Aadhunik Gadya/Padya – Godan, Kamayani, Kurukshetra, Chintamani…
16. Hindi Shikshan Vidhiyan

**Paper I – General Studies**
17. Rajasthan GK
18. Rajasthan Current Affairs (placeholder – update monthly)
19. World / India GK – Constitution, Economy, Geography
20. Educational Psychology

> Questions are **PYQ-pattern practice questions**, modelled on RPSC 2011–2022 papers. They are NOT verbatim PYQs. Use the built-in **Import PYQ** tool to merge real PYQs.

### Deploy to GitHub Pages
1. Push this folder to a repo: `rpsc-hindi-guru`
2. Settings → Pages → Source: GitHub Actions
3. Workflow at `.github/workflows/pages.yml` auto-deploys on push.

Or: Settings → Pages → Branch: main / root – done.

### Add / Expand Questions
- Edit `generate_questions_v2.py` – add more Qs to the banks, run: `python3 generate_questions_v2.py`
- Or use the in-app **Import PYQ** button: paste JSON `[{"q":"...","options":["A","B","C","D"],"answer":0,"explanation":"","topic":""}]`
- Custom imported Qs are stored in localStorage and included in Speed/Random tests.
- JSON files live in `/data/*.json` – 20 module files, easy to replace.

### Tech
- Pure HTML + Tailwind CDN + Vanilla JS
- No build step, no framework, no backend
- PWA ready – `manifest.json` + `sw.js`
- 100% static – works on GitHub Pages / Vercel / Netlify

### License
by Hitesh for all free for students, teachers.

Made with ❤️ for RPSC 2nd Grade Hindi aspirants.
