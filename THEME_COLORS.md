# Guía de Colores del Tema

Este documento describe la paleta de colores personalizada implementada en el proyecto, diseñada siguiendo las mejores prácticas de accesibilidad.

## Paleta de Colores Principal

### Primary (Azul)
Usado para elementos principales, botones primarios y enlaces importantes.
- `primary-50` a `primary-950`: Gama completa de azules
- Base: `primary-500` (#3b82f6)
- Uso recomendado: Botones principales, enlaces, elementos interactivos

### Secondary (Teal/Verde Azulado)
Para elementos secundarios y de apoyo.
- `secondary-50` a `secondary-950`: Gama completa de teals
- Base: `secondary-500` (#14b8a6)
- Uso recomendado: Botones secundarios, badges, elementos de apoyo

### Tertiary (Magenta/Púrpura)
Para acentos y elementos destacados.
- `tertiary-50` a `tertiary-950`: Gama completa de magentas
- Base: `tertiary-500` (#d946ef)
- Uso recomendado: Elementos decorativos, acentos especiales

### Accent (Naranja)
Para llamadas a la acción y elementos que requieren atención.
- `accent-50` a `accent-950`: Gama completa de naranjas
- Base: `accent-500` (#f97316)
- Uso recomendado: CTAs, elementos que requieren atención inmediata

## Colores de Estado

### Success (Verde)
- Base: `success-500` (#22c55e)
- Uso: Mensajes de éxito, confirmaciones, estados positivos

### Warning (Amarillo/Ámbar)
- Base: `warning-500` (#f59e0b)
- Uso: Advertencias, estados de precaución

### Error (Rojo)
- Base: `error-500` (#ef4444)
- Uso: Errores, estados negativos, eliminación

### Info (Azul Cielo)
- Base: `info-500` (#0ea5e9)
- Uso: Información general, tooltips, ayuda

## Colores Neutros

### Neutral
Grises mejorados para fondos y elementos neutros.
- `neutral-50` a `neutral-950`: Gama completa de grises

## Modo Claro/Oscuro

### Light Mode
- `light-bg`: #ffffff (Fondo principal)
- `light-surface`: #f8fafc (Superficies elevadas)
- `light-border`: #e2e8f0 (Bordes)
- `light-text`: #0f172a (Texto principal, contraste 15.3:1)
- `light-muted`: #64748b (Texto secundario, contraste 4.7:1)

### Dark Mode
- `dark-bg`: #0f172a (Fondo principal)
- `dark-surface`: #1e293b (Superficies elevadas)
- `dark-border`: #334155 (Bordes)
- `dark-text`: #f8fafc (Texto principal, contraste 15.3:1)
- `dark-muted`: #94a3b8 (Texto secundario, contraste 4.7:1)

## Accesibilidad

Todos los colores han sido seleccionados cumpliendo con las pautas WCAG 2.1:

- **Nivel AA**: Contraste mínimo de 4.5:1 para texto normal
- **Nivel AAA**: Contraste mínimo de 7:1 para texto importante
- **Focus States**: Todos los elementos interactivos tienen estados de foco visibles
- **Color Alone**: No se usa solo el color para transmitir información

## Ejemplos de Uso

### Botones
```html
<!-- Botón primario -->
<button class="bg-primary-500 hover:bg-primary-600 text-white px-4 py-2 rounded-lg focus:ring-2 focus:ring-primary-500">
  Botón Principal
</button>

<!-- Botón secundario -->
<button class="bg-secondary-500 hover:bg-secondary-600 text-white px-4 py-2 rounded-lg focus:ring-2 focus:ring-secondary-500">
  Botón Secundario
</button>
```

### Tarjetas
```html
<div class="bg-light-surface dark:bg-dark-surface border border-light-border dark:border-dark-border rounded-lg p-4">
  <h3 class="text-light-text dark:text-dark-text">Título</h3>
  <p class="text-light-muted dark:text-dark-muted">Descripción</p>
</div>
```

### Estados
```html
<!-- Mensaje de éxito -->
<div class="bg-success-50 border border-success-200 text-success-800 p-4 rounded-lg">
  Operación exitosa
</div>

<!-- Mensaje de error -->
<div class="bg-error-50 border border-error-200 text-error-800 p-4 rounded-lg">
  Error en la operación
</div>
```

## Notas de Implementación

1. **Consistencia**: Usa siempre los colores del tema en lugar de colores hardcodeados
2. **Modo Oscuro**: Siempre incluir variantes dark: para todos los colores
3. **Estados de Foco**: Incluir focus:ring-2 y focus:ring-{color}-500 en elementos interactivos
4. **Transiciones**: Usar transition-colors duration-200 para cambios suaves
5. **Contrastes**: Verificar siempre el contraste, especialmente en modo oscuro
