# Guía editorial para la web personal de Nicolás Bazaes

Base de revisión: 3 de noviembre de 2026. Documento editable para futuras modificaciones de [nbazaes.dev](https://nbazaes.dev). Se revisaron el listado de repositorios de GitHub, README públicos y archivos seleccionados de las copias locales: contenido del portafolio, manifiestos y evidencia del kernel. Es una revisión editorial, no una auditoría funcional de cada aplicación.

## 1. Intención y posicionamiento

Preferencias acordadas: combinar empleo, clientes y una presentación personal/pasional. El README de GitHub está en inglés. La web conserva español e inglés. Linux, servidores propios, experimentación y herramientas para necesidades cercanas deben tener espacio propio.

**Propuesta central:** desarrollo aplicaciones para necesidades concretas y me involucro también en la infraestructura que las mantiene funcionando.

El visitante debería entender quién es Nicolás, explorar algo que construyó y encontrar cómo contactarlo. Un reclutador puede profundizar en arquitectura y código; un cliente, en el problema resuelto; alguien con intereses similares, en Linux y proyectos personales.

### Hechos e impresiones

| Evidencia observada | Interpretación editorial |
| --- | --- |
| BazPOS reúne React, API Django, roles, datos y despliegue Docker. | Hay una historia de desarrollo que se extiende hasta la operación. Usarlo como caso principal. |
| Discursantes aborda la programación de oradores de una congregación local. | La motivación comunitaria ayuda a contar quién está detrás del código. |
| FamilyApp combina Android, backend propio y sincronización. | La curiosidad técnica se aplica también a la vida cotidiana y al control sobre los datos. |
| MarkIt Desktop envuelve un conversor existente con una interfaz. | Interés por hacer herramientas técnicas más cómodas de usar. |
| El repositorio del kernel conserva un cambio pequeño, pruebas y revisión. | Buen ejemplo de investigación y resolución de un problema concreto. |
| La web tiene terminal interactiva y contenido ES/EN con Astro. | La afinidad por la consola ya tiene una expresión personal que conviene conservar. |

Estas impresiones orientan el relato; no acreditan años de experiencia, seniority, resultados económicos ni niveles de dominio. No deducir esas afirmaciones del número de repositorios o dependencias.

## 2. Proyectos y evidencia

Los enlaces son públicos. Las tecnologías describen la documentación revisada; no certifican disponibilidad de demos ni pruebas completas de las funciones.

| Prioridad | Proyecto y fuente | Problema y tecnologías | Uso recomendado |
| --- | --- | --- | --- |
| Principal | [BazPOS](https://github.com/nbazaes/django-bazpos) | Gestión comercial: ventas, inventario, proveedores, devoluciones y caja. React, Django REST Framework, MariaDB, Docker Compose, Gunicorn y nginx según README. | Caso de estudio: problema, flujo, separación de responsabilidades y despliegue. Reutilizar su presentación existente. |
| Diferenciador | [Linux kernel patches](https://github.com/nbazaes/linux-kernel-patches) | Selección automática SMBus/RMI4 para el touchpad ThinkPad E490, ID LEN2058. Registro de pruebas, revisión, integración y backports. | Bloque breve con evidencia y explicación del problema en lenguaje común. |
| Destacado | [MarkIt Desktop](https://github.com/nbazaes/markit-desktop) | Interfaz para convertir archivos a Markdown con MarkItDown. Tauri, Svelte y Python según README y manifiesto local. | Herramienta y exploración personal. Atribuir el motor de conversión a Microsoft. |
| Destacado | [Discursantes](https://github.com/nbazaes/discursantes_react) | Programación de oradores, fechas, temas e historial. React confirmado; backend pendiente de reconciliar entre versiones. | Historia comunitaria; evitar mezclar tecnologías de distintas implementaciones. |
| Destacado | [FamilyApp](https://github.com/nbazaes/family-app) | Compras, tareas, calendario y gastos. Kotlin, Jetpack Compose, almacenamiento local, sincronización y FastAPI según README; backend FastAPI corroborado localmente. | Proyecto personal que amplía el perfil hacia Android y servicios propios. |
| Secundario | [Facturas SII](https://github.com/nbazaes/descargar-facturas-sii) | Descargas por folio con Python y Selenium; conserva progreso según README. | Ejemplo de automatización. No llamarlo integración oficial ni garantizar compatibilidad actual del portal. |
| Secundario | [TicketOps AI](https://github.com/nbazaes/ticketops-ai) | Clasificación de reportes con FastAPI, PostgreSQL, Astro, Ollama y LM Studio según README. | Experimento de IA aplicada. Evitar cifras de precisión sin evaluación. |
| Secundario | [Asistente de Cocina](https://github.com/nbazaes/asistente-cocina) | Recetas, despensa e importación con Expo, React Native y TypeScript según documentación y manifiesto local. | Muestra adicional de curiosidad; omitir versiones del texto editorial. |
| Contexto | [Portafolio Astro](https://github.com/nbazaes/landing-astro) | Sitio bilingüe con páginas estáticas y terminal interactiva. | Enlace al código desde el pie o terminal; priorizar otros proyectos en portada. |
| Comercial opcional | [Constant: código público](https://github.com/nbazaes/webconstAD) | README público: Astro SSR, Django REST Framework, PostgreSQL y R2. Existen implementaciones distintas. | Confirmar versión vigente antes de asociar código y sitio comercial o describir compras. |

### Evidencia de Linux

El registro público y la copia local de `synaptics-len2058-e490/upstream.patch` identifican el commit `16ca52bc209fa4bf9239cd9e5643e95533476b58`, la autoría, el ID LEN2058 y pruebas sin parámetro manual. El repositorio documenta integración y backports. Se incluye el [commit oficial](https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/commit/?id=16ca52bc209fa4bf9239cd9e5643e95533476b58) como fuente primaria; el navegador de esta sesión no pudo recuperarlo directamente.

Texto recomendado: «Contribuí un cambio al driver Synaptics para habilitar automáticamente SMBus/RMI4 en el touchpad del ThinkPad E490». Para fechas y versiones, enlazar la tabla del repositorio y comprobarla antes de reproducir su detalle. No extrapolar este cambio a experiencia general en desarrollo de drivers.

## 3. Textos propuestos ES/EN

Propuestas listas para adaptar. Mantener el sentido entre idiomas, con redacción natural en cada uno.

### Presentación inicial

**ES — Título:** Construyo aplicaciones y cuido los sistemas que las hacen funcionar.

**ES — Introducción:** Soy Nicolás Bazaes, desarrollador y entusiasta de Linux en Los Ángeles, Chile. Trabajo con Python, Django y React, automatizo tareas y alojo mis propios servicios. Muchos de mis proyectos nacen de algo cercano: un negocio, mi comunidad o una herramienta que quiero usar en casa.

**EN — Headline:** I build applications and look after the systems that keep them running.

**EN — Introduction:** I'm Nicolás Bazaes, a developer and Linux enthusiast based in Los Ángeles, Chile. I work with Python, Django, and React, automate tasks, and host my own services. Many of my projects start close to home: a business, my community, or a tool I want to use myself.

Botón principal: **Ver proyectos / Explore my projects**. Secundario: **Contactar / Get in touch**. Mantener **Abrir terminal / Open terminal** como invitación adicional.

### Biografía personal

**ES:** Me interesa entender qué ocurre detrás de una aplicación: cómo se organiza la lógica, dónde viven los datos y cómo mantener el servicio funcionando. Por eso vuelvo al backend y a Linux, aunque también disfruto construyendo la interfaz. Mis proyectos me han llevado a probar herramientas de escritorio, aplicaciones Android y modelos de lenguaje locales. Alojar mis propios servicios me da un lugar para experimentar y aprender con cosas que uso.

**EN:** I like understanding what happens behind an application: how the logic is organized, where the data lives, and how to keep the service running. That's why I keep coming back to backend development and Linux, though I enjoy building the interface too. My projects have taken me into desktop tools, Android apps, and local language models. Hosting my own services gives me somewhere to experiment and learn with things I use.

### Descripciones para fichas

| Proyecto | Español | English |
| --- | --- | --- |
| BazPOS | Aplicación de punto de venta y gestión comercial que reúne ventas, inventario, proveedores y caja. React en la interfaz, Django en la API y MariaDB para los datos. | A point-of-sale and business management application bringing sales, inventory, suppliers, and cash register closing together. React on the frontend, Django for the API, and MariaDB for storage. |
| MarkIt Desktop | Interfaz de escritorio para MarkItDown de Microsoft, con conversión por lotes y vista previa de Markdown. Construida con Tauri, Svelte y Python. | A desktop interface for Microsoft's MarkItDown, with batch conversion and Markdown previews. Built with Tauri, Svelte, and Python. |
| Discursantes | Aplicación React para organizar oradores, fechas y temas de una congregación local, con historial de participaciones. | A React application for organizing speakers, dates, and topics in a local congregation, with a history of past assignments. |
| FamilyApp | Organizador familiar autoalojable para compras, tareas, calendario y gastos, con cliente Android y backend FastAPI. | A self-hosted family organizer for shopping, tasks, calendars, and expenses, with an Android client and a FastAPI backend. |
| Linux | Cambio al driver Synaptics para seleccionar automáticamente SMBus/RMI4 en el ThinkPad E490, integrado en el kernel de Linux. | A Synaptics driver change enabling automatic SMBus/RMI4 selection on the ThinkPad E490, merged into the Linux kernel. |

### Contacto

**ES:** ¿Tienes una oportunidad de desarrollo, un proyecto en mente o ganas de conversar sobre Linux y servidores propios? Escríbeme a nbazaes@bazaes.cl.

**EN:** Have a development opportunity, a project in mind, or an interest in Linux and self-hosting? Reach me at nbazaes@bazaes.cl.

### Metadatos

**Título ES:** Nicolás Bazaes | Desarrollo web y Linux

**Título EN:** Nicolás Bazaes | Web Development & Linux

**Descripción ES:** Desarrollador en Chile. Aplicaciones con Python, Django y React, automatización y servicios autoalojados. Explora mis proyectos y mi contribución al kernel de Linux.

**Descripción EN:** Developer based in Chile. Python, Django, and React applications, automation, and self-hosted services. Explore my projects and my contribution to the Linux kernel.

## 4. Voz y selección

- Primera persona. Explicar para quién sirve algo y qué permite hacer, seguido de tecnología y una decisión concreta.
- Equilibrar proyectos comerciales y personales. BazPOS muestra amplitud; Discursantes, comunidad; FamilyApp y MarkIt Desktop, intereses propios.
- Sustituir «dominio de Linux» por acciones comprobables: alojar servicios, desplegar con Docker o investigar el comportamiento del touchpad.
- Priorizar Python/Django, React y Linux/Docker. Presentar las demás tecnologías como herramientas utilizadas o exploraciones, sin porcentajes de dominio.
- Conservar la terminal y ofrecer navegación convencional, enlaces claros y correo accesible.
- Respetar atribuciones: MarkItDown es de Microsoft; MarkIt Desktop es la interfaz propia. Conservar las notas de asistencia de IA existentes al contar el proceso de los proyectos.
- No inventar disponibilidad laboral vigente, títulos académicos, seniority, clientes, usuarios, ahorro o ingresos. La situación académica del README anterior necesita confirmación.
- Separar capacidades implementadas, planes y resultados medidos. Gestionar facturas en un POS no implica emisión tributaria certificada.
- No publicar detalles de repositorios privados por haber tenido acceso a ellos. Esta guía usa enlaces públicos para las afirmaciones propuestas.

## 5. Aplicación futura en Astro

Repositorio identificado: `landing-astro`, copia local `/home/nicolas/Desarrollo/landing_astro`. Esta entrega no lo modifica ni publica la web. Antes de editarlo, leer sus instrucciones locales y revisar Git.

### Estructura recomendada

Conservar BazPOS como caso principal. Mostrar después la contribución Linux como bloque de evidencia, seguido de MarkIt Desktop, Discursantes y FamilyApp. Dejar automatización e IA como proyectos adicionales. Añadir la biografía cerca de la presentación o de «Cómo trabajo». Cerrar con contacto.

### Fuentes de contenido existentes

| Fuente | Aplicación |
| --- | --- |
| `src/content/profile.md` | Identidad, contacto y metadatos compartidos. Mantener dominio y enlaces salvo cambio confirmado. |
| `src/content/site/es.md` y equivalente `en.md` | Hero, stack, principios y textos de terminal. Mantener el mismo relato en ambos idiomas. |
| `src/content/projects/` | Fichas, orden, destacado, nombre visible, arquitectura y enlaces. Mantener BazPOS como destacado. |
| `src/content.config.ts` | Validar los campos existentes antes de añadir claves o cambiar el esquema. |
| `src/lib/engineering.ts` | Ejemplos concretos de arquitectura y operación, coherentes con las fichas. |

Usar el esquema actual cuando alcance: `category`, `description` y `metrics` tienen ES/EN; `githubUrl` es obligatorio y `demoUrl` opcional. `metrics` contiene también capacidades cualitativas: no inventar cifras. No rellenar enlaces con destinos privados o ficticios. Un futuro caso sin código público requeriría adaptar explícitamente su presentación.

Hoy no existe un campo específico de biografía en el perfil. Se puede incorporar al texto inicial y a `terminal.readmeLines`. Una sección propia requerirá un cambio explícito de esquema y componentes; no introducir claves sin consumidor. Conservar las rutas, cambio de idioma y navegación sin JavaScript.

### Discrepancias a resolver

| Hallazgo | Acción |
| --- | --- |
| README de Discursantes: Express/MariaDB y sin autenticación. Web y manifiesto local: Clerk/Supabase. | Comprobar rama y código del despliegue elegido. Las dependencias no prueban funcionamiento. Hasta reconciliarlo, usar descripción funcional con React. |
| Ficha de Constant: Django/SQLite. README público: Astro/Django/PostgreSQL/R2. Existe otra implementación local. | Identificar la versión documentada y desplegada. No asociar automáticamente el repositorio con el sitio actual ni anunciar pagos habilitados sin comprobarlos. |
| Stack de la web: Go, GraphQL y Redis sin evidencia suficiente en esta revisión. | Retirarlos de destacados o aportar proyecto y uso concreto. Incorporar MariaDB, documentada en BazPOS. |
| MarkIt Desktop conserva enlaces de instalación y clonación hacia Microsoft. | Enlazar el repositorio propio y comprobar sus releases antes de prometer instaladores. La corrección de su README es tarea separada. |
| La web indica disponibilidad y el perfil anterior mencionaba estudios. | Confirmar vigencia antes de actualizar esos datos. Los textos propuestos evitan depender de ellos. |

### Verificación de una futura edición

1. Revisar coherencia de portada, terminal, fichas y metadatos ES/EN.
2. Ejecutar `npm run validate` para tipos y build, y `npm test` si se cambian textos o comportamiento de terminal.
3. Comprobar portada y rutas inglesas, enlaces, correo, teclado y móvil. Contenido principal y navegación deben funcionar sin JavaScript.
4. Comprobar la presentación existente de BazPOS, capturas, video, subtítulos y enlace a demo. Verificar la demo antes de anunciar disponibilidad actual.
5. Revisar localmente antes de publicar. No hay cambios de APIs ni dependencias previstos por esta guía.

## 6. Prompt reutilizable

```text
Actualiza el contenido de mi web usando PERSONAL_WEBSITE_GUIDE.md y mi
README de perfil como base editorial. Quiero combinar empleo y clientes
con una presentación personal: Linux, self-hosting, curiosidad y proyectos
que resuelven necesidades cercanas.

Lee las instrucciones del repositorio y revisa su estado actual.
Conserva Astro bilingüe, la terminal y la presentación de BazPOS.
Aplica los textos ES/EN en las fuentes existentes y mantén coherencia
entre portada, terminal, fichas y metadatos. Cambia el esquema solo si
el contenido lo requiere y actualiza también sus consumidores.

Prioriza BazPOS, la contribución concreta a Linux, MarkIt Desktop,
Discursantes y FamilyApp. Resuelve las discrepancias registradas antes
de afirmar tecnologías, pagos, producción o disponibilidad de demos.
Si no puedes resolverlas con evidencia, usa una descripción funcional
y señala lo pendiente. Respeta las atribuciones. Usa evidencia pública
para afirmaciones publicadas y no inventes métricas, experiencia ni
información biográfica vigente.

Ejecuta las comprobaciones correspondientes y revisa ES/EN, móvil,
teclado y navegación sin JavaScript. Entrega los cambios y limitaciones.
No publiques ni hagas push como parte de esta tarea.
```
