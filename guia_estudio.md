# 👔Etrevistas backend java👔

## ✒️Resumen laboral

Utiliza el método STAR (Situación, Tarea, Acción, Resultado)

### Domi
Trabaje un año en el proyecto de domiciliaciones desarrollando servicios sencillos y dando soporte a la aplicacion.

### Azteca 360 
(Detalla el proceso desde el análisis hasta el mantenimiento, incluyendo cualquier problema que surgió y cómo lo resolviste.)
Posteriormente participe en un proyecto nuevo que es una plataforma de pagos que expone medios de pago para instituciones internas y externas al grupo, dentro de mis funciones eran realizar servicios, realizar pruebas y estaba encargado de administrar las API Proxies del proyecto desde el analisis, creacion, pruebas, liberacion y mantenimiento asi como el acompañamiento a los clientes que se fueron integrando. Los utimos meses trabaje en una migracion de Tibco a spring boot.
Las tecnologias que utilice para el desarrollo de los microservicios son Spring Boot con Java 8, para la documentacion swagger y para las pruebas JUnit, Docker y JMeter de lado de APIGEE ocupaba swagger con open api 2.0 para la creacion de yaml, apigee, utilizabamos la estrategia de api first. En ambas tareas utilizaba git para el manejo de versiones y la integracion continua, asi como jira y confluence para el manejo de las historias de usuraio.

### Kairos (Santanter)
Trabajé desarrollando microservicios con Spring Boot 3 y Java 17 en un proyecto de crédito. Los servicios que desarrollé incluyen un microservicio para la generación de contratos, una librería para el manejo de errores, e implementamos Kafka para la mejora de los tiempos de respuesta de los servicios de una aplicación de solicitud de tarjeta de crédito. (Explicar por qué se eligió Kafka, cómo se implementó y los beneficios obtenidos.)

### Ejemplos de retos en mi carrera
Aprender y capasitarme en nuevas tecnologias son retos importantes en mi carrera pero es algo que me gusta hacer, por ejemplo, con APIGEE nos dieron una capasaitacion muy basica y tuve que leer mucho la documentación para entender mejor los procesos. 

### 5 Habilidades y debilidades
✍

---
## ☕Java Puro

### Programación orientada a objetos

>Paradigma de programación que parte del concepto de "objetos" como base.

4 pilares de la POO
- Abstracción: Es la capacidad de obtener la información relevante para resolver un problema.
- Encapsulamiento: Es la habilidad de poder decidir las partes que se expondrán a hacia otras entidades. Este pilar apunta a ocultar o publicar atributos o métodos dependiendo del caso.
- Polimorfismo: Construir metodos con el mismo nombre pero comportamiento diferente.
    Por lo general diremos que existen 3 tipos de polimorfismo:
  - Sobrecarga: El más conocido y se aplica cuando existen funciones con el mismo nombre en clases que son completamente independientes una de la otra.
  - Paramétrico: Existen funciones con el mismo nombre pero se usan diferentes parámetros (nombre o tipo). Se selecciona el método dependiendo del tipo de datos que se envíe.
  - Inclusión: Es cuando se puede llamar a un método sin tener que conocer su tipo, así no se toma en cuenta los detalles de las clases especializadas, utilizando una interfaz común.
- Herencia: Es la capacidad de transferir características propias como atributos y métodos de una clase a otra. (Reutilizar código).

**Modificadores de acceso**

| |Clase Propia|Paquete|SubClase|Publico|
|-------- |------------|-------|--------|-------|
|Private  |✔|✘|✘|✘|
|Default  |✔|✔|✘|✘|
|Protected|✔|✔|✔/✘|✘|
|Public   |✔|✔|✔|✔|


**Colecciones**: 
- **List**: Lista ordenada de objetos.
- **Set**: Coleccion desordenada de objetos unicos.
- **Map**: Coleccion llave valor.


**¿Qué es una lambda?**
Un lambda es un concepto relacionado con la programación funcional que se definió en Java 8 para tratar de dotar a Java de un paradigma funcional que difiere del paradigma de la 
programación imperativa.

**Supplier**: Es una interfaz funcional que no toma argumentos y devuelve un resultado de tipo T. Se utiliza para generar valores de forma perezosa o diferida. La interfaz Supplier 
tiene un único método llamado get() que devuelve un valor de tipo T1.

**Consumer**: Es una interfaz funcional que toma un argumento de tipo T y no devuelve ningún resultado. Se utiliza para realizar operaciones con el objeto de tipo T, como imprimirlo 
en la consola o almacenarlo en una base de datos. La interfaz Consumer tiene un único método llamado accept(T t)1.

**Predicate**: Es una interfaz funcional que toma un argumento de tipo T y devuelve un valor booleano. Se utiliza para evaluar una condición sobre el objeto de tipo T. 
La interfaz Predicate tiene un único método llamado test(T t)1.

**Function**: Es una interfaz funcional que toma un argumento de tipo T y devuelve un resultado de tipo R. Se utiliza para transformar objetos de tipo T en objetos de tipo R. 
La interfaz Function tiene un único método llamado apply(T t)1.


**¿Qué es Java Stream?**
En la versión 8 de Java se incluyó un API que facilitaba en gran medida el trabajo con colecciones. Este nos permite realizar operaciones sobre la colección, como por ejemplo buscar, 
filtrar, reordenar, reducir, etc…

**static**
La directiva static permite el acceso a métodos y variables de clase sin la necesidad de instanciar un objeto de dicha clase
✍

**Novedades de JAVA 8**
- Lambdas
- Stream
- Java.time

**Novedades de Java 11**
- Inferencia de tipos en datos primitivos.
- Metodo estatico of en colecciones.
---
## 🍃SPRING

**Spring**: Framework de java para delegar tarear repetitivas. Con el uso de anotaciones.
**Spring boot**: Proyecto basado en Spring para la creacion de aplicaciones autocontenidas. Contiene propio servidor de aplicaciones embebido e icluye gestor de dependencias como Gradle y Maven.
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

### Anotaciones

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

## 💬Kafka
✍

---

## 📌Adicionales

**Git**: Control de versiones

**5 principios S.O.L.I.D. de diseño de aplicaciones de software**
- **S** – Single Responsibility Principle (SRP): Una clase debería tener una, y solo una, razón para cambiar.
- **O** – Open/Closed Principle (OCP): Deberías ser capaz de extender el comportamiento de una clase, sin modificarla.
- **L** – Liskov Substitution Principle (LSP): Las clases derivadas deben poder sustituirse por sus clases base.
- **I** – Interface Segregation Principle (ISP): Haz interfaces que sean específicas para un tipo de cliente.
- **D** – Dependency Inversion Principle (DIP): Depende de abstracciones, no de clases concretas.
    
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

---
## 📐Patrones de diseño

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

### Patrones estructurales
> Estos patrones explican cómo ensamblar objetos y clases en estructuras más grandes, mientras se mantiene la flexibilidad y eficiencia de la estructura.
- Proxy
- Adapter
- Decorador

###Patrones de comportamiento
> Estos patrones tratan con algoritmos y la asignación de responsabilidades entre objetos.

- Command
- Strategy
- Observer

---
## 🤔Preguntas Frecuentes

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