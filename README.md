# PomoPanda

Single-file Pomodoro timer with YouTube/Spotify embed support.

Quick deploy instructions

1) Initialize git and push to GitHub:

```bash
git init
git add pomopanda.html README.md
git commit -m "Add PomoPanda"
# create repo on GitHub and add remote, then push
git remote add origin https://github.com/<your-username>/<repo>.git
git push -u origin main
```

2) Deploy to Vercel (recommended):

- Option A: From CLI (fast)

```bash
npm install -g vercel
vercel login
vercel         # follow prompts
vercel --prod  # deploy production
```

- Option B: From Vercel dashboard

Create a new project → import your GitHub repo → Deploy.

Notes & troubleshooting

- Serve over HTTP(S). Vercel provides HTTPS automatically; this avoids file:// iframe restrictions.
- Some YouTube videos disallow embedding — if the embedded player stays blank use the "Open on YouTube" fallback link shown under the player.
- No API keys required for simple iframe embeds. You only need the YouTube/Spotify Web APIs for searching or controlling playback.

If you want, I can create the GitHub repo for you (requires access) or guide you through connecting Vercel to GitHub step-by-step.