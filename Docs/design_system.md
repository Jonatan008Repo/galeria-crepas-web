# Galería de Crepas — Design System

Documentación del sistema de diseño del sitio web **Galería de Crepas**.

Este Design System define los principios visuales, tokens de diseño, componentes y reglas de layout que garantizan consistencia visual, escalabilidad y facilidad de mantenimiento en el proyecto.

---

# 1. Principios de Diseño

El sitio debe reflejar el concepto central del restaurante:

**Gastronomía + Arte**

Principios clave:

**Visual First**
La fotografía de comida y del espacio debe ser protagonista.

**Simple Menu UX**
El menú debe ser extremadamente fácil de leer, especialmente cuando se accede mediante QR.

**Mobile First**
Gran parte del tráfico provendrá de escaneo QR o Instagram.

**Estética tipo galería**
El layout debe recordar una galería artística: espacios amplios, imágenes grandes, composición visual cuidada.

---

# 2. Design Tokens

Los tokens son las unidades básicas del sistema visual.

## Colores

### Brand

Guinda (Primario)

```
color-brand-primary
#9F056D
```

Verde (Secundario)

```
color-brand-secondary
#8ED94F
```

---

### Neutrales

Negro suave

```
#1A1A1A
```

Gris oscuro

```
#444444
```

Gris medio

```
#888888
```

Gris claro

```
#F5F5F5
```

Blanco

```
#FFFFFF
```

---

## Tipografía

### Headings

Fuente:

**Londrina Solid**

Uso:

* títulos principales
* encabezados de sección
* nombres de crepas

Escala recomendada:

H1 — 48px
H2 — 36px
H3 — 28px
H4 — 22px

---

### Texto de interfaz

Fuente:

**Montserrat**

Uso:

* textos de menú
* descripciones
* botones
* navegación

Escala recomendada:

Body Large — 18px
Body — 16px
Small — 14px
Caption — 12px

---

# 3. Sistema de Espaciado

El sistema usa una **grid de 8px**.

Tokens:

```
space-1  = 4px
space-2  = 8px
space-3  = 16px
space-4  = 24px
space-5  = 32px
space-6  = 48px
space-7  = 64px
space-8  = 96px
```

Uso típico:

Secciones grandes
64px – 96px

Separación entre componentes
24px – 32px

Separación interna de cards
16px

---

# 4. Grid System

El sitio utiliza un **layout responsive basado en 12 columnas**.

## Desktop

```
12 columns
max width: 1200px
gutter: 24px
margin: auto
```

## Tablet

```
8 columns
gutter: 20px
```

## Mobile

```
4 columns
gutter: 16px
```

---

# 5. Border Radius

Tokens:

```
radius-sm = 6px
radius-md = 10px
radius-lg = 16px
radius-xl = 24px
```

Uso:

Cards
radius-md

Imágenes
radius-lg

Botones
radius-md

---

# 6. Sombras

Las sombras deben ser suaves para mantener una estética moderna.

Card Shadow

```
0px 6px 20px rgba(0,0,0,0.08)
```

Hover Shadow

```
0px 10px 30px rgba(0,0,0,0.12)
```

---

# 7. Componentes UI

## Navbar

Elementos:

* logo
* menú principal
* botón WhatsApp

En mobile se convierte en **hamburger menu**.

---

## Botones

### Primary Button

Color

```
background: #9F056D
text: white
```

Hover

```
background: darker guinda
```

Uso:

* ver menú
* ver galería
* contacto

---

### Secondary Button

```
background: transparent
border: brand color
text: brand color
```

---

## Menu Card

Elemento clave del sitio.

Contenido:

* foto de la crepa
* nombre
* ingredientes

Layout:

```
image
title
ingredient list
```

---

## Crepa Especial Card

Incluye:

* imagen grande
* nombre
* descripción
* ingredientes destacados

Estas cards deben ser **visualmente más prominentes**.

---

## Review Card

Contenido:

* foto o avatar
* nombre
* rating
* comentario

---

## Gallery Grid

Layout tipo:

**masonry / instagram grid**

Ejemplo:

```
2 columnas mobile
3 tablet
4 desktop
```

---

## WhatsApp Floating Button

Posición:

```
bottom-right
```

Siempre visible.

Acción:

Abrir chat directo.

---

# 8. Iconografía

Iconos simples estilo:

* outline
* minimal

Uso típico:

* ubicación
* horario
* teléfono
* redes sociales

Bibliotecas recomendadas:

* Lucide
* Heroicons

---

# 9. Imágenes

Las imágenes deben cumplir:

Resolución mínima

```
1600px ancho
```

Formato recomendado

```
WebP
```

Tipos de imágenes:

* comida
* interior del local
* galería de arte
* clientes disfrutando

---

# 10. Accesibilidad

Reglas mínimas:

Contraste mínimo
WCAG AA

Texto mínimo

```
16px
```

Imágenes

Siempre incluir **alt text**.

---

# 11. Animaciones

Las animaciones deben ser sutiles.

Ejemplos:

Hover en cards

```
scale 1 → 1.03
```

Fade-in en secciones

```
opacity 0 → 1
```

Duración

```
200ms – 300ms
```

---

# 12. Responsive Strategy

Mobile es la prioridad.

Flujos críticos:

* escaneo de QR
* navegación del menú
* ver ubicación

Las páginas deben cargarse rápido incluso en redes móviles.

---

# 13. Estructura en Figma

El archivo de Figma debe organizarse así:

```
Foundations
    Colors
    Typography
    Spacing

Components
    Buttons
    Cards
    Navbar
    Footer

Patterns
    Menu Layout
    Gallery Layout
    Hero Sections

Pages
    Home
    Menu
    Special Crepes
    Gallery
```
