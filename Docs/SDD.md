# SPEC-DRIVEN DEVELOPMENT (SDD)
## Proyecto Web — Galería de Crepas
### Versión
1.0
### Fecha
Marzo 2026
### Preparado por
Equipo de desarrollo web
---
# 1. PRODUCT SPECIFICATION
## 1.1 Descripción del proyecto
Diseño y desarrollo de un sitio web oficial para el restaurante **Galería de Crepas**, ubicado en la ciudad de Puebla.
El sitio funcionará como:
* escaparate visual del restaurante
* menú digital accesible mediante QR
* herramienta de atracción de clientes al local
* punto central de conexión con Instagram y WhatsApp
El proyecto busca fortalecer la identidad artística del restaurante y comunicar su propuesta gastronómica basada en crepas personalizables y crepas especiales.
---
# 1.2 Objetivos del proyecto
## Objetivo principal
Aumentar la afluencia de clientes al restaurante mediante una presencia digital visual, moderna y optimizada para dispositivos móviles.
## Objetivos secundarios
1. Mostrar el menú de forma clara y visual.
2. Ofrecer un menú digital accesible mediante QR en las mesas.
3. Reforzar el branding artístico del restaurante.
4. Integrar redes sociales para aumentar engagement.
5. Permitir la actualización sencilla del menú y contenido.
6. Preparar la arquitectura para futuras funciones de pedidos.
---
# 1.3 Público objetivo
### Segmento principal
**Estudiantes universitarios**
Características:
* consumo frecuente
* uso intensivo de redes sociales
* preferencia por experiencias visuales
### Segmento secundario
**Parejas**
Características:
* buscan lugares agradables
* valoran la estética del espacio
### Segmento terciario
**Familias**
Características:
* consumo ocasional
* valoran claridad del menú
---
# 1.4 Propuesta de valor
Galería de Crepas ofrece una experiencia gastronómica que combina:
* crepas artesanales
* un ambiente artístico con obras de artistas locales
* un sistema de menú simple y personalizable
El sitio web debe comunicar esta propuesta con claridad.
---
# 1.5 Funcionalidades principales
## F1 — Página de inicio
Presentación visual del restaurante.
Contenido:
* hero con fotografía
* introducción al concepto
* crepas destacadas
* acceso rápido al menú
* galería visual
* reseñas
* mapa de ubicación
---
## F2 — Menú digital
Página optimizada para dispositivos móviles.
Características:
* carga rápida
* navegación simple
* categorías claras
Categorías:
* crepas dulces
* crepas saladas
* ingredientes extra
* crepas especiales
---
## F3 — Galería
Sección visual que muestre:
* crepas
* interior del restaurante
* arte de la galería
---
## F4 — Crepas especiales
Sección dedicada a crepas con recetas especiales.
Contenido:
* fotografía
* descripción
* ingredientes
---
## F5 — Reseñas
Sección con opiniones de clientes.
Posible integración con:
Google Reviews.
---
## F6 — Ubicación
Mapa interactivo.
Información:
* dirección
* botón de navegación
* horarios
---
## F7 — Contacto
Integración con:
* Instagram
* WhatsApp Business
---
# 1.6 Casos de uso
## Caso de uso 1
Cliente busca crepas en Puebla.
Flujo:
1 usuario entra al sitio
2 visualiza fotos de crepas
3 revisa menú
4 decide visitar el restaurante
---
## Caso de uso 2
Cliente dentro del restaurante.
Flujo:
1 escanea QR
2 accede al menú
3 revisa opciones
4 realiza pedido en caja
---
## Caso de uso 3
Cliente descubre el restaurante en Instagram.
Flujo:
1 entra al sitio desde perfil
2 ve galería
3 revisa ubicación
4 planea visita
---
# 2. DESIGN SPECIFICATION
## 2.1 Identidad visual
La identidad de marca utiliza una estética artística basada en:
* diversidad de sabores
* creatividad visual
* ambiente cultural
El logotipo representa una crepa con elementos geométricos que simbolizan variedad de sensaciones.
---
## 2.2 Paleta cromática
Colores principales:
Guinda
HEX #9f056d
Verde
HEX #8ed94f
Colores secundarios:
variaciones claras y oscuras de estos tonos.
Uso recomendado:
* guinda como color principal
* verde como color de acento
* fondo blanco o gris claro
---
## 2.3 Tipografía
Tipografías oficiales:
Títulos
Londrina Solid
Cuerpo de texto
Montserrat
Jerarquía:
Hero
Londrina Solid
Subtítulos
Montserrat SemiBold
Texto
Montserrat Regular
---
## 2.4 Estilo visual
El sitio debe transmitir:
* creatividad
* energía visual
* cercanía
* modernidad
Características visuales:
* fotografías grandes
* composiciones tipo galería
* uso de bloques de color
* diseño limpio
---
## 2.5 Componentes visuales
Componentes del sistema de diseño:
HeroSection
MenuCard
CrepaCard
GalleryGrid
ReviewCard
MapSection
WhatsAppButton
MenuCategory
---
# 2.6 Wireframe general
Página Inicio
Hero
Concepto
Crepas especiales
Cómo funciona el menú
Galería
Reseñas
Ubicación
Footer
---
# 3. TECHNICAL SPECIFICATION
## 3.1 Arquitectura tecnológica
Frontend
Astro
Estilos
Tailwind CSS
Gestión de contenido
CMS Headless
Opciones recomendadas:
Sanity
Strapi
Directus
---
## 3.2 Estructura del proyecto
repository
galeria-de-crepas-web
estructura
docs
src
components
pages
layouts
styles
public
---
## 3.3 Estructura de páginas
/
home
/menu
menú completo
/crepas-especiales
/galeria
/ubicacion
/contacto
---
## 3.4 SEO
Optimización para búsquedas locales.
Palabras clave objetivo:
crepas Puebla
crepas dulces Puebla
crepas saladas Puebla
crepas cerca de universidades Puebla
---
## 3.5 Performance
Requisitos:
* carga menor a 2 segundos
* optimización de imágenes
* diseño mobile-first
---
## 3.6 Integraciones
Google Maps
Instagram feed
WhatsApp Business
---
# 4. CONTENT SPECIFICATION
## 4.1 Tipos de contenido
Crepas
Ingredientes
Crepas especiales
Imágenes
Reseñas
Información del local
---
## 4.2 Frecuencia de actualización
Menú
2 a 3 veces por mes.
---
# 5. QR MENU SYSTEM
El restaurante usará códigos QR en las mesas.
El QR redirigirá a:
/menu
Ventajas:
* actualización inmediata
* no requiere impresión
* mejor experiencia móvil
---
# 6. FUTURE FEATURES
Posibles evoluciones del sitio:
Pedidos por WhatsApp
Sistema de pedidos online
Programa de promociones
Sección de artistas locales
---
# 7. DEVELOPMENT ROADMAP
## Fase 1
Definición de arquitectura
Creación de repositorio
---
## Fase 2
Wireframes
Prototipo en Figma
---
## Fase 3
Desarrollo frontend
---
## Fase 4
Integración CMS
---
## Fase 5
Optimización SEO
---
## Fase 6
Publicación
---
# 8. ÉXITO DEL PROYECTO
El proyecto será exitoso si:
* el menú es fácil de consultar
* el sitio carga rápido
* el diseño refleja la identidad del restaurante
* aumenta la interacción desde Instagram
* mejora la visibilidad local
---
# FIN DEL DOCUMENTO
