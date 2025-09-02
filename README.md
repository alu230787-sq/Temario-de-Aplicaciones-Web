# Temario-de-Aplicaciones-Web
Accede a GitHub y crea un repositorio llamado Temario de Aplicaciones Web con el archivo README en donde investigarás con imágenes los temas propuestos.  

# 1.Introduccion al desarrollo web  

# Historia y evaluacion del desarrollo web: 

# 1. Orígenes: Web 1.0 (Década de 1990)  
1991: Tim Berners-Lee publica el primer sitio web y crea el protocolo HTTP y el lenguaje HTML.
Características: Sitios estáticos, solo texto e imágenes, navegación simple, sin interacción con el usuario.
Herramientas: HTML, CSS básico, navegadores primitivos como Mosaic y Netscape.  

# 2. Interactividad Inicial (Web 1.0 tardía)  
Aparecen los CGI scripts: Permiten formularios y respuestas dinámicas.
Lenguajes como Perl y PHP: PHP (1995), JavaScript (1995), permiten crear páginas más interactivas.
CSS: Introducido en 1996 para separar el contenido de la presentación.  

# 3. Web 2.0 (Años 2000)  
Características: Participación del usuario (wikis, blogs, redes sociales), contenido dinámico, AJAX para interactividad sin recargar la página.
Tecnologías clave: JavaScript, XML/JSON, frameworks como jQuery, aparición de CMS como WordPress.
Diseño Responsivo: Nace CSS3, se popularizan los móviles, surgen técnicas de diseño adaptable.

# 4. Frameworks y Librerías Modernas (2010 en adelante)  
Front-end: Surgen frameworks como Angular, React y Vue.js para crear interfaces ricas y reactivas.
Back-end: Node.js permite JavaScript en el servidor; frameworks como Django (Python), Ruby on Rails y Laravel (PHP) agilizan el desarrollo.
APIs REST y GraphQL: Facilitan la comunicación entre front-end y back-end.  

# 5. Web 3.0 y Tendencias Actuales  
Características: Inteligencia artificial, blockchain, aplicaciones descentralizadas (dApps), experiencia personalizada.  
PWA (Progressive Web Apps): Aplicaciones web que funcionan offline y tienen experiencia similar a la nativa.  
Jamstack: Arquitectura moderna que separa front-end, back-end y bases de datos, mejorando velocidad y seguridad.

# Resumen de la Evolución
De estática a interactiva: De páginas informativas a aplicaciones complejas.  
De monolíticas a modulares: Separación de responsabilidades entre front-end y back-end.  
De local a global: Acceso universal, optimización para múltiples dispositivos y regiones.  
La evolución del desarrollo web ha sido impulsada por la necesidad de mejorar la experiencia del usuario, la eficiencia en el desarrollo y la expansión de Internet a todos los aspectos de la vida moderna.

# Tipos de aplicaciones web (estáticas, dinámicas, SPA, PWA)

# 1. Aplicaciones web estáticas  
# Definición:  
Las páginas y el contenido no cambian en respuesta a la interacción del usuario.  

# Características:  
El servidor simplemente entrega archivos HTML, CSS e imágenes.  
No hay procesamiento en el servidor más allá de servir los archivos.  

# Ejemplo: 
Portafolios, sitios informativos sencillos.  

# Ventajas:  
Rápidas y seguras.  
Fácil mantenimiento.  

# Desventajas:  
No ofrecen personalización ni interactividad avanzada.  

# 2. Aplicaciones web dinámicas  
# Definición:
El contenido puede cambiar en función de la interacción del usuario o de datos almacenados en una base de datos.  

# Características:  
El servidor ejecuta código (PHP, Node.js, Python, etc.) para generar páginas personalizadas.

# Ejemplo:  
Tiendas en línea, sistemas de reservas, foros.

# Ventajas:  
Contenido personalizado.  
Funcionalidades avanzadas como registros, búsquedas, etc.  

# Desventajas:
Requiere programación y bases de datos.
Puede ser más complejo de mantener.

# 3. SPA (Single Page Application)
# Definición: 
Aplicación web que carga una sola página HTML y actualiza el contenido dinámicamente mediante JavaScript, sin recargar la página completa.  

# Características:  
Navegación fluida y rápida.  
Uso intensivo de frameworks como React, Angular, Vue.js.  
La comunicación con el servidor se realiza principalmente por AJAX/API.  

# Ejemplo: 
Gmail, Google Maps, Trello.

# Ventajas:  
Experiencia de usuario similar a una aplicación de escritorio.  
Menos recarga de páginas, mayor velocidad.  

# Desventajas:
SEO más complicado (aunque hay soluciones).
Inicialmente puede tardar más en cargar.

# 4. PWA (Progressive Web App)  
Definición: Aplicación web que utiliza tecnologías modernas para ofrecer una experiencia similar a la de una aplicación nativa, incluyendo funcionamiento offline y notificaciones.  
Características:  
Se instala en el dispositivo como una app.  
Funciona offline gracias a Service Workers.  
Permite notificaciones push y acceso a funcionalidades del dispositivo. 

# Ejemplo:
Twitter Lite, Starbucks.  
# Ventajas:  
Experiencia de usuario avanzada.  
Acceso desde el navegador o como app instalada.  
Mejor rendimiento y confiabilidad.  
# Desventajas:  
Requiere conocimientos avanzados de desarrollo web.  
Algunas funciones pueden estar limitadas según el navegador. 



# 2.Arquitectura de aplicaciones web

# Cliente-Servidor:  
divide un sistema en dos roles: el cliente, que solicita información y servicios a través de un navegador, y el servidor, que procesa estas peticiones y devuelve los datos necesarios. Esta interacción, que se basa en protocolos como HTTP, permite al cliente mostrar una interfaz de usuario interactiva mientras el servidor gestiona la lógica de negocio, el almacenamiento de datos y la entrega de recursos de forma centralizada. 

# Componentes principales  
## Cliente:  
Es la interfaz con la que el usuario interactúa directamente, generalmente a través de un navegador web. 
Responsabilidades: Mostrar la interfaz gráfica, recibir la entrada del usuario y enviar peticiones al servidor. 

## Ejemplos:  
Un navegador web que muestra un sitio de compras en línea o solicita un documento. 

## Servidor:
Es la máquina o software que aloja los recursos y servicios. 

## Responsabilidades:
Procesar las solicitudes de los clientes, gestionar la base de datos y la lógica de la aplicación, y enviar los datos solicitados de vuelta al cliente.  
Ejemplos: Un servidor web que entrega páginas HTML, CSS y JavaScript. 

# Cómo funciona  
1. Solicitud:  
El cliente (navegador) envía una solicitud de un servicio o datos a través de la red, usando un protocolo como HTTP.  
2. Procesamiento:  
El servidor recibe la solicitud, la procesa y accede a la información necesaria o ejecuta la lógica de la aplicación.   
3. Respuesta:  
El servidor envía los datos o la respuesta solicitada de vuelta al cliente.   
4. Presentación:  
El cliente recibe la respuesta y la utiliza para actualizar la interfaz de usuario y presentar la información al usuario de forma dinámica.

# Ventajas de esta arquitectura  
Seguridad:  
La centralización de los datos en el servidor permite una mejor gestión de la seguridad.  
Escalabilidad:  
Es posible escalar los recursos del servidor de forma independiente para satisfacer la demanda.  
Modularidad:  
La separación de funciones entre cliente y servidor facilita la gestión y el desarrollo de componentes.  
Optimización:  
Cada componente se enfoca en sus tareas específicas, lo que mejora el rendimiento general del sistema.  

# Arquitectura de tres capas (Presentacion, logica, datos)
# 1. Capa de Presentación

## Qué es:  
Es la interfaz con la que el usuario interactúa directamente.

## Responsabilidades:  
Mostrar la información al usuario (UI/UX).  
Recoger la entrada del usuario (formularios, clics).  
Enviar solicitudes al backend (generalmente vía HTTP/HTTPS). 

## Ejemplo:  
Un sitio web construido con HTML, CSS y JavaScript que muestra productos y permite realizar compras.  

# 2. Capa de Lógica de Negocio (o capa intermedia)   
## Qué es:  
Gestiona las reglas y procesos de la aplicación, actuando como intermediario entre la presentación y los datos.  

## Responsabilidades:  
Procesar las solicitudes del usuario.  
Aplicar reglas de negocio (validaciones, cálculos).  
Decidir cómo interactuar con la base de datos.  
# Ejemplo:  
Un sistema que verifica si hay stock de un producto antes de permitir la compra, o que calcula el precio final con descuentos.

# 3. Capa de Datos  
## Qué es:  
Gestiona el almacenamiento y recuperación de la información.  

## Responsabilidades:  
Acceder, modificar y almacenar datos (usando bases de datos como MySQL, PostgreSQL, MongoDB).
Proporcionar datos a la capa de lógica bajo demanda. Ejemplo:
Una base de datos que guarda la información de usuarios, productos, pedidos, etc.

# REST y API-first design
### ¿Qué es REST?
**REST (Representational State Transfer)** es un estilo arquitectónico para el diseño de servicios web. Se basa en el uso de HTTP para la comunicación entre cliente y servidor, siguiendo principios simples y estandarizados.

**Características clave de REST:**
- **Recursos:** Todo se representa como un recurso (usuarios, productos, etc.) identificado por una URL.
- **Métodos HTTP:** Se utilizan los métodos estándar de HTTP (GET, POST, PUT, DELETE) para realizar operaciones sobre los recursos.
- **Sin estado (stateless):** Cada solicitud del cliente al servidor debe contener toda la información necesaria; el servidor no almacena el estado de la sesión.
- **Formato de datos:** Usualmente se intercambian datos en formato JSON o XML.
- **Escalabilidad:** Al ser sencillo y usar HTTP, REST facilita la escalabilidad y la integración.

**Ejemplo de endpoints REST:**
- `GET /productos` — Obtiene la lista de productos.
- `POST /usuarios` — Crea un nuevo usuario.
- `PUT /productos/5` — Actualiza el producto con ID 5.
- `DELETE /usuarios/10` — Elimina el usuario con ID 10.

### API-first design

El **API-first design** es una metodología en la que el diseño y la definición de la API se realizan antes de comenzar el desarrollo de la aplicación. Esto permite que los equipos de frontend y backend trabajen de forma paralela y asegura una comunicación clara entre los componentes.  

**Ventajas de API-first:**  
- **Desarrollo paralelo:** Los equipos pueden avanzar al mismo tiempo sin esperar a que el otro termine su parte.  
- **Documentación clara:** El contrato de la API se define (por ejemplo, usando Swagger/OpenAPI), facilitando la integración y el mantenimiento.  
- **Consistencia:** Todas las aplicaciones y servicios se comunican siguiendo el mismo estándar.  
- **Escalabilidad:** Permite añadir nuevas funcionalidades o integrar otros servicios fácilmente.  

**Proceso típico:**  
1. Se diseña y documenta la API (endpoints, formatos de datos, autenticación).  
2. Se comparte la documentación con todos los equipos.  
3. Los equipos desarrollan sus componentes basándose en la API definida.  

**Herramientas comunes:**  
- **Swagger / OpenAPI:** Para diseñar, documentar y probar APIs.  
- **Postman:** Para probar y validar endpoints.  
- **RAML / API Blueprint:** Otros lenguajes para definir APIs.  

# 3. -Lenguajes y tecnologías fundamentales  
# HTML, CSS, JavaScript, PHP, MySQL  

### HTML (HyperText Markup Language)
Es el lenguaje de marcado principal para crear la estructura de las páginas web. Define los elementos como encabezados, párrafos, imágenes, enlaces, listas, formularios y mucho más.

- **Propósito:** Estructura del contenido.
- **Ejemplo:**
  ```html
  <h1>Bienvenido a mi sitio web</h1>
  <p>Este es un párrafo.</p>
  ```

### CSS (Cascading Style Sheets)
Se utiliza para darle estilo y presentación visual a las páginas web hechas con HTML. Permite definir colores, fuentes, márgenes, posiciones y adaptar el diseño a diferentes dispositivos (diseño responsivo).  

- **Propósito:** Diseño y apariencia.  
- **Ejemplo:**  
  ```css  
  body { background-color: #f0f0f0; }  
  h1 { color: #333; }  
  ```

### JavaScript  
Es el lenguaje de programación del navegador. Permite crear páginas web interactivas, dinámicas y responder a acciones del usuario sin recargar la página.  

- **Propósito:** Interactividad y dinamismo.  
- **Ejemplo:**  
  ```javascript  
  document.getElementById('boton').onclick = function() {  
    alert('¡Has hecho clic!');  
  };
  ```

### PHP (Hypertext Preprocessor)  
Lenguaje de programación del lado del servidor. Permite crear páginas web dinámicas que interactúan con bases de datos, procesan formularios y generan contenido personalizado.  

- **Propósito:** Lógica de servidor y generación dinámica de contenido.  
- **Ejemplo:**  
  ```php  
  <?php  
    echo "¡Hola, usuario!";  
  ?>  
  ```  

### MySQL  
Sistema de gestión de bases de datos relacional. Permite almacenar, consultar y manipular datos de forma eficiente. Es muy utilizado junto con PHP para crear aplicaciones web dinámicas.  

- **Propósito:** Almacenamiento y gestión de datos.  
- **Ejemplo de consulta SQL:**  
  ```sql  
  SELECT * FROM usuarios WHERE activo = 1;  
  ```  

---  

**Resumen:**    
- **HTML:** Estructura el contenido de la web.    
- **CSS:** Da estilo y diseño visual.  
- **JavaScript:** Añade interactividad en el navegador.  
- **PHP:** Programa la lógica del servidor y genera contenido dinámico.   
- **MySQL:** Almacena y gestiona los datos de la aplicación.  




# 4.-Control de versiones   
Git y GitHub  
Flujo de trabajo con ramas (branching, merge, pull requests)

# Propósito de Aprendizaje 2: Desarrollar componentes y funcionalidades de una aplicación web  
# 1.-Diseño e implementación del frontend
Maquetación/Wireframe/Mockup
API
# 2.-Diseño e implementación del backend
Servidor
Manejo de peticiones y respuestas HTTP
Conexión a bases de datos (MySQL, PostgreSQL, MongoDB)
# 3.-Bases de datos
 Modelado de datos y relaciones
ORM (Object Relational Mapping)
CRUD desde el backend
# 4.-Seguridad básica en aplicaciones web
Validación de formularios
Autenticación y autorización 

# Propósito de Aprendizaje 3: Implementar y desplegar una aplicación web funcional
1. -Integración de frontend y backend  
Interfaz de usuario Frontend  
Manejo de API  
Proceso de Solicitud y Respuesta de Backend  

2.- Almacenamiento en Servidor  
Tipos de servidores   
Servidores y servicios de hosting   
Proveedores de Servicios de Almacenamiento  

3.-Optimización y rendimiento  
Optimización de recursos (imágenes, scripts)  
Despliegue de aplicaciones web  
CI/CD básico  
Documentación del proyecto  

