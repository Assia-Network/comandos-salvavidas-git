# Sample 05 — Perdí un commit después de reset

Ejecutaste un reset y el commit ya no aparece en `git log`.

## 1. Mira el reflog

```bash
git reflog
```

Ejemplo:

```text
12ab34c HEAD@{0}: reset: moving to HEAD~1
98de76f HEAD@{1}: commit: trabajo importante
```

## 2. Crea una rama desde el commit perdido

```bash
git switch -c rescate 98de76f
```

Ahora el commit vuelve a estar referenciado por una rama.
