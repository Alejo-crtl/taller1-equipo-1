# Estándar de codificación - Equipo 1

Lenguaje(s) del proyecto formativo: ...
## 1. Nombrado
(pendiente)
## 2. Formato
(pendiente)
## 3. Comentarios y documentación
## Idea clave

> Comenta el **porqué**, no el **qué**.  
> El código debe explicarse solo; los comentarios aclaran decisiones.

## Cuándo comentar

**Sí comenta:**
- Decisiones raras o no obvias.
- Soluciones temporales (`// HACK: ...`).
- Restricciones importantes.
- Reglas de negocio complejas.

**No comentes:**
- Código obvio: `i++ // suma 1`.
- Código comentado: mejor bórralo, queda en Git.
- Comentarios desactualizados.
- Código mal nombrado: primero refactoriza.

## Documentar funciones

Documenta funciones públicas con:
- Qué hace.
- Parámetros.
- Qué devuelve.
- Errores que lanza.
- Un ejemplo.

Ejemplo JavaScript:

```javascript
/**
 * Calcula el precio total con impuestos y descuento.
 * @param {number} precio - Precio base.
 * @param {number} impuesto - Impuesto en decimal (0.08 = 8%).
 * @returns {number} Precio final.
 */
function calcularTotal(precio, impuesto) {
  return precio * (1 + impuesto);
}
```

Ejemplo Python:

```python
def calcular_total(precio, impuesto):
    """Calcula el precio total con impuestos.

    Args:
        precio (float): Precio base.
        impuesto (float): Impuesto en decimal.

    Returns:
        float: Precio final.
    """
    return precio * (1 + impuesto)
```

## README mínimo

Todo proyecto debe tener un `README.md` con:

1. **Qué es:** nombre y descripción breve.
2. **Para qué sirve:** problema que resuelve.
3. **Cómo se instala:** comandos.
4. **Cómo se usa:** ejemplo básico.
5. **Cómo contribuir:** pasos para fork y Pull Request.

Plantilla corta:

```markdown
# Nombre del Proyecto

Descripción breve del proyecto.

## Instalación

```bash
git clone https://github.com/usuario/proyecto.git
cd proyecto
npm install
```

## Uso

```bash
npm start
```

## Pruebas

```bash
npm test
```

## Licencia

MIT

## 4. Estructura de carpetas
## Estructura recomendada

```text
mi-proyecto/
├── README.md
├── .gitignore
├── LICENSE
├── src/              # Código fuente
├── tests/            # Pruebas
├── docs/             # Documentación
└── .github/          # Configuración de GitHub
    ├── workflows/    # GitHub Actions
    └── ISSUE_TEMPLATE/
```

## Reglas simples

- La raíz debe tener pocos archivos.
- Código en `src/`.
- Pruebas en `tests/`.
- Documentación en `docs/`.
- Configuración de GitHub en `.github/`.
- Usa nombres claros: `mi-proyecto/`, `src/utils/`.

## Estándar para GitHub

Archivos importantes:

| Archivo | Para qué sirve |
|---|---|
| `README.md` | Página principal del repositorio. |
| `.gitignore` | Evita subir archivos basura. |
| `LICENSE` | Indica la licencia. |
| `CONTRIBUTING.md` | Explica cómo contribuir. |
| `.github/workflows/` | Automatizaciones y CI/CD. |
| `.github/ISSUE_TEMPLATE/` | Plantillas para issues. | 

## 5. Git: ramas, commits y pull requests
(pendiente)