# Capítulo IV: Product Design
## 4.1. Style Guidelines

En esta sección se establecen los lineamientos visuales y comunicativos que guiarán el diseño de la plataforma, con el objetivo de garantizar una experiencia consistente, accesible y alineada al dominio terapéutico.
Las decisiones de diseño se fundamentan en principios de claridad, accesibilidad y confianza, tomando como referencia buenas prácticas de sistemas de diseño como Material Design.

### 4.1.1. General Style Guidelines

### Branding:

Nuestra plataforma está dirigida a padres, profesionales de la terapia e instituciones. Su identidad visual busca transmitir confianza, accesibilidad y acompañamiento.
El sistema se presenta como una herramienta de apoyo en procesos terapéuticos y educativos. Por eso, el diseño evita elementos visuales complejos o sobrecargados. Prioriza la claridad, la empatía y la facilidad de uso.
Además, se busca generar una sensación de seguridad en los usuarios, especialmente en los padres, quienes necesitan confiar en la plataforma para seguir el desarrollo de sus hijos.

### Typography:

Se utiliza un tipo de letra sin remates, dado que es muy legible en entornos digitales y puede ser empleado por los diferentes tipos de usuarios.
La jerarquía tipográfica está estructurada de la siguiente forma:
* Títulos: tamaño grande, peso bold, para marcar las secciones de contenido principal.
* Subtítulos: tamaño medio, peso semi-bold.
* Texto general: tamaño estándar, peso regular.
* Botones y etiquetas: tamaño medio, matiz visual.
Esta estructura se traduce en una lectura fácil, lo cual resulta especialmente importante para los padres de familia, que necesitan asimilar rápidamente la información, así como para usuarios con distintas capacidades cognitivas.

### Colors:

* Morado (Color principal): El morado es el que representa mayor empatía, sensibilidad y apoyo. El morado es el color sin lugar a dudas, apropiado para un entorno relacionado con la atención y el desarrollo de personas con necesidades especiales, pues transmite la proximidad y comprensión necesarias.
* Azul (Color secundario): Refuerza la confianza, la seguridad y el profesionalismo. El azul será clave para que los padres de familia se sientan tranquilos y tengan credibilidad de que los servicios que ofrece la plataforma son verdaderos.
* Amarillo (Color de acento): Brinda energía, optimismo y dinamismo. Se utiliza en elementos interactivos o enfatizados (botones o notificaciones) para llamar la atención proporcionando una señal de alerta pero sin saturación visual.
* Colores neutros (blanco y grises): Se utilizan como base para los fondos y las estructuras así que permiten que la interfaz sea limpia, legible y fácil de navegar.

### Spacing:

Se aplica un sistema de espaciado basado en una cuadrícula modular (8px) para poder conseguir una uniformidad visual en toda la interfaz.
El espaciado correcto entre los elementos permite:

* Mejorar la legibilidad.
* Evitar la saturación visual.
* Facilitar la navegación.

| Token    | Valor (px) | Valor (DXA/rem) | Aplicación                                      |
|----------|------------|-----------------|-------------------------------------------------|
| space-1  | 4px        | 0.25rem         | Separación interna mínima (icono + texto)       |
| space-2  | 8px        | 0.5rem          | Padding interno de chips y badges               |
| space-3  | 12px       | 0.75rem         | Padding de campos de texto (input)              |
| space-4  | 16px       | 1rem            | Padding estándar de tarjetas y botones          |
| space-5  | 20px       | 1.25rem         | Separación entre componentes relacionados       |
| space-6  | 24px       | 1.5rem          | Margen entre secciones de formulario            |
| space-8  | 32px       | 2rem            | Separación entre secciones de contenido         |
| space-10 | 40px       | 2.5rem          | Padding de secciones principales (contenedores) |
| space-12 | 48px       | 3rem            | Espaciado entre bloques de página               |
| space-16 | 64px       | 4rem            | Margen vertical entre secciones de página       |
| space-24 | 96px       | 6rem            | Hero sections y márgenes de pantalla completa   |

Dado que la plataforma incluye una multitud de funcionalidades (calendario, sesiones, marketplace, etc.), los espacios en blanco se convierten en un aspecto clave para conseguir una interfaz ordenada y que el usuario pueda entender.

### Dimensiones a adoptar:

El tono de comunicación:

| Dimensión                | Posición            | Justificación                                                                   |
|--------------------------|---------------------|---------------------------------------------------------------------------------|
| Divertido / Serio        | Balanceado (50/50)  | Se usa humor con moderación; no trivializa situaciones sensibles de los niños.  |
| Formal / Casual          | Semi-formal (40/60) | Tono cercano y accesible para padres, sin perder credibilidad profesional.      |
| Respetuoso / Irreverente | Respetuoso (90/10)  | Siempre empático y sensible a las necesidades especiales.                       |
| Entusiasta / Sereno      | Sereno (30/70)      | Transmite tranquilidad y confianza; evita generar ansiedad en los padres.       |

Lenguaje aplicado: Claro, empático y directo.

Se excluye el empleo del léxico técnico complicado, preponderando mensajes fáciles de entender para los padres de familia. A la vez, se mantiene un tono respetuoso por la sensibilidad que esta problemática conlleva (niños con necesidades especiales).

### Accesibilidad:

La plataforma está diseñada para ser utilizada por personas con distintas capacidades visuales, cognitivas y motrices. Se aplican los principios WCAG 2.1 nivel AA como estándar mínimo, con aspiración a nivel AAA en los módulos más críticos.
Principios aplicados:

* Contraste de color: ratio mínimo 4.5:1 para texto normal y 3:1 para texto grande. Todos los colores de la paleta han sido verificados.
* Tamaños táctiles: todos los elementos interactivos tienen un área mínima de 44×44px (WCAG 2.5.5).
* Navegación por teclado: todos los flujos críticos son completamente navegables sin ratón.
* Etiquetas ARIA: todos los componentes interactivos incluyen atributos aria-label, aria-describedby o roles semánticos correctos.
* Texto alternativo: todas las imágenes informativas incluyen atributo alt descriptivo.
* Indicador de foco visible: se muestra un outline claro (#5B2D8E, 3px) al navegar con teclado.
* Compatibilidad multiplataforma: web (Chrome, Firefox, Safari, Edge), iOS y Android.
* Modo de alto contraste: se respetan las preferencias del sistema operativo (prefers-contrast: more).
* Reducción de movimiento: las animaciones se desactivan si el usuario tiene activado prefers-reduced-motion.

### 4.1.2. Web Style Guidelines

En esta sección se explican e ilustran las decisiones sobre los estándares visuales y de interacción para las interfaces web responsivas de la plataforma. Se definen los componentes, patrones de interacción y especificaciones técnicas para el desarrollo front-end web.

### Breakpoints y Diseño Responsivo:

La interfaz web adopta un enfoque mobile-first, escalando progresivamente hacia pantallas más grandes. Se definen los siguientes breakpoints:

* xs — < 480px: Móviles pequeños (diseño base).
* sm — 480px – 767px: Móviles grandes y phablets.
* md — 768px – 1023px: Tablets en orientación vertical.
* lg — 1024px – 1279px: Tablets en horizontal y laptops pequeñas.
* xl — 1280px – 1535px: Desktops estándar.
* 2xl — ≥ 1536px: Pantallas grandes y monitores 4K.

### Componentes Base
Los componentes de la interfaz web siguen el sistema de componentes de Material Design 3, adaptados a la identidad visual de la plataforma. A continuación se documentan los principales:

Botones:
*  Primario (Filled): Fondo #F5A623 texto blanco, border-radius 8px, padding 12px 24px. Hover: #7B4DB0. Active: #4A2070.
*  Acento (Filled Tonal): Fondo #F5A623, texto #111827, border-radius 8px. Para CTAs de alta visibilidad.
*  Ghost / Text: Sin borde ni fondo. Texto #5B2D8E. Para acciones de baja prioridad.
*  Destructivo: Fondo #C62828, texto blanco. Solo para acciones irreversibles (eliminar, cancelar sesión).
   Todos los botones incluyen: estado disabled (opacidad 38%), indicador de foco visible, estado loading con spinner, y mínimo 44px de altura para accesibilidad táctil.

Inputs y Formularios:
* Campo de texto: border 1px #5B2D8E, border-radius 6px, padding 12px 16px. Focus: border 2px #5B2D8E + box-shadow 0 0 0 3px #EDE5F7.
* Estado de error: border 2px #C62828, mensaje de error en #C62828 debajo del campo.
* Estado de éxito: border 2px #2E7D32 + icono de check en el campo.
* Labels: siempre visibles (no dependen del placeholder). Texto #343A40, Body Medium.
* Helper text: texto secundario debajo del campo, Color #6C757D, Body Small.

Tarjetas (Cards):
* Fondo: #FFFFFF, border-radius 12px, box-shadow 0 2px 8px rgba(0,0,0,0.08).
* Borde opcional: 1px #DEE2E6 para tarjetas en fondos de mismo color.
* Padding interno: 24px (space-6).
* Hover interactivo: box-shadow 0 4px 16px rgba(91,45,142,0.12), transform translateY(-2px), transición 200ms ease.

Navegación:
* Top App Bar (desktop): altura 64px, fondo #FFFFFF, sombra sutil. Logo a la izquierda, navegación principal centrada, acciones de usuario a la derecha.
* Sidebar (dashboard): ancho 260px colapsado a 72px en tablet. Fondo #F8F9FA, íconos + labels. Ítem activo: fondo #EDE5F7, texto #5B2D8E, borde izquierdo 3px #5B2D8E.
* Bottom Navigation (mobile): 4–5 destinos, íconos + labels cortos, ítem activo en #5B2D8E.
* Breadcrumbs: separador /, texto #111827, ítem activo #343A40, Body Medium.

Iconografía:
* Biblioteca base: Material Symbols (Google) en variante Rounded.
* Tamaños: 20px (inline/label), 24px (estándar), 32px (destacado), 48px (hero/vacío).
* Color por defecto: hereda del contexto. En superficies claras: #343A40. En superficies de color: #FFFFFF.
* Íconos de estado: siempre acompañados de texto (no dependen del ícono solo para transmitir información).

### Mobile Style Guidelines

Esta sección define las adaptaciones específicas de los componentes, patrones de interacción y lineamientos visuales para dispositivos móviles, manteniendo coherencia directa con el sistema definido en Web Style Guidelines (Material Design 3 adaptado a la identidad visual de la plataforma).
El diseño mobile sigue un enfoque mobile-first, priorizando claridad, accesibilidad y ejecución rápida de tareas críticas como agendar citas, revisar progreso y comunicarse.

Resoluciones y Breakpoints Mobile
Se consideran los siguientes rangos para mobile:
* xs (<480px): móviles pequeños (base del diseño).
* sm (480px – 767px): móviles grandes.
  El diseño se construye desde xs como base, escalando a sm sin alterar la jerarquía visual.

Adaptación de Componentes Base

Botones (Mobile)
Se derivan directamente de los definidos en web, con ajustes táctiles:
* Altura mínima: 44px (accesibilidad)
* Padding: 12px 16px (más compacto que web)
* Border-radius: 8px

### Tipos:
Primario (Filled):
* Fondo: #5B2D8E.
* Texto: #FFFFFF.
* Active: #4A2070.

Secundario (Outlined):
* Borde: 1.5px #5B2D8E.
* Texto: #5B2D8E.
* Fondo: transparente.

Acento (CTA):
* Fondo: #F5A623.
* Uso: acciones principales (ej: “Agendar cita”).

Destructivo:
* Fondo: #C62828.
* Uso: cancelar sesión, eliminar registro.

### Estados incluidos:
* Disabled: opacidad 38%.
* Loading: spinner centrado.
* Focus: outline visible (#5B2D8E, 3px).

Inputs y Formularios (Mobile)
Adaptación para interacción táctil:
* Padding: 12px 16px.
* Border: 1px #DEE2E6.
* Border-radius: 6px.

### Estados:
Focus:
* Border: 2px #5B2D8E.
* Shadow: 0 0 0 3px #EDE5F7.

Error:
* Border: 2px #C62828.
* Mensaje debajo.

Éxito:
* Border: 2px #2E7D32.
* Ícono check.

### Consideraciones mobile:
* Labels siempre visibles (no placeholder).
* Formularios divididos en pasos (stepper).
* Inputs ocupan 100% del ancho.

Tarjetas (Cards) – Mobile
Se mantienen consistentes con web:
* Fondo: #FFFFFF.
* Border-radius: 12px.
* Shadow: 0 2px 8px rgba(0,0,0,0.08).
* Padding: 16px–24px (space-4 a space-6).

### Uso principal:
* Sesiones
* Reportes
* Pacientes

### Interacción:
* Swipe gestures (acción rápida).
* Tap para expandir detalle.

Navegación Mobile

Bottom Navigation (Principal)
* 4–5 ítems máximo:
- Inicio
- Citas
- Progreso
- Mensajes
- Perfil

* Ítem activo:
- Color: #5B2D8E
- Label visible siempre

Top Bar (Mobile)
* Altura: 56px
* Fondo: #FFFFFF
* Incluye:
- Título de pantalla
- Botón de retroceso

Componentes Específicos Mobile

FAB (Floating Action Button)
* Tamaño: 56px
* Color: #5B2D8E
* Ícono: blanco
* Uso:
- Acción principal (ej: agendar cita).

Bottom Sheets
* Reemplazan modales web
* Altura adaptable
* Incluyen drag handle

Uso:
* Confirmar citas
* Ver detalles
* Acciones rápidas

Snackbars
* Posición: inferior
* Duración: 4 segundos
* Acción opcional (ej: “Deshacer”)

Pull-to-refresh
* Aplicado en:
- Lista de citas
- Mensajes
- Progreso

Gestos (Swipe)
* Swipe derecha → confirmar.
* Swipe izquierda → cancelar/eliminar.

Iconografía
Se mantiene el sistema definido en web:
* Biblioteca: Material Symbols Rounded.
* Tamaños:
- 24px estándar
- 20px en labels

### Reglas:
* Nunca usar solo ícono sin texto en acciones críticas.
* Color:
- #343A40 en fondos claros.
- #FFFFFF en fondos oscuros.

Densidad y Layout Mobile
Para evitar sobrecarga cognitiva:
* Máximo 1 acción principal por pantalla.
* Listas de 3–5 elementos visibles.
* Texto mínimo: 16px.
* Uso de spacing basado en sistema de 8px.

### Accesibilidad en Mobile
Se mantiene alineación con WCAG 2.1:
* Área táctil mínima: 44x44px.
* Contraste mínimo 4.5:1.
* Navegación compatible con lectores de pantalla.
* Indicador de foco visible.
* Soporte para:
- prefers-reduced-motion.
- modo alto contraste.

## 4.1.3.1. IOS Mobile Style Guidelines.
Resolución y Breakpoints iOS
Se consideran los siguientes dispositivos como referencia:
* iPhone SE / mini (375px): base mínima del diseño.
* iPhone estándar (390px – 430px): rango principal de diseño.
* iPhone Plus / Pro Max (430px+): escalado fluido sin ruptura de jerarquía.

El diseño se construye desde 375px como base, escalando hacia arriba sin alterar la estructura visual ni la densidad de información.

Componentes Base – Adaptación iOS

Botones (iOS)
Se mantiene el sistema definido en Mobile Style Guidelines con ajustes para la experiencia táctil de iOS:
* Altura mínima: 44px (alineado con las recomendaciones de Apple HIG).
* Border-radius: 10px (acercamiento a la estética de iOS).
* Feedback táctil: se usa UIImpactFeedbackGenerator (haptic feedback suave en acciones primarias).

Tipos heredados:
* Primario (Filled): fondo #5B2D8E, texto #FFFFFF.
* Secundario (Outlined): borde 1.5px #5B2D8E, fondo transparente.
* Acento (CTA): fondo #F5A623, uso en "Agendar cita".
* Destructivo: fondo #C62828, confirmación mediante Action Sheet nativo

Inputs y Formularios (iOS)
* Uso del teclado nativo de iOS según tipo de campo: emailAddress, phonePad, numberPad, default.
* Return key configurado contextualmente: "Siguiente" en campos intermedios, "Listo" en el último campo.
* Labels siempre visibles por encima del campo (no como placeholder).
* Formularios extensos divididos en pasos con stepper visible.

Estados:
* Focus: borde 2px #5B2D8E, sombra 0 0 0 3px #EDE5F7.
* Error: borde 2px #C62828 con mensaje descriptivo debajo.
* Éxito: borde 2px #2E7D32 con ícono de check.

Navegación iOS

Tab Bar (Bottom Navigation)

Reemplaza la Bottom Navigation genérica siguiendo el patrón nativo UITabBar:
* Máximo 5 ítems: Inicio, Citas, Progreso, Mensajes, Perfil.
* Ítem activo: color #5B2D8E, label siempre visible.
* Fondo: #FFFFFF con separador sutil (#DEE2E6).
* Compatible con gestos de deslizamiento horizontal entre tabs.

Navigation Bar (Top Bar)

Sigue el patrón UINavigationBar:

* Altura: 44px (sin safe area).
* Fondo: #FFFFFF.
* Título centrado en vistas de detalle; alineado a la izquierda en vistas raíz (Large Title).
* Botón de retroceso: chevron nativo + label de pantalla anterior.

Safe Area

Todos los layouts respetan las Safe Areas de iOS:
* Top: barra de estado + Navigation Bar.
* Bottom: Home Indicator (especialmente en iPhone sin botón físico).
* Ningún elemento interactivo se superpone al Home Indicator.

Componentes Específicos iOS

Action Sheets

Reemplazan modales de confirmación destructiva:
* Título descriptivo de la acción.
* Opción destructiva en rojo (#C62828).
* Siempre incluye opción "Cancelar".

Bottom Sheets / Sheets

Adaptados al patrón UISheetPresentationController:
* Altura adaptable con detents: .medium y .large.
* Drag handle visible.
* Uso: confirmar citas, ver detalles de sesión, acciones rápidas.

Alerts

Para confirmaciones críticas se usa el estilo de alerta nativo de iOS:
* Título + mensaje breve.
* Máximo 2 acciones (confirmar / cancelar).
* Nunca más de 2 botones en línea.

Pull-to-Refresh

Implementado con UIRefreshControl nativo en:
* Lista de citas.
* Mensajes.
* Progreso del estudiante.

Iconografía en iOS

Se mantiene la biblioteca Material Symbols Rounded del sistema general, garantizando consistencia multiplataforma:
* Tamaño estándar: 24px.
* Tamaño en labels y Tab Bar: 24px con label debajo.
* Color en fondos claros: #343A40.
* Color en fondos de color / oscuros: #FFFFFF.
* Nunca usar ícono solo sin texto en acciones críticas.

Tipografía en iOS

Se respeta la escala tipográfica del sistema, con adaptaciones para legibilidad en iOS:
* Fuente principal del sistema: SF Pro como fallback si la fuente propia no carga (definir en font-family).
* Texto mínimo: 16px para evitar zoom automático del navegador/app.
* Interlineado mínimo: 1.5 en párrafos de contenido.
* Soporte para Dynamic Type de iOS: los tamaños escalan con la configuración de accesibilidad del usuario.

| Gesto                         | Acción                                            |
|-------------------------------|---------------------------------------------------|
| Swipe derecha (desde borde)   | Retroceder en la navegación (back gesture nativo) |
| Swipe derecha sobre tarjeta   | Confirmar / acción positiva                       |
| Swipe izquierda sobre tarjeta | Menú contextual (acciones secundarias)            |
| Long press                    | Cancelar / eliminar                               |
| Pull down                     | Cerrar modales / sheets                           |

Accesibilidad en iOS

Alineado con WCAG 2.1 y las pautas de Apple Accessibility:
* Área táctil mínima: 44×44px.
* Contraste mínimo: 4.5:1 (texto normal), 3:1 (texto grande).
* Soporte para prefers-reduced-motion: desactivar animaciones decorativas.
* Indicador de foco visible en navegación por teclado externo (iPad / bluetooth).
* Compatible con modo de alto contraste y texto en negrita del sistema.