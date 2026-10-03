# 04 — Stash: guardar cambios temporalmente

`stash` permite limpiar temporalmente tu working tree sin crear un commit definitivo.

## Guardar cambios

```bash
git stash push -m "trabajo temporal"
```

## Incluir archivos no rastreados

```bash
git stash push -u -m "incluye archivos nuevos"
```

## Ver stashes

```bash
git stash list
```

## Recuperar el último stash y eliminarlo de la lista

```bash
git stash pop
```

## Aplicar sin eliminarlo

```bash
git stash apply stash@{0}
```

## Ver el contenido

```bash
git stash show -p stash@{0}
```

## Eliminar uno

```bash
git stash drop stash@{0}
```

## Crear una rama desde un stash

```bash
git stash branch rescate-stash stash@{0}
```
