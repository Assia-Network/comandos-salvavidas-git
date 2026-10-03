# 10 — Buenas prácticas

## Haz commits pequeños y comprensibles

Mejor:

```text
fix: corrige validación de correo
```

Que:

```text
cambios varios finales ahora sí
```

## Revisa antes de confirmar

```bash
git status
git diff
git diff --staged
```

## Usa ramas para cambios independientes

```bash
git switch -c feat/nueva-funcion
```

## Sincroniza antes de empezar una sesión

```bash
git fetch origin
git status
```

## Evita subir secretos

No publiques:
- contraseñas;
- tokens;
- claves privadas;
- archivos `.env` con credenciales;
- datos personales innecesarios.

Si un secreto ya fue publicado, borrarlo en un commit nuevo no garantiza que desaparezca del historial. Debe rotarse la credencial y, si corresponde, limpiar el historial.

## Usa `--force-with-lease` antes que `--force`

Si realmente necesitas reescribir una rama remota:

```bash
git push --force-with-lease
```

Es más seguro porque evita sobrescribir cambios remotos inesperados.
