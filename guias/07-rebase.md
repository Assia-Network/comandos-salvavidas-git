# 07 — Rebase

`rebase` mueve commits para reconstruir una historia lineal. Es potente, pero puede reescribir hashes.

## Rebase básico

```bash
git switch feature
git rebase main
```

## Si hay conflicto

Resuelve el archivo y luego:

```bash
git add archivo
git rebase --continue
```

## Saltar un commit conflictivo

```bash
git rebase --skip
```

## Cancelar

```bash
git rebase --abort
```

## Rebase interactivo

```bash
git rebase -i HEAD~5
```

Acciones habituales:
- `pick`: conservar;
- `reword`: cambiar mensaje;
- `squash`: combinar con el anterior;
- `fixup`: combinar descartando el mensaje;
- `drop`: eliminar.

## Regla de seguridad

Evita reescribir ramas públicas compartidas, salvo que el equipo lo haya acordado.
