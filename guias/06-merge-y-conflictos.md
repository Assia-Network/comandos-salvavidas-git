# 06 — Merge y conflictos

## Fusionar una rama

Desde la rama destino:

```bash
git switch main
git merge feature
```

## Si aparece un conflicto

Primero:

```bash
git status
```

Git marcará archivos como "both modified".

Dentro del archivo aparecerán marcadores similares a:

```text
<<<<<<< HEAD
contenido actual
=======
contenido de la otra rama
>>>>>>> feature
```

Edita el archivo y deja únicamente el resultado correcto.

Después:

```bash
git add archivo_conflictivo.md
git commit
```

## Cancelar el merge

```bash
git merge --abort
```

## Ver archivos en conflicto

```bash
git diff --name-only --diff-filter=U
```
