# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

### 5.1.1. Software Development Environment Configuration

En esta sección se describen los productos de software utilizados por los miembros del equipo Conecta para colaborar en el ciclo de vida del producto TherapyConnect, organizados por tipo de actividad.

**Project Management**
Para la gestión del proyecto se utilizó Trello (https://trello.com), herramienta basada en el modelo Kanban que permite organizar tareas, asignar responsables y hacer seguimiento del avance por sprint de forma visual y colaborativa.

**Product UX/UI Design**
Para el diseño de wireframes, mock-ups y prototipos interactivos se utilizó Figma (https://www.figma.com), herramienta colaborativa basada en la web que permite diseñar interfaces y compartir prototipos en tiempo real. Para la elaboración de User Personas, Empathy Maps, Journey Maps e Impact Maps se utilizó UXPressia (https://uxpressia.com). Para los diagramas de Wireflows, User Flows y Event Storming se utilizó LucidChart (https://www.lucidchart.com) y Miro (https://miro.com).

**Software Development**
Para el desarrollo del Landing Page se utilizó HTML5, CSS3 y JavaScript, editados mediante Visual Studio Code (https://code.visualstudio.com), editor de código ligero y extensible ampliamente adoptado en el equipo.

**Software Documentation**
Para la documentación de los Web Services se utilizó Swagger UI mediante la especificación OpenAPI (https://swagger.io), lo que permite visualizar y probar los endpoints del API de forma interactiva. Para los diagramas de arquitectura de software bajo el modelo C4 se utilizó Miro (https://miro.com). Para diagramas UML y de base de datos se utilizó LucidChart y Vertabelo (https://vertabelo.com).

**Software Deployment**
Para el despliegue del Landing Page se utilizó GitHub Pages (https://pages.github.com), servicio gratuito integrado con GitHub que permite publicar sitios estáticos directamente desde un repositorio. Para el despliegue de la Web Application y los Web Services se utilizarán servicios cloud como Railway o Render, a definir en sprints posteriores.

**Version Control**
Para el almacenamiento y control de versiones del código fuente se utilizó Git gestionado desde GitHub (https://github.com), aplicando el flujo de trabajo GitFlow, Conventional Commits y Semantic Versioning.

---

### 5.1.2. Source Code Management

El equipo Conecta utiliza GitHub como plataforma de control de versiones y colaboración, bajo la organización pública:

**Organización GitHub:** https://github.com/1ASI0729-2610-11913

Los repositorios establecidos para cada producto de la solución son los siguientes:

| Producto | Repositorio URL |
|---|---|
| Startup / Informe | https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect.git |
| Landing Page | (por definir — se creará bajo la misma organización) |
| Frontend Web Application | (por definir — se creará bajo la misma organización) |
| RESTful Web Services | (por definir — se creará bajo la misma organización) |

---

### 5.1.3. Source Code Style Guide & Conventions

Esta sección está dedicada a determinar y establecer las convenciones y estándares que serán utilizados en la codificación por el equipo para que la solución garantice consistencia, legibilidad y mantenibilidad. Los lineamientos aquí aplicados tienen su base en guías definidas y posteriormente bien conocidas como Google Style Guides, Angular Style Guide y las prácticas de Spring Boot.

**Principios Generales:**
- Todo el código debe neutralizarse en inglés (nombres de variable, función, clase, etc.).
- Se prioriza la claridad sobre la complejidad.
- El código debe ser autoexplicativo: no se permiten comentarios.
- Se debe respetar una estructura común en todos los archivos.
- Se aplicará el principio de SRP (Single Responsibility) a funciones y clases.

**Nomenclatura General:**
- **Variables:** Se utilizará la nomenclatura camelCase para nombrar variables, iniciando con minúscula y usando palabras descriptivas. Ejemplos: `userName`, `sessionDate`, `patientAge`.
- **Functions:** Las funciones se nombran en camelCase, utilizando verbos que describen la acción que realizan. Ejemplos: `getUserData()`, `createSession()`, `validateLogin()`.
- **Classes:** Las clases se nombran en PascalCase, iniciando cada palabra con mayúscula. Ejemplos: `TherapySession`, `UserProfile`, `AppointmentManager`.
- **Interfaces:** Se utilizará PascalCase para interfaces, representando estructuras de datos del dominio. Ejemplos: `Patient`, `SessionRecord`, `UserAccount`.
- **Constants:** Las constantes se escribirán en UPPER_CASE, separando palabras con guiones bajos. Ejemplos: `MAX_SESSIONS`, `API_URL`, `DEFAULT_TIMEOUT`.
- **Files:** Los archivos se nombran en kebab-case, usando palabras en minúscula separadas por guiones. Ejemplos: `user-profile.component.ts`, `session-service.js`.
- **Components:** Los componentes se nombran en PascalCase y deben reflejar su funcionalidad dentro del sistema. Ejemplos: `SessionCardComponent`, `LoginFormComponent`.
- **CSS Classes:** Se utilizará kebab-case para clases CSS, priorizando nombres descriptivos y reutilizables. Ejemplos: `main-container`, `primary-button`, `session-card`.

**Convenciones HTML:**
- Uso de HTML5 semántico (`section`, `article`, `nav`).
- Uso de etiquetas en minúscula.
- Indentación de 2 espacios.
- Clases descriptivas.

**Convenciones CSS:**
- Uso de kebab-case.
- Evitar IDs.
- Clases reutilizables.
- Separación por componentes.

**Convenciones JavaScript:**
- Uso de `const` y `let`.
- Evitar `var`.
- Funciones pequeñas.
- Uso de arrow functions.

**Convenciones TypeScript:**
- Tipado obligatorio.
- Evitar `any`.
- Uso de interfaces.
- Modularización.

**Convenciones Angular:**
- Estructura por módulos.
- Uso de servicios.
- Componentes reutilizables.

**Convenciones Java:**
- Clases en PascalCase.
- Métodos en camelCase.
- Encapsulamiento.

**Convenciones Spring Boot:**
- Arquitectura: Controller, Service, Repository.
- Uso de anotaciones estándar.

**Convenciones Gherkin:**
- Given / When / Then.
- Escenarios claros.

**Prácticas Adicionales:**
- Evitar duplicación de código (DRY).
- Mantener funciones cortas (< 20 líneas).
- Usar nombres descriptivos.
- Validar entradas de usuario.

---

### 5.1.4. Software Deployment Configuration

---

## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1

#### 5.2.1.1. Sprint Planning 1

En esta sección se especifican los aspectos principales del Sprint Planning Meeting del Sprint 1. A continuación se presenta el cuadro resumen de la reunión de planificación.

| Sprint # | Sprint 1 |
|---|---|
| **Sprint Planning Background** | |
| Date | 2026-04-21 |
| Time | 09:00 AM |
| Location | Reunión virtual mediante Google Meet |
| Prepared By | Lopez Torres, Leonardo Gabriel |
| Attendees (to planning meeting) | Lopez Torres, Leonardo Gabriel / Lopez Montalvo, Kevin Edu / Conde Huashuayo, Sebasthian Alex / Vilchez Vite, Gabriel Alejandro / Flores Chávez, Fabricio |
| Sprint 0 Review Summary | Al ser el primer sprint del proyecto, no existe un sprint anterior que revisar. Se parte desde cero con el levantamiento de requisitos, la definición del producto y la planificación inicial. |
| Sprint 0 Retrospective Summary | Al ser el primer sprint, no aplica retrospectiva de sprint anterior. El equipo realizó una sesión inicial de alineamiento para establecer acuerdos de trabajo, herramientas de colaboración y metodología a seguir durante el desarrollo del proyecto. |
| **Sprint Goal & User Stories** | |
| Sprint 1 Goal | Desarrollar la landing page completa y responsive de la plataforma, establecer los style guidelines del sistema de diseño y habilitar el flujo básico de acceso (registro, inicio de sesión y recuperación de contraseña) para los tres segmentos de usuario: padres de familia, profesores e instituciones terapéuticas. |
| Sprint 1 Velocity | 40 Story Points (Capacidad establecida para el equipo en este primer sprint, considerando la familiarización con el proyecto y la configuración del entorno de desarrollo.) |
| Sum of Story Points | 40 Story Points (Distribuidos en: Landing Page: 28 SP \| Style Guidelines: 10 SP \| Acceso básico EP01: 8 SP — con redondeo de 6 SP descontados por ajuste de velocidad inicial) |

---

#### 5.2.1.2. Aspect Leaders and Collaborators

En esta sección el equipo incluye la elaboración de un artefacto Leadership-and-Collaboration Matrix (LACX), que indique por cada aspecto dentro del alcance del Sprint, quién es el líder y quién o quiénes son colaboradores en dicho aspecto, con el fin de brindar mayor claridad y efectividad en la comunicación al interior del equipo. La sección incluye una introducción donde se explica cuáles son los principales aspectos que se toma en cuenta en el Sprint. Dependiendo del Sprint un aspecto puede ser un subconjunto del alcance funcional de la solución (por ejemplo feature, bounded context, etc.).

Los aspectos considerados en el Sprint 1 son: Landing Page, Style Guidelines, y Flujo de Acceso (Autenticación). Cada aspecto agrupa las User Stories relacionadas trabajadas durante este sprint.

| Team Member (Last Name, First Name) | GitHub Username  | Landing Page L / C | Style Guidelines L / C | Flujo de Acceso L / C |
|---|------------------|---|---|---|
| Flores Chávez, Fabricio | Elmiau2341       | L | C | C |
| Vilchez Vite, Gabriel Alejandro | GZ-99            | C | C | C |
| Lopez Torres, Leonardo Gabriel | Deiko-138        | C | L | C |
| Lopez Montalvo, Kevin Edu | Lopescamos       | C | C | L |
| Conde Huashuayo, Sebasthian Alex | SebasthianAlexCH | C | C | C |

---

#### 5.2.1.3. Sprint Backlog 1

El objetivo del Sprint 1 es establecer la base del producto TherapyConnect: desarrollar la landing page completa y responsive, definir los style guidelines del sistema de diseño y habilitar el flujo básico de acceso para los tres segmentos de usuario.

Trello: https://trello.com/invite/b/6a01270ea96c0a53e6826d61/ATTI1da43f25bafa713ad39a42e4bf04ea24CA66726B/therapyconnect-sprint-1

<img src="imagenes/Trello_Sprint1.png"> 


| User Story Id | User Story Title | Task Id | Task Title | Description | Estimation (Hours) | Assigned To | Status |
|---|---|---|---|---|---|---|---|
| US128 | Visualización de la landing page | T001 | Estructura base HTML | Crear el archivo index.html con la estructura semántica de todas las secciones de la landing. | 4h | Flores Chávez, Fabricio | Done |
| | | T002 | Estilos CSS globales | Implementar main.css con variables de color, tipografía y reset general del proyecto. | 4h | Flores Chávez, Fabricio | Done |
| | | T003 | Testing de carga y visualización | Verificar que la landing carga sin errores en distintos navegadores. | 2h | Vilchez Vite, Gabriel | Done |
| US129 | Sección Hero con llamada a la acción | T004 | Maquetación HTML del Hero | Implementar la estructura HTML con título, subtítulo y botón CTA. | 3h | Flores Chávez, Fabricio | Done |
| | | T005 | Estilos CSS del Hero | Aplicar estilos de fondo, tipografía, colores y alineación del Hero. | 3h | Flores Chávez, Fabricio | Done |
| | | T006 | Vincular CTA al registro | Configurar el enlace del botón 'Comenzar ahora' hacia el formulario de registro. | 2h | Lopez Torres, Leonardo | Done |
| US130 | Sección de funcionalidades principales | T007 | Maquetación HTML de funcionalidades | Implementar tarjetas de funcionalidades con íconos y textos descriptivos. | 4h | Vilchez Vite, Gabriel | Done |
| | | T008 | Estilos CSS de tarjetas | Aplicar estilos con hover y animaciones de entrada a las tarjetas. | 4h | Vilchez Vite, Gabriel | Done |
| US131 | Sección de segmentos objetivo | T009 | Maquetación HTML de segmentos | Crear las tres tarjetas para padres, instituciones y profesores con íconos representativos. | 4h | Conde Huashuayo, Sebasthian | Done |
| | | T010 | Interacción hover por segmento | Implementar la funcionalidad que muestra beneficios específicos al seleccionar cada tarjeta. | 4h | Conde Huashuayo, Sebasthian | Done |
| US132 | Sección de planes y precios | T011 | Maquetación HTML de planes | Implementar tarjetas de planes con nombre, precio, duración y lista de beneficios. | 4h | Flores Chávez, Fabricio | Done |
| | | T012 | Estilos y destacado del plan recomendado | Aplicar estilos y resaltar el plan recomendado con etiqueta o borde diferenciado. | 4h | Flores Chávez, Fabricio | Done |
| US133 | Sección de testimonios | T013 | Maquetación HTML de testimonios | Crear tarjetas con avatar, nombre y texto del comentario del usuario. | 3h | Vilchez Vite, Gabriel | Done |
| | | T014 | Implementar carrusel de testimonios | Desarrollar el carrusel en JavaScript con navegación por flechas y autoavance. | 5h | Vilchez Vite, Gabriel | Done |
| US134 | Sección de preguntas frecuentes (FAQ) | T015 | Maquetación HTML del FAQ | Implementar la estructura de acordeón con preguntas y respuestas. | 3h | Conde Huashuayo, Sebasthian | Done |
| | | T016 | Funcionalidad JS del acordeón | Implementar el despliegue y colapso de respuestas al hacer clic en cada pregunta. | 3h | Conde Huashuayo, Sebasthian | Done |
| US135 | Sección de contacto y footer | T017 | Maquetación HTML del footer | Implementar el footer con columnas de contacto, redes sociales y enlaces a términos. | 3h | Lopez Montalvo, Kevin | Done |
| | | T018 | Formulario de contacto y validación | Desarrollar el formulario de contacto con validación de campos y mensaje de confirmación. | 5h | Lopez Montalvo, Kevin | Done |
| US136 | Navegación interna de la landing page | T019 | Implementar menú de navegación | Crear el menú con enlaces a cada sección de la landing page. | 3h | Lopez Torres, Leonardo | Done |
| | | T020 | Scroll suave y menú fijo | Implementar desplazamiento suave entre secciones y menú fijo al hacer scroll. | 4h | Lopez Torres, Leonardo | Done |
| | | T021 | Menú hamburguesa para móvil | Implementar el menú hamburguesa responsive con funcionalidad de apertura y cierre. | 3h | Lopez Torres, Leonardo | Done |
| US137 | Diseño responsive de la landing page | T022 | Media queries para móvil | Agregar media queries CSS para adaptar el layout a pantallas de smartphone. | 6h | Flores Chávez, Fabricio | Done |
| | | T023 | Media queries para tablet | Agregar media queries CSS para el layout intermedio en dispositivos tablet. | 4h | Flores Chávez, Fabricio | Done |
| | | T024 | Testing responsive multi-dispositivo | Verificar la correcta visualización en distintos tamaños de pantalla y navegadores. | 2h | Vilchez Vite, Gabriel | Done |
| US-SG01 | Definición de paleta de colores | T025 | Seleccionar y definir paleta | Seleccionar colores primarios, secundarios y de estado para la plataforma. | 3h | Lopez Torres, Leonardo | Done |
| | | T026 | Documentar paleta en guía de estilos | Registrar códigos hexadecimales y uso de cada color en el documento de style guidelines. | 2h | Lopez Torres, Leonardo | Done |
| | | T027 | Aplicar variables CSS de paleta | Implementar las variables CSS (--color-primary, etc.) en el proyecto. | 3h | Lopez Torres, Leonardo | Done |
| US-SG02 | Definición de tipografía | T028 | Seleccionar fuente y escala tipográfica | Elegir la tipografía principal y definir tamaños H1-H4, cuerpo y etiquetas. | 3h | Lopez Torres, Leonardo | Done |
| | | T029 | Documentar tipografía en guía de estilos | Registrar fuente, tamaños y pesos tipográficos en el documento de style guidelines. | 2h | Lopez Torres, Leonardo | Done |
| US-SG03 | Componentes base de UI | T030 | Diseñar botones y variantes | Definir y maquetar estilos de botones (primario, secundario, deshabilitado) con estados hover y active. | 4h | Lopez Torres, Leonardo | Done |
| | | T031 | Diseñar inputs, cards y alertas | Definir y maquetar estilos de inputs, tarjetas y componentes de alerta con sus variantes. | 4h | Lopez Torres, Leonardo | Done |
| US-SG04 | Definición de espaciados y grilla | T032 | Definir sistema de grilla | Establecer número de columnas, gutter y márgenes para desktop, tablet y móvil. | 3h | Lopez Torres, Leonardo | Done |
| | | T033 | Documentar y aplicar espaciados | Registrar valores de espaciado y aplicar variables CSS en el proyecto. | 2h | Lopez Torres, Leonardo | Done |
| US01 | Registro de usuario | T034 | Maquetación HTML del formulario de registro | Implementar la pantalla de registro con campos de nombre, correo, contraseña y selector de rol. | 4h | Lopez Montalvo, Kevin | Done |
| | | T035 | Validación de campos del formulario | Implementar validaciones de campos obligatorios, formato de correo y longitud de contraseña. | 4h | Lopez Montalvo, Kevin | Done |
| | | T036 | Detección de correo duplicado | Implementar verificación para detectar correo ya registrado y mostrar mensaje de error. | 4h | Lopez Montalvo, Kevin | Done |
| | | T037 | Confirmación y redirección tras registro | Implementar mensaje de éxito y redirección al dashboard según el rol seleccionado. | 4h | Lopez Montalvo, Kevin | Done |
| US02 | Inicio de sesión | T038 | Maquetación HTML de la pantalla de login | Implementar la vista de inicio de sesión con campos de correo, contraseña y botón de ingreso. | 3h | Lopez Montalvo, Kevin | Done |
| | | T039 | Autenticación y redirección por rol | Implementar la lógica que valida credenciales y redirige al dashboard según el rol del usuario. | 6h | Lopez Montalvo, Kevin | Done |
| | | T040 | Mensaje de error en credenciales incorrectas | Mostrar mensaje claro cuando el correo o contraseña ingresados sean incorrectos. | 2h | Lopez Montalvo, Kevin | Done |
| US03 | Recuperación de contraseña | T041 | Pantalla de solicitud de recuperación | Implementar la vista donde el usuario ingresa su correo para solicitar el restablecimiento. | 3h | Conde Huashuayo, Sebasthian | Done |
| | | T042 | Envío de enlace de recuperación | Implementar el envío de correo con enlace seguro y temporizado para restablecer la contraseña. | 5h | Conde Huashuayo, Sebasthian | Done |
| | | T043 | Pantalla de nueva contraseña | Desarrollar el formulario donde el usuario define su nueva contraseña tras seguir el enlace. | 4h | Conde Huashuayo, Sebasthian | Done |
| US07 | Cierre de sesión seguro | T044 | Implementar botón de cierre de sesión | Agregar la opción de cerrar sesión en el menú, eliminar el token y redirigir al login. | 3h | Lopez Montalvo, Kevin | Done |
| | | T045 | Cierre automático por inactividad | Implementar el temporizador de inactividad que cierra la sesión y notifica al usuario. | 5h | Lopez Montalvo, Kevin | Done |

---

#### 5.2.1.4. Development Evidence for Sprint Review

| Repository | Branch | Commit Id | Commit Message | Committed on (Date) |
|---|---|---|---|---|
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | main | 13677da | doc: javascript | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | main | 9ff63a4 | Add main.css with base styles and layout | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | main | 29e223d | Update print statement from 'Hello' to 'Goodbye' | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | main | 8002da7 | Add mobile menu and language switch functionality | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | main | ddd2592 | Add initial CSS styles for the project | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | hotfix/fix-pages-index | db339dc | Merge branch 'hotfix/fix-pages-index' | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | hotfix/fix-pages-index | 8af213b | fix(pages): relocate index.html to public root. | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | hotfix/github-pages-deploy | e294786 | Merge branch 'hotfix/github-pages-deploy' | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | hotfix/github-pages-deploy | c66ca2f | fix: configure GitHub Pages deployment from public folder | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | release/v0.0.1 | d925511 | Merge branch 'release/v0.0.1' | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | release/v0.0.1 | fe1ld8e | fix(release): normalize contact placeholder information. | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | release/v0.0.1 | 7d61e80 | fix(release): replace empty footer placeholder links with non-navigable placeholders. | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | release/v0.0.1 | 62f432f | fix(release): add required validation to contact form fields | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | release/v0.0.1 | 4a6a864 | fix(release): remove obsolete inline onerror attribute from logo image. | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | main | dc69480 | fix(layout): correct asset paths in static resources | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | main | c5b6780 | feat(footer): implement footer section | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | main | 6a2f108 | feat(contact): implement contact form section | 04/25/2026 |
| https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect | main | cff85a2 | feat(pricing): implement pricing plans section | 04/25/2026 |

---

#### 5.2.1.5. Execution Evidence for Sprint Review

---

#### 5.2.1.6. Services Documentation Evidence for Sprint Review

Durante el Sprint 1, el alcance de implementación estuvo enfocado exclusivamente en el desarrollo y despliegue de la primera versión del Landing Page de TherapyConnect, así como en la definición del sistema de diseño base (Style Guidelines) y la habilitación del flujo de acceso básico (registro, inicio de sesión, recuperación de contraseña y cierre de sesión) a nivel de interfaz de usuario.

En consecuencia, no se ha realizado en este sprint el desarrollo de Web Services ni la implementación de endpoints RESTful, por lo que no existe documentación de servicios mediante OpenAPI/Swagger que reportar en esta entrega. La documentación de servicios será incorporada a partir del Sprint 2, cuando se inicie la implementación del backend con Spring Boot, conforme al plan de desarrollo establecido en el Product Backlog.

---

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

Durante el Sprint 1, el equipo Conecta realizó el despliegue de la primera versión pública de la Landing Page de TherapyConnect utilizando GitHub Pages, servicio gratuito y estático integrado directamente con el repositorio de GitHub.

**Plataforma de despliegue:** GitHub Pages — https://pages.github.com

**URL de la landing page desplegada:**
https://1asi0729-2610-11913.github.io/upc-pre-202610-1asi0729-11913-TherapyConnect-website/

**Proceso de despliegue realizado:**

1. Se creó el repositorio de la Landing Page bajo la organización GitHub del equipo: https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect.git
2. Se configuró la rama main como rama de producción del repositorio.
3. Todo el contenido estático de la landing page (HTML, CSS, JS) fue integrado a main mediante Pull Requests revisados por al menos un integrante del equipo, siguiendo el flujo GitFlow y Conventional Commits establecido.
4. En la sección Settings → Pages del repositorio, se seleccionó la rama main como fuente de publicación.
5. GitHub Pages generó automáticamente la URL pública y publicó el sitio estático.

---

#### 5.2.1.8. Team Collaboration Insights during Sprint

Durante el Sprint 1, el equipo Conecta utilizó GitHub como plataforma central de colaboración y control de versiones, aplicando el flujo de trabajo GitFlow junto con Conventional Commits y Semantic Versioning para mantener trazabilidad y orden en el desarrollo.

**Organización GitHub del equipo:**
https://github.com/1ASI0729-2610-11913/upc-pre-202610-1asi0729-11913-TherapyConnect.git

**Flujo de trabajo aplicado:**

- Cada integrante trabajó en ramas individuales siguiendo la convención `feature/US{id}-descripcion`, creadas desde la rama develop.
- Los cambios se integraron a develop mediante Pull Requests, requiriendo al menos una revisión y aprobación de otro integrante antes del merge.
- Los mensajes de commit siguieron el estándar Conventional Commits (`feat:`, `fix:`, `docs:`, `style:`, etc.), garantizando trazabilidad por funcionalidad.
- Al finalizar el sprint, develop fue fusionada a main para el despliegue en GitHub Pages.