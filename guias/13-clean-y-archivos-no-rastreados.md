# 13 — `git clean` y archivos no rastreados

`git clean` elimina archivos que Git todavía no está siguiendo. Puede ser útil, pero también puede borrar trabajo que nunca llegó a un commit.

## Primero: simular

```bash
git clean -n
```

Esto muestra lo que se eliminaría sin borrar nada.

## Incluir directorios en la simulación

```bash
git clean -nd
```

## Eliminar archivos no rastreados

```bash
git clean -f
```

## Eliminar también directorios

```bash
git clean -fd
```

## Archivos ignorados

Para ver qué se eliminaría incluyendo archivos ignorados:

```bash
git clean -ndx
```

`-x` puede afectar entornos virtuales, builds y archivos locales incluidos en `.gitignore`, así que úsalo con especial cuidado.

## Recomendación

Ejecuta siempre primero `git clean -n` o `git clean -nd` y revisa la lista antes de usar `-f`.
