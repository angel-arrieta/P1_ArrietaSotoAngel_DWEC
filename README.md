# Gestor de Pagos

La aplicación web que he ideado es para mi grupo scout tiene el propósito de ofrecer a los padres una herramienta sencilla y clara para consultar el estado de los pagos realizados y pendientes de sus hijos, sin embargo, solo es de consulta, no permite realizar pagos a través de la plataforma. La interfaz está optimizada para brindar una experiencia intuitiva tanto para los padres como para el tesorero de mi grupo.

## Analisis de mercado

Al buscar información sobre otros gestores de pagos, he encontrado el gestor Sage y la herramienta SoportNet, estos son sistemas de gestión de pagos mucho más amplios, orientados a un espectro más amplio de organizaciones o empresas, sin embargo he enfocado la aplicación en el entorno scout con una funcionalidad simplificada

### - Diferenciación

 - Transparencia: Los padres pueden estar al tanto en todo momento del estado de los pagos de sus hijos, evitando confusiones o retrasos.

 - Control Administrativo: El tesorero puede gestionar fácilmente los pagos, actualizando la información de manera centralizada y en tiempo real.

 - Simplicidad: La plataforma es intuitiva, diseñada para que tanto padres como administradores puedan navegar sin complicaciones.

### - Funcionalidades

 - **Login de Usuario**

    - Cada padre dispondrá de un usuario y contraseña únicos para acceder a la plataforma. El sistema asegurará la autenticación segura de cada usuario, garantizando la privacidad de los datos.
    - Una vez autenticado, el usuario tendrá acceso a la lista de sus hijos registrados en el grupo scout.

 - **Vista de Hijos**

    - Tras el inicio de sesión, el usuario podrá ver una lista con los nombres de sus hijos que pertenecen al grupo scout.
    - Al seleccionar a uno de sus hijos, el padre será redirigido a una página donde podrá visualizar el estado detallado de los conceptos de pago asignados a dicho hijo.

 - **Estado de Pagos**

    - En la vista de cada hijo, los padres podrán consultar los diferentes conceptos que se deben pagar (como cuotas de actividades, uniformes, campamentos, etc.).
    - Junto a cada concepto, se mostrará si el concepto ha sido pagado o si está pendiente, acompañado del monto correspondiente.
    - Si el concepto está pagado, se mostrará una indicación clara del estado de "Pagado", mientras que si está pendiente, el estado será "No pagado".
    - Al lado del estado de cada concepto se detallará la cantidad de dinero a pagar o la cantidad ya pagada.

 - **Cuenta del Tesorero (Administrador)**

    - El tesorero tendrá un usuario especial con permisos ampliados.
    - Podrá acceder a los datos de todos los niños del grupo scout y ver el estado de los pagos de cada uno.
    - El tesorero podrá cambiar el estado de los conceptos de pago entre "Pagado" y "No pagado" según reciba las contribuciones de los padres.
    - Además, podrá editar los nombres de los conceptos de pago, agregar nuevos conceptos o eliminar antiguos.
    - También podrá ajustar las cuantías de cada concepto según lo que se decida para las diferentes actividades o cuotas.

## Investigación de tecnologías y herramientas para Desarrollo el Web

Tras haber descrito mi programa de la forma más ideal, me dispongo a realizar un analisis de las herramientas que puedo disponer para llevar a cabo el proyecto.

### Modelos de Ejecución

La ejecución de código en el lado cliente se utiliza principalmente para mejorar la interacción y la experiencia del usuario, reduciendo la latencia y el tiempo de respuesta, ya que no necesita solicitar constantemente información al servidor. Los lenguajes más comunes son JavaScript o TypeScript, que permiten la manipulación dinámica del DOM y la actualización de la interfaz de usuario sin recargar la página.

 - Ventajas

    - Menor carga en el servidor, lo que reduce los costos de infraestructura.
    - Mejora de la experiencia del usuario al reducir la latencia en ciertas operaciones.
    - Permite interfaces más dinámicas y reactivas.

 - Desventajas

    - El rendimiento depende de los recursos del dispositivo del cliente (CPU, memoria).
    - Puede ser poco seguro, ya que el código está expuesto en el navegador.

### Diferencias entre Lenguajes Web

####  JavaScript

- Ventajas

    - Popularidad y compatibilidad universal: Es el único lenguaje de programación nativo de los navegadores, soportado en todos ellos sin necesidad de plugins.
    - Ecosistema amplio: Tiene un ecosistema de bibliotecas y frameworks como React, Angular o Vue.js, que facilitan el desarrollo de aplicaciones complejas.
    - Interactividad: Permite la manipulación del DOM y la creación de interfaces de usuario interactivas en tiempo real.
    - Desempeño en cliente: Ejecuta código directamente en el navegador, mejorando la capacidad de respuesta y la experiencia del usuario.

- Desventajas

    - Falta de tipado estático: Puede provocar errores en tiempo de ejecución debido a errores de tipificación.
    - Rendimiento: En aplicaciones muy grandes o mal optimizadas, el rendimiento puede verse afectado.

#### TypeScript

- Ventajas

    - Tipado estático: A diferencia de JavaScript, TypeScript es un superconjunto que añade tipos estáticos, lo que mejora la seguridad y reduce errores en tiempo de ejecución.
    - Herramientas de desarrollo: Mejora la experiencia de desarrollo con mejores autocompletados y detección temprana de errores en el código.
    - Escalabilidad: Ideal para proyectos grandes y colaborativos, ya que facilita la comprensión y mantenimiento del código.

- Desventajas

    - Requiere compilación: Necesita compilarse a JavaScript antes de ejecutarse en el navegador.
    - Curva de aprendizaje: Si bien es similar a JavaScript, los desarrolladores deben aprender nuevas características y sintaxis.

### Tecnologías Disponibles

 - **HTML/CSS (Lenguajes de marcas)** son esenciales para construir la estructura y diseño de la interfaz.

 - **React.js**: Es un framework JavaScript muy popular que facilita la creación de interfaces de usuario dinámicas, basado en componentes reutilizables. Facilita el manejo del estado de la aplicación y la actualización del DOM.

 - **Node.js con Express.js**: Node.js es un entorno de ejecución en servidor basado en JavaScript. Express es un framework minimalista para crear APIs, es ideal para aplicaciones en tiempo real y permite que el frontend y el backend compartan el mismo lenguaje (JavaScript/TypeScript), facilitando el desarrollo integrándose así perfectamente.

### Herramientas de Desarrollo

- Visual Studio Code (VS Code)
    - **Funciones**: Editor de código liviano con una amplia gama de extensiones que admiten tecnologías como JavaScript, TypeScript, React y Node.js. Ofrece depuración, autocompletado y Git integrado.
    - **Ventajas**: Popular, fácil de usar, multiplataforma y con una amplia gama de extensiones.
- Git/GitHub
    - **Funciones**: Control de versiones distribuido. GitHub permite la colaboración y almacenamiento de código en la nube.
    - **Ventajas**: Facilita la gestión de versiones y colaboración entre desarrolladores.
- Webpack/Babel
    - **Funciones**: Webpack es un empaquetador de módulos que permite optimizar los archivos para el frontend. Babel transpila el código TypeScript o ES6+ a una versión de JavaScript compatible con todos los navegadores.
    - **Ventajas**: Optimiza el rendimiento y garantiza la compatibilidad en navegadores.

### Compatibilidad en Navegadores

Los navegadores manejan de manera diferente algunas funciones avanzadas de JavaScript, como las nuevas características de ECMAScript. Además, algunos navegadores pueden tener un rendimiento desigual al ejecutar scripts muy grandes o pesados, se puede solucionar empleando las siguientes herramientas.

 - **Babel**: Transpila código moderno a una versión más compatible, asegurando que las características de ES6+ se ejecuten en navegadores antiguos.
 - **Polyfills**: Se pueden agregar para implementar características faltantes en navegadores antiguos.