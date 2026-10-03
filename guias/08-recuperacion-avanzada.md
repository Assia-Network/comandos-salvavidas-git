# 08 — Recuperación avanzada

## El salvavidas principal: reflog

```bash
git reflog
```

Muestra movimientos recientes de `HEAD`, incluso si un commit dejó de aparecer en `git log`.

Ejemplo:

```text
8fd123a HEAD@{0}: reset: moving to HEAD~2
4ab778c HEAD@{1}: commit: versión buena
```

Puedes recuperar el commit con:

```bash
git switch -c rescate 4ab778c
```

## Recuperar un archivo de otro commit

```bash
git restore --source=<hash> -- ruta/al/archivo
```

## Buscar objetos no referenciados

```bash
git fsck --lost-found
```

Úsalo como último recurso cuando `reflog` no basta.

## Inspeccionar un commit

```bash
git show <hash>
```

## Crear una rama antes de probar una recuperación

```bash
git branch respaldo-recuperacion
```
