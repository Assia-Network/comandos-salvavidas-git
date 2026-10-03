# 11 — GitHub y contribuciones

GitHub muestra en el perfil actividad de contribución, repositorios destacados y logros asociados a acciones concretas realizadas en la plataforma.

## Actividad que puede aparecer en el perfil

Según la documentación oficial de GitHub, acciones como crear repositorios o hacer forks cuentan como contribuciones; otras, como commits, issues, pull requests, revisiones y discusiones, cuentan cuando cumplen sus criterios de atribución.

## Recomendación para este repositorio

En vez de crear actividad artificial, úsalo como un proyecto real y evolutivo:

1. crea el repositorio;
2. sube una primera versión funcional;
3. abre issues para comandos o casos que falten;
4. trabaja cada mejora en su propia rama;
5. crea pull requests para incorporar cambios;
6. revisa y documenta cada incorporación;
7. publica versiones con tags cuando el contenido alcance hitos reales.

Esto deja un historial útil y comprensible para cualquiera que visite el proyecto.

## Identidad de commits

Comprueba tu configuración:

```bash
git config user.name
git config user.email
```

Para configurar:

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu-correo@example.com"
```

El correo debe coincidir con uno asociado a tu cuenta de GitHub para que la atribución funcione correctamente, salvo que uses la dirección `noreply` proporcionada por GitHub.
