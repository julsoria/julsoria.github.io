---
title: Talks
date: 2026-11-02
type: landing

design:
  spacing: '3rem'

# ─── HOW TO ADD A TALK ────────────────────────────────────────────────────────────────
#   {{< talk title="Paper or talk title"
#            venue="Venue &middot; City &middot; Month Year"
#            slides="2026-09-filename.pdf" >}}
#
#   slides   optional. Filename only; the file goes in static/uploads/slides/.
#            Compress first:  gs -sDEVICE=pdfwrite -dPDFSETTINGS=/ebook \
#                                -dNOPAUSE -dQUIET -dBATCH -sOutputFile=out.pdf in.pdf
#   kind     optional. kind="poster" labels the link "poster" instead of "slides".
#   note     optional. Shown in brackets after the title, e.g. note="poster".
#   Year headings:  {{< yr title="2025" >}}   (add first="true" on the topmost one)
#   Mirror any change in content/fr/talks.md.
#
# Every title and venue here is read off the actual slide deck. Do not add an entry whose
# title has not been read from its deck.
# TODO (Jules): two decks still have no venue, so they are NOT listed —
#   ~/Documents/0_PRESENTATIONS/3_SORIA.pdf                  (Nov 2025)
#   ~/Documents/0_PRESENTATIONS/LSLauVert25_Presentation.pdf (Dec 2025)
# ──────────────────────────────────────────────────────────────────────────────────────

sections:
  - block: markdown
    content:
      title: ''
      text: |-
        <div class="entries">

        {{< yr title="2026" first="true" >}}

        {{< talk title="Beyond $L_2$: Generalizing Abductive Latent Explanations to Diverse Prototype-Based Architectures"
                 venue="ECML PKDD 2026, Research Track &middot; Naples &middot; 7–11 September 2026"
                 slides="2026-09-ecml-pkdd-beyond-l2.pdf" >}}

        {{< talk title="Formal Abductive Latent Explanations for Prototype-Based Networks"
                 venue="CAp &amp; RFIAP 2026 &middot; Montpellier &middot; July 2026" >}}

        {{< talk title="Formal Abductive Latent Explanations for Prototype-Based Networks"
                 venue="NeuroSym4MLLM × EXPLAIN'AI workshop &middot; June 2026"
                 slides="2026-06-neurosym4mllm-explainai.pdf" >}}

        {{< talk title="Formal Abductive Latent Explanations for Prototype-Based Networks"
                 venue="NormaSTIC seminar on explainability &middot; Rouen &middot; May 2026"
                 slides="2026-05-normastic-formal-ale.pdf" >}}

        {{< talk title="Formal Abductive Latent Explanations for Prototype-Based Networks"
                 note="poster" kind="poster"
                 venue="CEA List Days &middot; Palaiseau &middot; May 2026"
                 slides="2026-05-cea-list-days-poster.pdf" >}}

        {{< talk title="Formal Abductive Latent Explanations for Prototype-Based Networks"
                 venue="AAAI 2026, Main Technical Track &middot; Singapore &middot; January 2026" >}}

        {{< yr title="2025" >}}

        {{< talk title="Towards Abductive Latent Explanations"
                 venue="TRUST-AI workshop at ECAI 2025 &middot; Bologna &middot; October 2025"
                 slides="2025-10-trust-ai-ecai-towards-ale.pdf" >}}

        {{< talk title="Explications de confiance pour l'intelligence artificielle"
                 venue="Journée des Thèses DILS, CEA List &middot; Palaiseau &middot; 20 &amp; 27 June 2025"
                 slides="2025-06-journee-des-theses.pdf" >}}

        {{< yr title="2024" >}}

        {{< talk title="Crafting Adversarial Examples Using Linear Regions"
                 venue="Workshop Fondements Mathématiques de l'IA &middot; 17 June 2024"
                 slides="2024-06-fondements-adversarial-linear-regions.pdf" >}}

        {{< talk title="Explications de confiance pour l'intelligence artificielle"
                 venue="Journée des Thèses DILS, CEA List &middot; Palaiseau &middot; 27–28 June 2024"
                 slides="2024-06-journee-des-theses.pdf" >}}

        {{< yr title="Other venues" >}}

        <div class="note">
          Also presented at the <strong>P-AI FM</strong> workshop, at <strong>PEPR SAIF</strong>
          project meetings, and to the working groups <strong>GT ECLAIRE</strong>,
          <strong>GT EXPLICON</strong> and <strong>GT XAI4U</strong> (Calais 2024,
          Toulouse 2025).
        </div>

        </div>
    design:
      width: wide
      columns: '1'
---
