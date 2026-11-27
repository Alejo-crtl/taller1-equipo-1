# Estándar de codificación - Equipo 1

Lenguaje(s) del proyecto formativo: ...
## 1. Nombrado
(pendiente)
## 2. Formato
(pendiente)
## 3. Comentarios y documentación
(pendiente)
## 4. Estructura de carpetas
(pendiente)

## 5. Git: ramas, commits y pull requests

### Nombres de ramas
Se usa formato `tipo/descripcion-corta` en minúsculas y separado por guiones:
 `main`: rama principal estable (protegida, no se hacen commits directos).
 `feat/nombre-funcionalidad`: nuevas funcionalidades.
 `fix/nombre-error`: corrección de errores.
 `docs/nombre-cambio`: cambios en documentación.
 `chore/nombre-tarea`: configuraciones y mantenimiento.

### Formato de commits
Se sigue el estándar **Conventional Commits** en español, en tiempo presente y sin punto final:
 `feat:` nueva funcionalidad ej. `feat: agrega login de usuarios`
 `fix:` corrección de un error ej. `fix: corrige validación de correo`
 `docs:` documentación ej. `docs: actualiza sección de Git en estándar`
 `style:` formato o indentación sin cambiar lógica
 `refactor:` mejora de código sin cambiar comportamiento
 `chore:` tareas de configuración ej. `chore: agrega archivo .editorconfig`

### Reglas de Pull Requests (PR)
 Todo cambio hacia `main` debe realizarse mediante un Pull Request desde una rama dedicada.
 El título debe ser claro y seguir el formato de commits.
 Si el PR resuelve un issue, debe incluir `Closes #N` en la descripción.
 Requiere al menos 1 revisión y aprobación de otro integrante del equipo antes de hacer merge.
 No se aceptan PR con conflictos pendientes.