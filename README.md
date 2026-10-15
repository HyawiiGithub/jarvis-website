# JARVIS — website

Public docs site for Jarvis, the AI inside the USSR economy Discord bot.
Static HTML + one stylesheet. No build step, no tracking, no sources cited.

## Pages

- `index.html` — what Jarvis is, feature cards, try-it lines
- `how-it-works.html` — hear → context → answer → autonomy → bug loop → limits
- `models.html` — the real provider/model chain, retired slugs, free-tier reality
- `commands.html` — every command Jarvis may mention, bug desk, power words, setup
- `setup.html` — env keys, PM2 deploy, per-server toggles, troubleshooting
- `style.css` — shared theme

## Preview locally

```sh
cd jarvis-website
python3 -m http.server 8080
# open http://localhost:8080
```

## Publish (GitHub Pages)

1. New repo, push this folder's contents to `main`.
2. Repo Settings → Pages → Deploy from branch → `main` / root.
3. Site goes live at `https://<you>.github.io/<repo>/`.

## Notes

- The model list mirrors the bot's actual failover chain. If the chain in
  `bot.js` changes, update `models.html` to match.
- The command list mirrors the bot's real commands. Same rule for
  `commands.html`.
- Everything here describes this bot only.
