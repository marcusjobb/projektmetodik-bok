# projektmetodik-bok

## Länkar mellan sidor

Skriv interna länkar **relativt till källfilen**, med `.md` — som du skulle göra i VS Code eller på GitHub:

```markdown
[Kanban](kanban.md)                            <!-- samma mapp -->
[Scrum](../agilt/scrum.md)                     <!-- annan avdelning -->
[Agilt](../agilt/index.md)                     <!-- en avdelnings index -->
[Rubrik](kanban.md#varför-en-wip-gräns)         <!-- med ankare -->
```

Pluginet `site/src/plugins/doc-links.mjs` gör om dem till rätt absoluta URL:er vid bygget.

Skriv **inte** länkar utifrån den publicerade URL:en (`../kanban/`, `kanban/`) — de räknas från fel mapp och blir trasiga.

Kontrollera innan commit: `npm run check:links`. CI kör samma kontroll och stoppar deployen om någon länk är trasig.
