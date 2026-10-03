# Sample 03 — Deshacer un commit ya publicado

Si el commit ya llegó al remoto y otras personas pueden haberlo descargado, crea un commit inverso.

```bash
git log --oneline
```

Luego:

```bash
git revert <hash>
```

Finalmente:

```bash
git push
```

Ventaja: no reescribe el historial existente.
