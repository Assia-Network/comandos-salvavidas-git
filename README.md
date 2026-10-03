# 🛟 Comandos Salvavidas Git

Repositorio práctico en español con comandos de Git para resolver situaciones reales: deshacer cambios, recuperar commits, trabajar con ramas, arreglar conflictos, usar `stash`, sincronizar remotos y entender qué hacer cuando algo sale mal.

> Objetivo: tener una guía rápida para consultar cuando Git se pone feo.

## 📚 Índice de guías

| Guía | Para qué sirve |
|---|---|
| [01 — Primeros auxilios](guias/01-primeros-auxilios.md) | Diagnosticar antes de tocar nada |
| [02 — Commits y deshacer cambios](guias/02-commits-y-deshacer.md) | `restore`, `reset`, `revert`, `commit --amend` |
| [03 — Ramas](guias/03-ramas.md) | Crear, cambiar, renombrar y borrar ramas |
| [04 — Stash](guias/04-stash.md) | Guardar trabajo temporalmente |
| [05 — Remotos](guias/05-remotos.md) | `fetch`, `pull`, `push`, upstream y origin |
| [06 — Merge y conflictos](guias/06-merge-y-conflictos.md) | Resolver conflictos sin entrar en pánico |
| [07 — Rebase](guias/07-rebase.md) | Reordenar o limpiar historial |
| [08 — Recuperación avanzada](guias/08-recuperacion-avanzada.md) | `reflog`, commits perdidos y rescate |
| [09 — Tags](guias/09-tags.md) | Versiones y puntos de restauración |
| [10 — Buenas prácticas](guias/10-buenas-practicas.md) | Flujo de trabajo más seguro |
| [11 — GitHub y contribuciones](guias/11-github-y-contribuciones.md) | Qué actividad cuenta en tu perfil |
| [12 — Cherry-pick](guias/12-cherry-pick.md) | Aplicar commits concretos entre ramas |
| [13 — Git clean](guias/13-clean-y-archivos-no-rastreados.md) | Limpiar archivos no rastreados con seguridad |
| [Cheatsheet](CHEATSHEET.md) | Resumen rápido de comandos |

## 🧪 Casos prácticos

Los ejemplos completos están en [`samples/`](samples/):

- [Borré un archivo por accidente](samples/sample-01-borre-un-archivo.md)
- [Hice commit en la rama equivocada](samples/sample-02-commit-rama-equivocada.md)
- [Quiero deshacer un commit ya publicado](samples/sample-03-deshacer-commit-publicado.md)
- [Tengo conflictos después de un pull](samples/sample-04-conflicto-despues-pull.md)
- [Perdí un commit después de reset](samples/sample-05-recuperar-commit-reset.md)

## 🚦Regla de oro

Antes de ejecutar comandos destructivos:

```bash
git status
git log --oneline --decorate --graph -10
git branch --show-current
```

Y si tienes dudas, crea una rama de respaldo:

```bash
git branch respaldo-antes-de-arreglar
```

## ⚠️ Comandos con riesgo

Estos comandos pueden eliminar trabajo local o reescribir historial:

```bash
git reset --hard
git clean -fd
git push --force
git rebase
```

No son "malos", pero deben usarse entendiendo qué modifican.

## 🧭 ¿Por dónde empiezo?

- Si **no sabes qué pasó** → [Primeros auxilios](guias/01-primeros-auxilios.md)
- Si **quieres deshacer algo** → [Commits y deshacer cambios](guias/02-commits-y-deshacer.md)
- Si **perdiste commits** → [Recuperación avanzada](guias/08-recuperacion-avanzada.md)
- Si **hay conflictos** → [Merge y conflictos](guias/06-merge-y-conflictos.md)
- Si solo quieres un comando rápido → [CHEATSHEET.md](CHEATSHEET.md)

## 🤝 Contribuciones

Consulta [CONTRIBUTING.md](CONTRIBUTING.md) para proponer nuevos casos, corregir comandos o añadir ejemplos.

## 📄 Licencia

Contenido disponible bajo [MIT](LICENSE.md).

---

Hecho para aprender Git usando problemas reales, no memorizando comandos aislados.
