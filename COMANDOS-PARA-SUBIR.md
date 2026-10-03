# Comandos para subir este repositorio a GitHub

Después de crear un repositorio vacío llamado `comandos-salvavidas-git` en GitHub:

```bash
cd comandos-salvavidas-git
git init
git add .
git commit -m "docs: publica primera versión de comandos salvavidas Git"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/comandos-salvavidas-git.git
git push -u origin main
```

## Para continuar mejorándolo

Crear rama:

```bash
git switch -c docs/nueva-guia
```

Guardar cambios:

```bash
git add .
git commit -m "docs: agrega nuevo caso práctico"
git push -u origin docs/nueva-guia
```

Luego puedes abrir un Pull Request desde GitHub y fusionarlo cuando la mejora esté lista.
