# Loma survey

The founding-member survey, as one self-contained page.

It is here, rather than in the app, for one reason: the link has to outlive
every machine any of us owns. No build step, no server, no deploy. GitHub
Pages serves the file and answers go straight to Supabase with the project's
publishable key, which is the same key the app already ships in its own client
bundle. There is no secret in this repository.

- `index.html` — the whole thing: markup, styling, the synthesised chime, and
  the write.
- `img/` — the photography behind each screen.

`?at=niches` (or `name`, `email`, `mvp`, `catalogue`, `spend`, `trips`, `done`)
opens one screen on its own, so a single question can go round for feedback
without anyone answering their way to it.

Answers land in `concierge_requests` under kind `survey_v1` and are read at
`/admin/survey` in the app.
