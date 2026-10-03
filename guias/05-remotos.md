# 05 — Remotos

## Ver remotos

```bash
git remote -v
```

## Agregar origin

```bash
git remote add origin https://github.com/USUARIO/REPOSITORIO.git
```

## Cambiar URL

```bash
git remote set-url origin https://github.com/USUARIO/NUEVO.git
```

## Descargar información sin mezclarla

```bash
git fetch origin
```

## Ver diferencias contra remoto

```bash
git log HEAD..origin/main --oneline
```

## Actualizar rama

```bash
git pull
```

Una opción que mantiene historial lineal:

```bash
git pull --rebase
```

## Primer push de una rama

```bash
git push -u origin mi-rama
```

Luego bastará normalmente con:

```bash
git push
```

## Ver upstream

```bash
git branch -vv
```
