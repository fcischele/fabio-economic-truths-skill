# fabio

Skill per agenti AI: con `/fabio` risponde con una "verità" economica da bar alla Fabio.

> Il reparto pescheria di un supermercato è sempre in perdita economica.

Segue lo standard `SKILL.md`, quindi funziona con Claude Code e con gli altri agenti che supportano le skill.

## Installazione

```bash
# Claude Code, disponibile in tutte le chat
npx skills add fcischele/fabio-economic-truths-skill --skill fabio -g -a claude-code

# tutti gli agenti supportati (Codex, Cursor, Windsurf, ...)
npx skills add fcischele/fabio-economic-truths-skill --skill fabio -g -a '*'
```

Senza `-g` la skill viene installata solo nel progetto corrente.

## Aggiornamento

```bash
npx skills update
```

## Modificare la skill

Tutto è in [`SKILL.md`](SKILL.md): la ricetta per comporre le frasi e gli esempi. Per aggiungere frasi basta aggiungerle alla lista `## Esempi`. Il modello le usa come base e ne inventa di nuove con la stessa vibe.
