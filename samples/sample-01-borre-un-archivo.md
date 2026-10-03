# Sample 01 — Borré un archivo por accidente

## Caso A: todavía no hiciste commit

Comprueba:

```bash
git status
```

Restaura:

```bash
git restore ruta/archivo.md
```

## Caso B: el archivo existía en un commit anterior

Busca el commit:

```bash
git log --oneline -- ruta/archivo.md
```

Restaura desde uno concreto:

```bash
git restore --source=<hash> -- ruta/archivo.md
```
