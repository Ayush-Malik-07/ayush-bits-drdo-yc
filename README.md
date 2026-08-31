# Ayush Malik — Interactive Resume

Single-file animated resume site. No build step, no dependencies, no framework.

**Live:** https://ayush-malik-07.github.io/ayush-bits-drdo-yc/

## Before pushing

Export the current resume from Overleaf as PDF and save it in this folder as
exactly `Ayush_Malik_Resume.pdf`. Both "Download ATS-friendly PDF" buttons on
the site link to that filename.

## Deploy (GitHub Pages)

1. Create a **public** repo named `ayush-bits-drdo-yc` under Ayush-Malik-07
2. From this folder:
   ```
   git init && git add -A && git commit -m "interactive resume"
   git branch -M main
   git remote add origin https://github.com/Ayush-Malik-07/ayush-bits-drdo-yc.git
   git push -u origin main
   ```
3. Settings -> Pages -> Source: `main` / root. Live in about a minute.

## Custom domain (optional, later)

Buy a domain, then `echo "ayushmalik.dev" > CNAME`, commit, and point DNS
A records at the GitHub Pages IPs (185.199.108-111.153). The PDF link is
relative, so it keeps working after the move.

## Notes

- Everything is in `index.html` (~46 KB): CSS, JS, SVG, canvas animations.
- `.nojekyll` stops GitHub from running Jekyll over the files.
