---
title: Publications
date: 2026-08-09
type: landing

design:
  spacing: '3rem'

sections:
  - block: markdown
    content:
      title: ''
      text: |-
        <style>
        .publist .pub{display:flex;gap:1.25rem;align-items:flex-start;margin:0 0 1.75rem}
        /* Emoji match the favicons on each paper's project page: 🍺 formal-ale, 📐 beyond-l2.
           Explicit emoji font stack so they render in colour rather than as glyph outlines. */
        .publist .icon{flex:0 0 3rem;width:3rem;font-size:2.25rem;line-height:1.2;
          text-align:center;user-select:none;
          font-family:"Apple Color Emoji","Segoe UI Emoji","Noto Color Emoji",
            "Twemoji Mozilla",sans-serif}
        /* margin:0 is required — Tailwind `prose` gives img a 2em top margin, which pushes
           the logo down to the bottom of the entry instead of aligning it with the title. */
        .publist .icon img{width:100%;height:auto;display:block;margin:0}
        .publist .meta{flex:1 1 auto;min-width:0}
        .publist .t{font-weight:700;line-height:1.35;margin-bottom:.15rem}
        .publist .a{font-size:.94em;opacity:.85;margin-bottom:.1rem}
        .publist .v{font-size:.94em;font-style:italic;opacity:.85;margin-bottom:.35rem}
        .publist .l{font-size:.9em}
        .publist .l a{margin-right:.75rem;white-space:nowrap}
        .publist h3{margin:0 0 1.25rem;padding-bottom:.35rem;
          border-bottom:1px solid rgba(120,120,120,.25)}
        .publist .yr{margin-top:2.5rem}
        @media(max-width:640px){.publist .icon{flex-basis:2.25rem;width:2.25rem;font-size:1.6rem}}
        </style>

        <div class="publist">

        <p>Also on <a href="https://scholar.google.com/citations?user=1Qctec0AAAAJ">Google Scholar</a> and <a href="https://orcid.org/0009-0009-6730-7406">ORCID</a>.</p>

        <h3>2026</h3>

        <div class="pub">
          <div class="icon" aria-hidden="true">📐</div>
          <div class="meta">
            <div class="t">Beyond $L_2$: Generalizing Abductive Latent Explanations to Diverse Prototype-Based Architectures</div>
            <div class="a">Jules Soria, Alban Grastien, Romain Xu-Darme, Julien Girard-Satabin, Zakaria Chihani, Daniela Cancila</div>
            <div class="v">ECML PKDD 2026 &middot; Naples, Italy</div>
            <div class="l">
              <a href="https://beyond-l2.github.io/">project page</a>
              <a href="https://github.com/julsoria/beyond_l2">code</a>
            </div>
          </div>
        </div>

        <div class="pub">
          <div class="icon" aria-hidden="true">🍺</div>
          <div class="meta">
            <div class="t">Formal Abductive Latent Explanations for Prototype-Based Networks</div>
            <div class="a">Jules Soria, Zakaria Chihani, Julien Girard-Satabin, Alban Grastien, Romain Xu-Darme, Daniela Cancila</div>
            <div class="v">AAAI 2026, Main Technical Track &middot; Singapore</div>
            <div class="l">
              <a href="https://formal-ale.github.io/">project page</a>
              <a href="https://arxiv.org/abs/2511.16588">arXiv</a>
              <a href="https://github.com/julsoria/ale">code</a>
              <a href="https://zenodo.org/records/16707325">models</a>
            </div>
          </div>
        </div>

        <h3 class="yr">2025</h3>

        <div class="pub">
          <div class="icon" aria-hidden="true"></div>
          <div class="meta">
            <div class="t">Towards Abductive Latent Explanations</div>
            <div class="a">Jules Soria, Zakaria Chihani, Julien Girard-Satabin, Alban Grastien, Romain Xu-Darme, Daniela Cancila</div>
            <div class="v">TRUST-AI workshop at ECAI 2025 &middot; Bologna, Italy &middot; CEUR-WS vol. 4132, 188–199</div>
            <div class="l">
              <a href="https://ceur-ws.org/Vol-4132/short34.pdf">pdf</a>
            </div>
          </div>
        </div>

        <h3 class="yr">2024</h3>

        <div class="pub">
          <div class="icon"><img src="/media/yago-mark.png" alt="YAGO project logo" loading="lazy"></div>
          <div class="meta">
            <div class="t">YAGO 4.5: A Large and Clean Knowledge Base with a Rich Taxonomy</div>
            <div class="a">Fabian M. Suchanek, Mehwish Alam, Thomas Bonald, Lihu Chen, Pierre-Henri Paris, Jules Soria</div>
            <div class="v">SIGIR 2024 &middot; Washington DC, USA &middot; 131–140</div>
            <div class="l">
              <a href="https://suchanek.name/work/publications/sigir-2024.pdf">pdf</a>
              <a href="https://doi.org/10.1145/3626772.3657876">doi</a>
              <a href="https://yago-knowledge.org/">YAGO project</a>
            </div>
          </div>
        </div>

        </div>
    design:
      width: wide
      columns: '1'
---
