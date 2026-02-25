# btm-interactive

Interactive figures for [Beyond the Metric](https://beyondthemetric.ca). Hosted via GitHub Pages.

## Setup

1. Create repo `btm-interactive` on GitHub
2. Push this folder
3. Enable GitHub Pages: **Settings → Pages → Source: Deploy from branch → `main` / `/ (root)`**
4. Your base URL will be: `https://<username>.github.io/btm-interactive/`

## Structure

```
btm-interactive/
├── index.html                          # Landing page
├── biathlon/
│   ├── fig1-speed-accuracy.html        # The Autonomic Frontier — Fig 1
│   ├── fig2-gold-profiles.html         # The Autonomic Frontier — Fig 2
│   ├── fig3-robustness.html            # The Autonomic Frontier — Fig 3
│   ├── fig4-fatigue.html               # The Autonomic Frontier — Fig 4
│   └── fig5-determinants.html          # The Autonomic Frontier — Fig 5
└── entropy/
    └── fig1-archetypes.html            # The Concentration Trap — Fig 1
```

## Ghost Embed Snippets

In Ghost, use an **HTML card** (not markdown) and paste the iframe. Replace `YOUR_USERNAME` with your GitHub username.

### The Autonomic Frontier (biathlon post)

**Fig 1 — Speed vs Accuracy scatter**
```html
<iframe src="https://YOUR_USERNAME.github.io/btm-interactive/biathlon/fig1-speed-accuracy.html" 
  width="100%" height="620" frameborder="0" loading="lazy"
  style="border:1px solid #1a1f2b; border-radius:8px; background:#0a0e14;">
</iframe>
```

**Fig 2 — Gold Medalist Profiles**
```html
<iframe src="https://YOUR_USERNAME.github.io/btm-interactive/biathlon/fig2-gold-profiles.html" 
  width="100%" height="520" frameborder="0" loading="lazy"
  style="border:1px solid #1a1f2b; border-radius:8px; background:#0d1117;">
</iframe>
```

**Fig 3 — Robustness ladder**
```html
<iframe src="https://YOUR_USERNAME.github.io/btm-interactive/biathlon/fig3-robustness.html" 
  width="100%" height="550" frameborder="0" loading="lazy"
  style="border:1px solid #1a1f2b; border-radius:8px; background:#0a0e14;">
</iframe>
```

**Fig 4 — Fatigue degradation**
```html
<iframe src="https://YOUR_USERNAME.github.io/btm-interactive/biathlon/fig4-fatigue.html" 
  width="100%" height="550" frameborder="0" loading="lazy"
  style="border:1px solid #1a1f2b; border-radius:8px; background:#0a0e14;">
</iframe>
```

**Fig 5 — Race determinants**
```html
<iframe src="https://YOUR_USERNAME.github.io/btm-interactive/biathlon/fig5-determinants.html" 
  width="100%" height="580" frameborder="0" loading="lazy"
  style="border:1px solid #1a1f2b; border-radius:8px; background:#0a0e14;">
</iframe>
```

### The Concentration Trap (entropy post)

**Fig 1 — Offensive Archetypes**
```html
<iframe src="https://YOUR_USERNAME.github.io/btm-interactive/entropy/fig1-archetypes.html" 
  width="100%" height="780" frameborder="0" loading="lazy"
  style="border:1px solid #1a1f2b; border-radius:8px; background:#080b10;">
</iframe>
```

## Notes

- All biathlon figures are mobile-responsive (scales fonts, margins, labels, hides toolbar on mobile)
- Fig 2 (gold profiles) is pure HTML/CSS/JS — no Plotly dependency
- The archetypes figure (entropy/fig1) uses pure D3.js with no library imports
- `loading="lazy"` defers iframe load until scrolled into view
- Adjust `height` values if needed after testing in Ghost preview
