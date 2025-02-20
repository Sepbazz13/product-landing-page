# product-landing-page
# Proyecto Nokia Indestructible - Documentación

## Estructura Semántica HTML

La estructura del sitio web se ha desarrollado siguiendo las mejores prácticas de HTML semántico, priorizando la accesibilidad y SEO.

### 1. Header (`<header>`)
- Contiene la navegación principal del sitio
- Uso de `<nav>` con `aria-label="Menú principal"` para mejor accesibilidad
- Enlaces de navegación organizados en lista `<ul>` para estructura semántica clara

```html
<header>
    <nav aria-label="Menú principal">
        <!-- Navegación -->
    </nav>
</header>
```

### 2. Contenido Principal (`<main>`)
Dividido en secciones semánticas para mejor organización y SEO:

#### Hero Section (`<section id="hero">`)
- Uso de `aria-labelledby="hero-title"` para vincular el contenido con su título
- Imagen principal con atributos alt descriptivos
- Estructura jerárquica con `<h1>` para el título principal

#### Features Section (`<section id="features">`)
- División en tres características principales usando `<div>`
- Títulos `<h3>` para mantener la jerarquía correcta
- Imágenes con alt text descriptivo para accesibilidad

### 3. Footer (`<footer>`)
Organizado en secciones lógicas para información de contacto:
- Uso de `<div class="footer-section">` para agrupar contenido relacionado
- Enlaces accesibles con `aria-label` para redes sociales
- Lista estructurada para horarios y enlaces

## Justificación de Etiquetas

1. **Etiquetas Semánticas Principales**:
   - `<header>`: Identifica claramente la cabecera del sitio
   - `<nav>`: Marca explícitamente la navegación principal
   - `<main>`: Contiene el contenido principal, excluyendo header y footer
   - `<footer>`: Agrupa la información de contacto y enlaces secundarios

2. **Etiquetas de Sección**:
   - `<section>`: Utilizada para dividir el contenido en bloques temáticos
   - `<h1>-<h3>`: Jerarquía clara de títulos para mejor SEO y estructura
   - `<div>`: Usado solo para agrupación visual sin valor semántico específico

3. **Elementos de Accesibilidad**:
   - Atributos `aria-label` y `aria-labelledby` para mejorar la navegación
   - Textos alternativos descriptivos en imágenes
   - Enlaces con propósito claro y textos descriptivos

## Prompts IA Utilizados

### Prompt 1: Footer con Información de Contacto
```
HU4: Footer con Información de Contacto
"Como visitante, quiero encontrar fácilmente la información de contacto y enlaces 
importantes al final de la página, para poder comunicarme con la empresa o acceder 
a recursos adicionales."

Criterios de Aceptación:
- Email de contacto
- Teléfono de soporte
- Horarios de atención
- Enlaces Importantes: Términos y condiciones
- Redes sociales
```

### Prompt 2: Estilos CSS Base
```
- Implementar un CSS reset o normalizer para consistencia entre navegadores
- Aplicar estilos de tipografía
- Espaciado y márgenes básicos
- Contraste adecuado para accesibilidad (de 3:1 a 5:1)
```

## Validación de Respuestas IA

1. **Validación de Estructura HTML**:
   - Verificación con W3C Validator
   - Comprobación de jerarquía de encabezados
   - Revisión de atributos ARIA y alt text

2. **Validación de CSS**:
   - Verificación de contrastes con WCAG Color Contrast Checker
   - Comprobación de responsive design en múltiples dispositivos
   - Testing de compatibilidad cross-browser

3. **Validación de Accesibilidad**:
   - Testing con lectores de pantalla
   - Verificación de navegación por teclado
   - Comprobación de WCAG 2.1 nivel AA

## Mejoras Futuras Planificadas

1. **Optimización**:
   - Implementar lazy loading para imágenes
   - Optimizar assets para mejor rendimiento
   - Añadir caché de recursos estáticos

2. **Accesibilidad**:
   - Añadir skip links para navegación por teclado
   - Implementar más roles ARIA donde sea necesario
   - Mejorar el contraste en elementos interactivos

3. **Contenido**:
   - Expandir sección de características
   - Añadir más detalles técnicos del producto
   - Implementar galería de imágenes interactiva
