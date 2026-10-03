# 09 — Tags

Los tags son útiles para marcar versiones estables o puntos importantes.

## Crear tag ligero

```bash
git tag v1.0.0
```

## Crear tag anotado

```bash
git tag -a v1.0.0 -m "Primera versión estable"
```

## Ver tags

```bash
git tag
```

## Subir uno

```bash
git push origin v1.0.0
```

## Subir todos

```bash
git push origin --tags
```

## Borrar local

```bash
git tag -d v1.0.0
```

## Borrar remoto

```bash
git push origin --delete v1.0.0
```
