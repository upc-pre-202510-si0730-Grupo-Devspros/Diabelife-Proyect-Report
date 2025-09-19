# Capítulo V: Product Implementation, Validation & Deployment.

En esta sección se describen las decisiones y lineamientos que garantizan consistencia en el desarrollo del proyecto.

# 5.1. Software Configuration Management.

En esta sección se presentan los productos de software empleados en el proyecto, cuyos enlaces correspondientes se encuentran disponibles en los anexos

# 5.1.1. Software Development Environment Configuration.

##### Project Management:

- Trello: Es una herramienta de gestión de proyectos basada en el método Kanban, utilizada para planificar tareas y asignar responsabilidades al equipo. Permite organizar el trabajo en tableros, listas y tarjetas, lo que facilita la visualización del flujo de actividades, el seguimiento del progreso de cada tarea y la colaboración en tiempo real entre los miembros del equipo. Además, se emplea para documentar los Sprint Backlogs, asignar responsables, establecer fechas de entrega y mantener la trazabilidad de las User Stories y tareas durante el desarrollo del proyecto.

##### Product UX/UI Design:

- Figma: Herramienta colaborativa utilizada para el diseño de wireframes, mock-ups y prototipos interactivos de las interfaces web.
- PlantUML: Utilizado para la elaboración de diagramas de clases, permitiendo representar la estructura del sistema, sus clases, atributos, métodos y las relaciones entre ellas de manera clara y estandarizada.
- Uxpressia: UXPressia: Herramienta utilizada para la creación de User Personas, Empathy Maps, Journey Maps e Impact Maps. Facilita la representación de perfiles de usuarios, sus motivaciones, necesidades y puntos de dolor, así como la visualización del recorrido del usuario y el impacto de las decisiones de diseño en la experiencia global del sistema.
-  Structurizr: Utilizado para la elaboración de diagramas del C4 Model en los niveles Context, Container y Component, con el fin de representar de manera clara la arquitectura del sistema y la relación entre sus elementos principales.
-  Lucidchart: Utilizado para la creación de diagramas de base de datos, facilitando la representación de entidades, atributos y relaciones entre tablas, así como la validación visual del modelo de datos.

#### Software Development

- JetBrains Rider: IDE que se usará para el desarrollo del backend en C# de nuestra aplicación.
- WebStorm: IDE especializado para el desarrollo frontend. Se utilizará para la creación de la Landing Page y el frontend de la aplicación en Vue.js.
- Visual Studio Code: Editor utilizado únicamente para la exportación del reporte de formato markdown a PDF.
- GitHub: Plataforma de control de versiones y colaboración.

#### Software Deployment

- GitHub Pages: Servicio de despliegue de aplicaciones web estáticas desde repositorios GitHub.
- Netlify: Plataforma que se utilizará para el despliegue del frontend de nuestra aplicación web.
- Azure: Plataforma en la nube que se utilizará para el despliegue del backend de la aplicación desarrollado en .NET en futuros sprints.



# 5.1.2. Source Code Management.

Para administrar el código fuente, se empleará GitHub como herramienta principal de control de versiones y espacio de colaboración entre los integrantes del equipo. Se han configurado repositorios independientes para cada uno de los productos del proyecto, cuyos enlaces pueden consultarse en la sección de anexos.

- **Organización en GitHub:** [https://github.com/upc-pre-202510-si0730-Grupo-Devspros](https://github.com/upc-pre-202510-si0730-Grupo-Devspros)
- **Repositorio del informe final:** [https://github.com/upc-pre-202510-si0730-Grupo-Devspros/Diabelife-Proyect-Report](https://github.com/upc-pre-202510-si0730-Grupo-Devspros/Diabelife-Proyect-Report)
- **Repositorio de la Landing Page:** [https://github.com/upc-pre-202510-si0730-Grupo-Devspros/Diabelife-Landing-Page](https://github.com/upc-pre-202510-si0730-Grupo-Devspros/Diabelife-Landing-Page)

### Modelo de ramificación: GitFlow

Se optó por utilizar GitFlow como estrategia de ramificación para el desarrollo. Este enfoque brinda una organización clara de las ramas y favorece el trabajo colaborativo entre los desarrolladores.

En el repositorio destinado al informe final se establecieron las siguientes ramas:

- dev: Rama central de desarrollo, en la que se unificarán todas las nuevas funcionalidades y ajustes de errores.

- chapter-1: Rama destinada a la elaboración del capítulo 1 del informe.

- chapter-2: Rama destinada a la elaboración del capítulo 2 del informe.

- chapter-3: Rama destinada a la elaboración del capítulo 3 del informe.

- chapter-4: Rama destinada a la elaboración del capítulo 4 del informe.

- chapter-5: Rama destinada a la elaboración del capítulo 5 del informe.


### Estilo de commits: Conventional Commits

Con el fin de mantener mensajes de commits claros y consistentes, se adoptará la convención Conventional Commits. Algunos ejemplos de uso son:

- feat: Add search by name functionality
- fix: Correct form validation error
- docs: Update installation instructions
- refactor: Simplify calculation logic

Los prefijos de categoría se emplearán con el siguiente significado:

- feat: A new feature
- fix: A bug fix
- docs: Documentation only changes
- style: Changes that do not affect the meaning of the code (formatting, missing semicolons, etc.)
- refactor: A code change that neither fixes a bug nor adds a feature
- test: Adding missing tests or correcting existing ones
- chore: Changes to the build process or auxiliary tools

# 5.1.3. Source Code Style Guide & Conventions.
En esta sección se definen las convenciones de nombres y codificación adoptadas por el equipo para los lenguajes utilizados en el proyecto: HTML, CSS, JavaScript y C#. El idioma estándar para todo el código (nombres de variables, funciones, clases, archivos, etc.) es el inglés.

#### Principios generales

- Idioma estándar: Todo el código fuente debe escribirse en inglés, incluyendo nombres de archivos, clases, variables y funciones.

- Prioridad a la legibilidad: Se privilegia el uso de nombres claros y descriptivos por encima de abreviaturas o tecnicismos innecesarios.

- Formato consistente: Se mantiene un estilo uniforme en todo el equipo y en todos los lenguajes, apoyado por herramientas automáticas.

- Nombres semánticos: Los sustantivos se emplean para clases, componentes y archivos, mientras que los verbos se utilizan en funciones o métodos.

- Indentación: 2 espacios para HTML, CSS y JavaScript; 4 espacios para C#.

### HTML5 y CSS3

**HTML5**

- Los archivos deben tener la extensión .html.

- Se recomienda el uso de etiquetas semánticas como <header>, <section>, <nav>, <footer>, entre otras.

- Todas las imágenes deben contar con el atributo alt, y se utilizan atributos aria-* para garantizar accesibilidad.

- Los atributos se escriben siempre entre comillas dobles (").

- Para los identificadores (id) se aplica camelCase, mientras que para las clases se emplea kebab-case.

- La indentación establecida es de 2 espacios.

**CSS3**

- Los archivos deben guardarse con la extensión .css.

- Los nombres de clases y archivos siguen la convención kebab-case, por ejemplo: main-header, product-card, login-form.

- Los estilos relacionados se organizan en bloques y se separan mediante comentarios para facilitar la lectura.

**JavaScript**

- Los archivos deben guardarse con la extensión .js.

- Para variables y funciones se emplea la convención camelCase, por ejemplo: userName, getUserData().

- Las clases y componentes utilizan PascalCase, como UserProfile o LoginForm.

- Se prioriza el uso de const y let en lugar de var.

- Se recomienda utilizar funciones flecha (=>) y nombres claros y descriptivos.

- Cada archivo debe enfocarse en una sola responsabilidad o componente

Basado en:
- [Guía de estilo JavaScript de Google](https://google.github.io/styleguide/jsguide.html?utm_source=chatgpt.com)
**C#**

- Los archivos deben tener la extensión .cs.

- Las clases y componentes utilizan PascalCase, por ejemplo: UserService o OrderController.

- Los métodos y variables se escriben en camelCase, como getUserById() o userEmail.

- Las constantes se definen en UPPER_SNAKE_CASE, por ejemplo: MAX_ATTEMPTS.

- Se recomienda una clase pública por archivo.

- Los métodos y clases públicas deben incluir documentación mediante XML comments (///) para mantener buenas prácticas de documentación.

Basado en:

- [Guía de estilo C# de Microsoft](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions?utm_source=chatgpt.com)
- [Buenas prácticas para .NET](https://learn.microsoft.com/en-us/dotnet/standard/design-guidelines/)
# 5.1.4. Software Deployment Configuration.
# 5.2. Landing Page, Services & Applications Implementation.
# 5.2.1. Sprint 1
# 5.2.1.1. Sprint Planning 1.
# 5.2.1.2. Aspect Leaders and Collaborators.
# 5.2.1.3. Sprint Backlog 1.
# 5.2.1.4. Development Evidence for Sprint Review.
# 5.2.1.5. Execution Evidence for Sprint Review.
# 5.2.1.6. Services Documentation Evidence for Sprint Review.
# 5.2.1.7. Software Deployment Evidence for Sprint Review.
# 5.2.1.8. Team Collaboration Insights during Sprint.
# Conclusiones
# Bibliografía
# Anexos