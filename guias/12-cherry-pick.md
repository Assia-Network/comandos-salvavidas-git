# 12 — Cherry-pick

`git cherry-pick` permite aplicar uno o más commits concretos sobre la rama actual.

## Aplicar un commit

```bash
git cherry-pick <hash>
```

## Aplicar varios commits

```bash
git cherry-pick <hash1> <hash2>
```

## Si aparece un conflicto

```bash
git status
```

Resuelve los archivos, márcalos y continúa:

```bash
git add <archivo>
git cherry-pick --continue
```

## Cancelar la operación

```bash
git cherry-pick --abort
```

## Cuándo conviene

- mover una corrección puntual entre ramas;
- rescatar un commit útil sin fusionar toda una rama;
- aplicar un hotfix concreto.

Evita usarlo indiscriminadamente sobre cambios que ya existen en la rama, porque puedes duplicar modificaciones o generar conflictos innecesarios.
