# Contribuir

Gracias por mejorar **Comandos Salvavidas Git**.

## Formas de contribuir

- corregir un comando;
- mejorar una explicación;
- agregar un caso real;
- añadir una advertencia de seguridad;
- crear una nueva guía.

## Flujo sugerido

```bash
git switch -c docs/nueva-guia
```

Haz cambios y revisa:

```bash
git status
git diff
```

Crea el commit:

```bash
git add .
git commit -m "docs: agrega guía sobre cherry-pick"
```

Después abre un Pull Request describiendo:
- problema que resuelve;
- comandos incluidos;
- riesgos o advertencias;
- ejemplo de uso.

## Estilo

- Explicaciones en español claro.
- Comandos dentro de bloques `bash`.
- Advertencias visibles para comandos destructivos.
- Evitar ejemplos con credenciales reales.
