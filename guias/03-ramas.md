# 03 — Ramas

## Ver ramas

```bash
git branch
```

Todas las ramas, incluidas remotas:

```bash
git branch -a
```

## Crear una rama

```bash
git branch nueva-funcionalidad
```

## Crear y cambiar a la nueva rama

```bash
git switch -c nueva-funcionalidad
```

## Cambiar de rama

```bash
git switch main
```

## Renombrar la rama actual

```bash
git branch -m nuevo-nombre
```

## Borrar una rama ya fusionada

```bash
git branch -d nombre-rama
```

## Forzar borrado de una rama local

```bash
git branch -D nombre-rama
```

## Borrar una rama remota

```bash
git push origin --delete nombre-rama
```

## Crear una rama de rescate desde un commit

```bash
git switch -c rescate <hash>
```
