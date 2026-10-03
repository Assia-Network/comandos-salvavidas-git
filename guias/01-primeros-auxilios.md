# 01 — Primeros auxilios Git

Cuando algo sale mal, no empieces con `reset --hard`. Primero identifica el estado real del repositorio.

## 1. Ver el estado

```bash
git status
```

Te dice:
- rama actual;
- archivos modificados;
- archivos en staging;
- conflictos;
- si estás adelantado o atrasado respecto al remoto.

## 2. Ver los últimos commits

```bash
git log --oneline --decorate --graph -10
```

Versión ampliada:

```bash
git log --all --oneline --decorate --graph
```

## 3. Saber en qué rama estás

```bash
git branch --show-current
```

## 4. Ver diferencias sin guardar

```bash
git diff
```

Para cambios que ya están en staging:

```bash
git diff --staged
```

## 5. Crear un respaldo antes de experimentar

```bash
git branch respaldo-antes-de-arreglar
```

O guardar cambios no confirmados:

```bash
git stash push -u -m "respaldo temporal"
```

## 6. Ver qué comando podría ayudarte

| Problema | Primera herramienta |
|---|---|
| Modifiqué un archivo y quiero descartarlo | `git restore` |
| Agregué algo a staging por error | `git restore --staged` |
| Quiero corregir el último commit | `git commit --amend` |
| Quiero deshacer un commit público | `git revert` |
| Perdí un commit | `git reflog` |
| Necesito cambiar de rama con cambios locales | `git stash` |
| Tengo conflictos | `git status` + resolución manual |

## Regla práctica

Si el commit ya fue compartido con otras personas, suele ser más seguro usar `git revert` que reescribir el historial.
