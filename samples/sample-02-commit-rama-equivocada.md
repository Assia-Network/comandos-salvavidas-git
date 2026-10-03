# Sample 02 — Hice commit en la rama equivocada

Supongamos que hiciste el commit en `main`, pero debía ir a `feature`.

## 1. Guarda el hash

```bash
git log -1 --oneline
```

## 2. Crea la rama correcta desde ese commit

```bash
git branch feature
```

## 3. Si el commit todavía no fue publicado, devuelve `main`

```bash
git reset --hard HEAD~1
```

## 4. Cambia a la rama correcta

```bash
git switch feature
```

Si ya publicaste `main`, evita reescribirlo sin considerar a otros colaboradores; normalmente conviene usar `git revert` en `main`.
