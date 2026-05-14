# JL Portfolio — Project Context

## Owner
John Lexus Hinolan (JL) — Freelance video producer, editor & content strategist.

## Live Site
https://johnlexus.github.io/Portfolio/

## Local Dev Server
Start with: `preview_start` → "Portfolio - Node Server (port 3000)"
Server script lives at: `D:\Portfolio building\serve-portfolio.js`
Preview at: http://localhost:3000

**Workflow rule:** Always preview locally first → ask "Ready to push live?" → only push on confirmation.

## File Structure
- `index.html` — entire site (all CSS, HTML, JS in one file)
- `.claude/launch.json` — dev server config
- `D:\Portfolio building\serve-portfolio.js` — Node HTTP server script

## Tech Stack
- Pure HTML/CSS/JS — no frameworks
- GitHub Pages hosting (repo: github.com/JohnLexus/Portfolio, branch: main)
- Git remote: https://github.com/JohnLexus/Portfolio.git
- Push command: `git push origin master:main`

## Design Tokens (CSS variables)
```
--black:#080405  --off:#0D0608   --card:#140809  --card2:#1A0B0E
--b1:#28101A     --b2:#3A1826    --burg:#6B1929  --white:#F0EBE2
--mu:#5C484D     --mu2:#8A7A7F   --pop:#C8A03C   (champagne gold)
--fd:'Bebas Neue'  --fb:'Outfit'  --fm:'Space Mono'
```

## Key Sections
- Hero with parallax (heroGrid + heroGlow divs, RAF-throttled scroll)
- About, Services, Work (YouTube lite embeds — click to load)
- Testimonials (2×2 grid — Shane Riggs, Vincent Infante, + 2 others)
- Packages (tabbed: Podcast Production / Personal Brand Growth)
  - Horizontal .pkg-row layout (280px left panel + flex right panel)
  - Prices: $200, $400, $650, $700, $1,100, $1,200
- FAQ, Contact

## Important Notes
- `index.html` path has spaces — use PowerShell for all file edits:
  `[System.IO.File]::WriteAllText('D:\Portfolio building\Porfolio Website\index.html', $content)`
- Node.js may have spaces in path on Windows — use 8.3 short path if needed:
  `C:\PROGRA~1\nodejs\node.exe`
- Git identity: johnlexus.hinolan@gmail.com / John Lexus Hinolan
