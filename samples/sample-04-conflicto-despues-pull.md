# Sample 04 — Conflicto después de pull

## 1. Inspecciona

```bash
git status
```

## 2. Abre cada archivo conflictivo

Busca:

```text
<<<<<<<
=======
>>>>>>>
```

Conserva manualmente la versión correcta.

## 3. Marca como resuelto

```bash
git add archivo.md
```

## 4. Continúa

Si era merge:

```bash
git commit
```

Si era rebase:

```bash
git rebase --continue
```
