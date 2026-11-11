#  👔Etrevistas backend java👔

## ✒️Resumen laboral

Utiliza el método STAR (Situación, Tarea, Acción, Resultado)

###  Domi
Trabaje un año en el proyecto de domiciliaciones desarrollando servicios sencillos y dando soporte a la aplicación. 

###  Azteca 360 02/2019 – 03/2023
(Detalla el proceso desde el análisis hasta el mantenimiento, incluyendo cualquier problema que surgió y cómo lo resolviste.) 
Posteriormente participe en un proyecto nuevo que es una plataforma de pagos que expone medios de pago para instituciones internas y externas al grupo, dentro de mis funciones eran realizar servicios, realizar pruebas y estaba encargado de administrar las API Proxies del proyecto desde el análisis, creación, pruebas, liberación y mantenimiento así como el acompañamiento a los clientes que se fueron integrando. Los últimos meses trabaje en una migración de Tibco a spring boot. 
Las tecnologías que utilice para el desarrollo de los microservicios son Spring Boot con Java 8, para la documentación swagger y para las pruebas JUnit, Docker y JMeter de lado de APIGEE ocupaba swagger con open api 2.0 para la creación de yaml, apigee, utilizábamos la estrategia de api first. En ambas tareas utilizaba git para el manejo de versiones y la integracion continua, asi como jira y confluence para el manejo de las historias de usuraio. 

###  Kairos (Santanter) 05/2023 – 03/2025
Trabajé desarrollando microservicios con Spring Boot 3 y Java 17 en un proyecto de crédito. Los servicios que desarrollé incluyen un microservicio para la generación de contratos, una librería para el manejo de errores, e implementamos Kafka para la mejora de los tiempos de respuesta de los servicios de una aplicación de solicitud de tarjeta de crédito. (Explicar por qué se eligió Kafka, cómo se implementó y los beneficios obtenidos.)

###  WIZELINE (GRUPO SALINAS) 05/2025 – 03/2026
Desarrollé de una funcionalidad de monitoreo basada en Kafka, permitiendo la captura y persistencia de respuestas de error para análisis posterior. Posteriormente, en el proyecto de Shopin Baz, asumí la responsabilidad de la certificación del ecosistema backend, donde gestioné la resolución de vulnerabilidades críticas detectadas por Checkmarx y aseguré el cumplimiento de estándares normativos mediante la documentación técnica rigurosa en plataformas institucionales.

### Ejemplos de retos en mi carrera
Aprender y capacitarme en nuevas tecnologías son retos importantes en mi carrera pero es algo que me gusta hacer, por ejemplo, con APIGEE nos dieron una capacitación muy básica y tuve que leer mucho la documentación para entender mejor los procesos. 

### 5 Habilidades y debilidades

#### Habilidades

- **Manejo de APIs y Arquitectura API-First:** Diseño y administración de APIs con Apigee, OpenAPI y Swagger, asegurando una integración eficiente.
- **Resiliencia:** Capacidad de adaptación aprendiendo rápidamente nuevas tecnologías y ajustándome a cambios.
- **Trabajo en Equipo:** Experiencia colaborando en equipos ágiles.
- **Autodidacta:** He aprendido algunas tecnologías por mi cuenta capacitándome con cursos y documentación. 

#### Debilidades

- **Delegación de Tareas:** Suelo querer resolver todo por mi cuenta, pero estoy mejorando en confiar más en el equipo y distribuir responsabilidades.
- **Experiencia con Frontend:** Mi enfoque ha sido backend, pero estoy explorando tecnologías frontend para comprender mejor el desarrollo full stack.
- **Comunicación Técnica:** Explicar conceptos complejos a perfiles no técnicos me ha sido un reto, pero he mejorado documentando de manera clara y concisa de la mano con IA.

---
##  ☕Java Puro

### Programación orientada a objetos

>Paradigma de programación que parte del concepto de "objetos" como base.

4 pilares de la POO
- Abstracción: Es el proceso de identificar las características esenciales de un objeto, ignorando los detalles de implementación irrelevantes para el sistema. Se logra mediante el uso de Interfaces y Clases Abstractas, permitiendo enfocarnos en el "qué hace" un objeto en lugar del "cómo lo hace".
- Encapsulamiento: Es el ocultamiento del estado interno de un objeto, obligando a que toda interacción se realice a través de métodos públicos (interfaz del objeto). Su objetivo principal es la integridad de los datos y la reducción del acoplamiento.
- Polimorfismo: Capacidad de una entidad (método u objeto) de referirse a instancias de distintos tipos o presentar diferentes comportamientos bajo un mismo nombre.
    Por lo general diremos que existen 3 tipos de polimorfismo:
  - Sobrecarga: Definir múltiples métodos con el mismo nombre en la misma clase, pero con diferente firma (distinto número o tipo de parámetros). Se resuelve en tiempo de compilación.
  - Paramétrico: En Java, esto se conoce principalmente como Generics. Permite definir clases o métodos que operan sobre tipos de datos genéricos sin comprometerse con uno específico hasta su instanciación.
  - Sobreescritura: Una subclase proporciona una implementación específica de un método que ya está definido en su clase padre o interfaz.
- Herencia: Mecanismo que permite crear nuevas clases (subclases) a partir de clases existentes (superclases), estableciendo una relación de jerarquía. (Reutilizar código).

**Modificadores de acceso**

| |Clase Propia|Paquete|SubClase|Publico|
|-------- |------------|-------|--------|-------|
|Private  |✔|✘|✘|✘|
|Default  |✔|✔|✘|✘|
|Protected|✔|✔|✔/✘|✘|
|Public   |✔|✔|✔|✔|
> Protected: El detalle técnico es que permite el acceso a subclases incluso si están en paquetes diferentes, pero solo a través de la herencia (no por instancia directa).

**Colecciones**: 

***1. Interfaz Collection***
Es la raíz de la jerarquía. Define las operaciones básicas como add(), remove(), size(), y contains().
> Sub-interfaces principales: List, Set, Queue.

***2. Interfaz List***
Define una colección ordenada (por índice) que permite elementos duplicados.
> Implementaciones clave: ArrayList, LinkedList, Vector.

***3. Interfaz Set***
Una colección que no permite elementos duplicados. Modela la abstracción matemática de un conjunto.
Sub-interfaz SortedSet: Para conjuntos que garantizan un orden (ej. TreeSet).
> Implementaciones clave: HashSet, LinkedHashSet.

***4. Interfaz Queue (Cola)***
Diseñada para retener elementos antes de ser procesados, siguiendo generalmente el principio FIFO (First-In-First-Out).
Sub-interfaz Deque: Una cola de doble terminación (permite insertar/eliminar por ambos extremos).
> Implementaciones clave: PriorityQueue, ArrayDeque.

***5. Interfaz Map***
¡Ojo aquí! En las entrevistas suelen preguntar esto: Map no hereda de Collection. Es una interfaz independiente porque opera con pares llave-valor.
Sub-interfaz SortedMap: Mantiene las llaves ordenadas.
> Implementaciones clave: HashMap, TreeMap, LinkedHashMap.


**¿Qué es una lambda?**
Es una función anónima (sin nombre) que permite tratar la funcionalidad como un argumento de método o el código como datos.
- Se introdujeron a partir de Java 8

**Supplier**: Es una interfaz funcional que no recibe argumentos y devuelve un resultado de tipo T. Se utiliza para generar valores de forma perezosa o diferida. La interfaz Supplier 
tiene un único método llamado `get()` que devuelve un valor de tipo T.
> Ejemplo: Uso de Optional.orElseGet(() -> new Resource()). A diferencia de orElse(), el Supplier solo se ejecuta si el Optional está vacío (Lazy Evaluation).

**Consumer**: Es una interfaz funcional que toma un argumento de tipo T y no devuelve ningún resultado. Se utiliza para realizar operaciones con el objeto de tipo T, como imprimirlo 
en la consola o almacenarlo en una base de datos. La interfaz Consumer tiene un único método llamado `accept(T t)`. Ejem. forEach() para realizar una acción en cada elemento, como imprimir.
> Ejemplo: list.forEach(System.out::println); (Aquí también puedes mencionar el uso de Method References ::).

**Predicate**: Es una interfaz funcional que toma un argumento de tipo T y devuelve un valor booleano. Se utiliza para evaluar una condición sobre el objeto de tipo T. 
La interfaz Predicate tiene un único método llamado `test(T t)`. Ejem. el método filter() para filtrar elementos de un Stream basándose en una condición.
> Ejemplo: stream.filter(user -> user.getAge() > 18).

**Function**: Es una interfaz funcional que toma un argumento de tipo T y devuelve un resultado de tipo R. Se utiliza para transformar objetos de tipo T en objetos de tipo R. 
La interfaz Function tiene un único método llamado `apply(T t)`. Ejem. el método map() para transformar elementos de un Stream, como convertir cadenas a sus longitudes.
> Ejemplo: stream.map(String::toUpperCase).


**¿Qué es Java Stream?**
En la versión 8 de Java se incluyó un API que facilitaba en gran medida el trabajo con colecciones. Este nos permite realizar operaciones sobre la colección, como por ejemplo buscar, 
filtrar, reordenar, reducir, etc…
> Un Stream no modifica la fuente original; genera un nuevo resultado o una nueva vista de los datos.
Tipos de Operaciones

**Para la entrevista, clasifica las operaciones así:**
Operaciones Intermedias: Devuelven un nuevo Stream. Son "lazy".
filter(Predicate): Filtra elementos.
map(Function): Transforma cada elemento.
sorted(): Ordena los elementos.
distinct(): Elimina duplicados.

**Operaciones Terminales: Inician el procesamiento y cierran el Stream.**
collect(): Transforma el Stream a una colección (List, Set, Map).
forEach(Consumer): Itera sobre los resultados.
reduce(): Combina elementos en un solo valor.
count(): Retorna el número de elementos.

**Pregunta de examen: ¿Cuál es la diferencia entre map() y flatMap()?**
Respuesta: map transforma un elemento en otro. flatMap se usa cuando cada elemento genera un Stream y quieres "aplanar" todos esos sub-streams en uno solo (ej. convertir una lista de listas en una sola lista plana).

**static**
La directiva static permite el acceso a métodos y variables de clase sin la necesidad de instanciar un objeto de dicha clase.
Static significa que el miembro (método o variable) pertenece a la clase en lugar de a una instancia específica.

- Variables Estáticas: Existe una sola copia de la variable para todas las instancias. Se usa comúnmente para constantes o contadores globales.

- Métodos Estáticos: Pueden ser llamados sin crear un objeto.
 - Restricción: No pueden acceder a miembros de instancia (this o super) porque no están asociados a ningún objeto.

**Novedades de JAVA 8**
- Lambdas
- Stream
- Java.time

**Novedades de Java 11**
- Inferencia de tipos en datos primitivos.
- Metodo estatico of en colecciones.

**Novedades de Java 17**
- Records: Similar a lombook se agregan getters (aunque no comienza por get), equals(), toString() y hashCode().
- Sealed Classes: Permiten restringir qué clases pueden extender o implementar una clase o interfaz.
- Mejora en instanceof: Ahora, puedes evitar hacer un casting explícito después de usar instanceof. Si la condición de instanceof es verdadera, automáticamente puedes usar la variable en el bloque.

```
Object obj = "Hello, Java!";

//Antes
if (obj instanceof String) {
    String str = (String) obj;  // casting manual
    System.out.println(str.toUpperCase());
}

//Mejora
if (obj instanceof String str) {  // Pattern Matching
    System.out.println(str.toUpperCase());
}
```

---
##  🍃SPRING

**Spring**: Framework de java para delegar tarear repetitivas. Con el uso de anotaciones.

**Spring boot**: Proyecto basado en Spring para la creacion de aplicaciones autocontenidas. Contiene propio servidor de aplicaciones embebido e incluye gestor de dependencias como Gradle y Maven.

**Spring data**: Proyecto para gestionar y usar bases de datos. A360 usa Srping data. Contiene otros proyectos como Spring Data JPA.

**Spring security**: Autenticacion, autorizacion y gestion de seguridad. Autenticacion por JWT.

**Inyección de dependencias**:
Principio de diseño utilizado para lograr una alta cohesión y un bajo acoplamiento. Sus principales funciones son evitar la instanciación de un objeto hasta que se requiera y desacoplar del objeto mediante interfaces, respetando así el principio de "Open/Close" de SOLID.
Se puede inyectar una dependencia mediante las anotaciones @Autowired, @Inject y @Qualifier, o utilizando el constructor de la clase que lo utilizará.
https://www.youtube.com/watch?v=_zBYWFo2l78

**Inversión de Control**:
✍

**Interseptor**:
✍

**Dependencia**: 
✍

###  Anotaciones

**Estereotipos**
- **@Component**: Anotacion general (padre) de estereotipos. Es para implem       entaciones mas generales como clases de seguridad.
- **@Controller**: Etiqueta que respresnta el diseño (metodos http, repustas, etc.).
  - **@RestController**: Etiqueta que respreseta que es un servicio rest (responde un formato JSON).
- **@Service**: Indica que la clase contendra la logica de negocio.       
- **@Repository**: Indica que la clase interactua con la base de datos.

**JPA**
- **@Entity**: Indica a java que esta representando a una tabla de base de datos.
- **@Table**: Recibe el nombre de la tabla que esta mapeando nuestra clase.
- **@Column**: Se pone cuando nombre de la tabla es diferente al de la clase.
- **@Id**: Representa el primary key.
- **@Embededid**: Representa el primary key es compuesta.
- **@GeneretedValue**: Genera valores para llaves primarias.
- **@OneToMany** ManyToOne: Relaciones entre tablas.

**Spring Boot**
- **@SpringBootApplication**: Esta anotación se utiliza en la clase de aplicación al configurar un proyecto Spring Boot. Clase main que debe ejecutar.
- **@RestController**: Indica que la clase sera un controlador de una API rest.
  - **@RequestBody**: Indica que el objeto de entrada sera el body.
  - @PathVariable: Indica el nombre del path parameter.
- **@RequestMapping**: Indica un path base
  - **@GetMapping**: Indica el path del recurso y que su verbo http es GET.
  - **@PostMapping**: Indica el path del recurso y que su verbo http es POST.
  - **@PutMapping**: Indica el path del recurso y que su verbo http es PUT.
  - **@DeleteMapping**: Indica el path del recurso y que su verbo http es DELETE.
- **@Autowired**: Anotación para inyectar una dependencia e instanciar con el contenedor de inversion de control de Spring.

---

##  💬Kafka
✍

---

##  📌Adicionales

**Git**: Control de versiones

**5 principios S.O.L.I.D. de diseño de aplicaciones de software**
- **S** – Single Responsibility Principle (SRP): Principio de Responsabilidad Única: Cada clase o módulo debe tener una única responsabilidad o motivo de cambio. Esto ayuda a que el código sea más fácil de mantener y menos propenso a errores.
- **O** – Open/Closed Principle (OCP): Principio de Abierto/Cerrado: Las entidades de software (clases, módulos, funciones) deben estar abiertas para extensión, pero cerradas para modificación. Esto significa que podemos agregar nuevas funcionalidades sin alterar el código existente.
- **L** – Liskov Substitution Principle (LSP): Principio de Sustitución de Liskov: Las subclases deben ser sustituibles por sus clases base sin alterar el comportamiento esperado del programa. Esto asegura que el código funcione correctamente cuando se utiliza una subclase en lugar de su clase base.
- **I** – Interface Segregation Principle (ISP): Principio de Segregación de Interfaces: Los clientes no deben estar obligados a depender de interfaces que no usan. Es mejor tener interfaces específicas y pequeñas en lugar de interfaces grandes y generales. En otras palabras, una clase no debe implementar una interfaz con métodos que no va a utilizar.
- **D** – Dependency Inversion Principle (DIP): Principio de Inversión de Dependencias: Los módulos de alto nivel no deben depender de los módulos de bajo nivel, sino de abstracciones (interfaces). Esto permite que los módulos sean menos dependientes entre sí y facilita el cambio o la implementación de nuevas funcionalidades.
    
**Maven**: Herramienta de software para la gestión y construcción de proyectos.

**Docker**: Herramineta que automatiza el despliegue de aplicaciones dentro de contenedores de software. (Funciona como un servidor).
- docker build . -t microservice-security:v1 (Se crea imagen con los datos del archivo dockerfile).
- docker run -p 8080:8081 --name microservice-security microservice-security:v1 (Crear contenedor).

**JUnit**: Herramienta para la implementacion de pruebas al proyecto de spring.

**JMeter**: Herramineta para realizar pruebas de estres.

**Swagger**: 
- **@ApiOperation**: Agrear descripcion a un recurso.
- **@ApiResponse**: Codigo y mensaje de respuesta ejemplo(code = 200, message = "OK")
- **@ApiParam**: (required = true, value = "")

**Microservicios**: Es un enfoque de arquitectura donde se cubren necesidades particulares de un contexto.

## JWT

### ¿Qué es?
Es un token utilizado para la autenticación de usuarios.

### ¿Qué partes componen un JWT?
- Header: Contiene el algoritmo de cifrado.
- Payload: Contiene el mensaje a compartir.
- Signature: Clave/Contraseña y la conbinación de header y payload.

### ¿Cómo se genera un JWT en un microservicio con spring?

1. Clase para generar y firmar el token JWT.
2. Validar las credenciales (por ejemplo, en un AuthenticationManager), generar el JWT y lo devuelverlo al cliente.

### ¿Cómo validas un JWT en un microservicio con spring?

1. Se crea una clase component donde que decodifica y extrae la información.
2. Se crea filter donde interceptas las solicitudes.
   - Se valida token
3. Se incluye el filter en spring security (clase config).

---
##  📐Patrones de diseño

### Patrones creacionales
> Estos patrones proporcionan mecanismos de creación de objetos que incrementan la flexibilidad y la reutilización del código existente.
- Builder
  - El patrón nos permite producir distintos tipos y representaciones de un objeto empleando el mismo código de construcción.
  - Digamos que tenemos un constructor con **diez parámetros opcionales**. Invocar a semejante bestia es poco práctico, por lo que sobrecargamos el constructor y creamos varias versiones más cortas con menos parámetros. Estos constructores siguen recurriendo al principal, pasando algunos valores por defecto a cualquier parámetro omitido.
    ~~~
    class Pizza {
        Pizza(int size) { ... }
        Pizza(int size, boolean cheese) { ... }
        Pizza(int size, boolean cheese, boolean pepperoni) { ... }
    ~~~
  - Se utilizan cuando existen multiples parametro para un constructor como ejemplo las configuraciones de dependencias para spring.
- Singleton: Patrón de diseño creacional que nos permite asegurarnos de que una clase tenga una única instancia (static) y un punto de acceso global.
  - En A360 se utiliza para instanciar las credenciales de apigee.
- Factory
- Abstract Factory

###  Patrones estructurales
> Estos patrones explican cómo ensamblar objetos y clases en estructuras más grandes, mientras se mantiene la flexibilidad y eficiencia de la estructura.
- Proxy
- Adapter
- Decorador

### Patrones de comportamiento
> Estos patrones tratan con algoritmos y la asignación de responsabilidades entre objetos.

- Command
- Strategy
- Observer

### Patrones específicos de Microservicios
> En sistemas distribuidos y basados en eventos, algunos patrones específicos son fundamentales:

- Circuit Breaker:
  - Este patrón evita que un servicio siga haciendo llamadas fallidas a otro servicio cuando éste está caído o responde lentamente. Es común en arquitecturas distribuidas para mejorar la resiliencia. Hystrix o Resilience4j son bibliotecas comunes que implementan este patrón.

- Saga:
  - Permite manejar transacciones distribuidas mediante la coordinación de varios pasos en diferentes servicios, de modo que, si uno de los pasos falla, cada servicio ejecuta una "acción compensatoria" para deshacer el trabajo realizado.

- Event Sourcing:
  - En lugar de almacenar solo el estado actual de una entidad, se almacenan todos los eventos que llevaron a ese estado. Esto facilita el seguimiento de cambios históricos y es útil para sistemas auditables o en aplicaciones financieras.

- Retry:
 - Reintentar automáticamente llamadas fallidas a un servicio externo, especialmente en casos de fallos transitorios (como problemas de red temporales).

- Bulkhead:
 - Divide recursos para evitar que un fallo en una parte afecte a todo el sistema. 

- Rate Limiting:
 - Controlar la cantidad de solicitudes que un servicio puede recibir en un período de tiempo determinado.

---
## 🤔Preguntas Frecuentes

**¿Qué es un API Gateway y cómo puede mejorar la arquitectura de microservicios?**
    Es una puerta de entrada de peticiones a múltiples servicios, sirve como filtro, balanceo de carga, caching, autenticación, monitorización y para ofuscar las rutas de los servicios.

**¿Que hacer cuando algo falla en produccion?**
    Replicar el error en desarrollo

**¿Diferencia entre clase abstracta e interfaz?**
    - La clase se extiende y la interfaz se implementa.
    - Clase abstracta solo es obligatorio implementar los metodos abstractos.

**API**:
    API es el acrónimo de interfaz de programación de aplicaciones (application programming interface en inglés). Es un conjunto de reglas bien definidas que se utilizan para especificar formalmente la comunicación entre dos componentes de software.
    Apiproxy un medio para exponer servicios a un tercero permite agregar caracteristicas como seguridad, cuotas, analitica.

**API REST**
    Una API REST es una interfaz de comunicación entre sistemas de información que usa el protocolo de transferencia de hipertexto (hypertext transfer protocol o HTTP, por su siglas en inglés) para obtener datos o ejecutar operaciones sobre dichos datos en diversos formatos, como pueden ser XML o JSON.

**REST**
    REST es una arquitectura de desarrollo web que puede ser utilizada en cualquier cliente HTTP.

**API RESTfull**
    Es un API que implementa la arquitectua REST.

**Diferencia de restcontroller y controller**
	RestController responde un formato JSON.

**Seguridad en apis**
✍

**Diferencia entre spring y spring boot**
    Spring boot es un prroyecto basado en spring y facilita el despliegue de aplicaciones con servidores embebidos

**¿Que es un bean?**
    Un objeto que es ensamblado y administrado por un contenedor de Spring IoC.

**¿Cual es la diferencia entre jpa y hibernate?**
    Hibernate sirve para el mapeo objeto-relacional (ORM) facilita el mapeo de atributos entre una base de datos relacional tradicional y el modelo de objetos de una aplicación

**Idempotencia**
	- **Definición de idempotencia:** La idempotencia es una propiedad de una operación en matemáticas e informática que hace que ejecutar la misma solicitud varias veces produzca exactamente el mismo estado y resultado del sistema que ejecutarla una sola vez.
	- Métodos idempotentes (GET, PUT, DELETE)
	- Métodos no idempotentes (POST, PATCH)
	- Hacer que un servicio sea idempotente: El cliente genera un UUID único y lo envía en los encabezados HTTP; esto es fundamental para evitar duplicados (como cargos dobles o registros repetidos) cuando ocurren fallos de red y el cliente reintenta la petición.
	
**Que es una interfaz funcional?**
 	- Es una interfaz que tiene exactamente un método abstracto. Se utiliza como el pilar fundamental para la programación funcional.
	- Para asegurarte de que cumple esta regla, se utiliza la anotación `@FunctionalInterface`. Si alguien intenta agregar un segundo método abstracto por error, el compilador generará un fallo.

