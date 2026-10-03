# 02 — Commits y deshacer cambios

## Quitar un archivo de staging sin borrar sus cambios

```bash
git restore --staged archivo.txt
```

## Descartar cambios locales de un archivo

```bash
git restore archivo.txt
```

> Esto elimina las modificaciones no confirmadas de ese archivo.

## Corregir el mensaje del último commit

```bash
git commit --amend -m "mensaje corregido"
```

## Agregar un archivo olvidado al último commit

```bash
git add archivo_olvidado.py
git commit --amend --no-edit
```

## Deshacer un commit sin reescribir el historial

```bash
git revert <hash>
```

Ideal cuando el commit ya fue publicado.

## Mover HEAD hacia atrás conservando cambios

```bash
git reset --soft HEAD~1
```

El commit desaparece del historial actual, pero los cambios permanecen en staging.

## Mover HEAD hacia atrás y conservar cambios fuera de staging

```bash
git reset HEAD~1
```

Equivale normalmente a `--mixed`.

## Eliminar commit y cambios locales

```bash
git reset --hard HEAD~1
```

⚠️ Destructivo para cambios locales. Si lo ejecutaste por accidente, revisa `git reflog`.
