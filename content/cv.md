---
title: 'CV'
date: 2026-08-09
type: landing

design:
  spacing: '5rem'

# Note: `username` refers to the author profile in `data/authors/`
#
# The `resume-skills` and `resume-languages` blocks were removed deliberately: they render
# self-rated proficiency as percentage bars and rings ("Python 100%", "Mandarin 20%"), which
# reads badly on an academic CV. The underlying `skills:` and `languages:` data is still in
# data/authors/me.yaml, so re-adding either block is a two-line change if ever wanted.

# Page sections
sections:
  - block: resume-experience
    content:
      username: me
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
---
