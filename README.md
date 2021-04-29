![Banner](imagenes/banner.png)

# M0S0: Fundamentos de Programación y Algoritmia

En esta sesión, comenzaremos sobre los fundamentos en sobre desarrollo de Software, lenguajes de programación y algoritmia básica.

# ÍNDICE

- [Conceptos Generales del Desarrollo de Software](https://github.com/U-Camp/BOOT-M0/blob/main/README.md#conceptos-generales-del-desarrollo-de-software)
    - [Lenguajes de Programación](https://github.com/U-Camp/BOOT-M0/blob/main/README.md#lenguajes-de-programaci%C3%B3n)
    - [Paradigmas de Programación](https://github.com/U-Camp/BOOT-M0/blob/main/README.md#paradigmas-de-programaci%C3%B3n)
    - [Principios básicos de Programación Orientada a Objetos](https://github.com/U-Camp/BOOT-M0/blob/main/README.md#principios-b%C3%A1sicos-de-la-programaci%C3%B3n-orientada-a-objetos)
    - [Patrones de Diseño](https://github.com/U-Camp/BOOT-M0/blob/main/README.md#patrones-de-dise%C3%B1o)
    - [Full Stack Development](https://github.com/U-Camp/BOOT-M0/blob/main/README.md#full-stack-development)
- [Breve Historia de la World Wide Web](https://github.com/U-Camp/BOOT-M0/blob/main/README.md#breve-historia-de-la-world-wide-web)
- [Fundamentos de HTML](https://github.com/U-Camp/BOOT-M0/blob/main/README.md#fundamentos-de-html)

# Conceptos Generales del Desarrollo de Software

## Lenguajes de Programación

Un lenguaje de programación ("programming language") es un lenguaje formal con reglas sintácticas, semánticas y gramaticales bien definidas (por ejemplo, un `if` debe tener siempre una condición por cumplir), el cual está conformado por un conjunto de palabras clave e instrucciones (`if, for, const, let, while`) que, al escribirse de manera correcta (código), se traducen en órdenes que algún dispositivo electrónico puede entender y ejecutar.

Los lenguajes de programación proveen y habilitan una estructura y un medio entendible (ambiente de desarrollo) para que se le puedan dictar instrucciones a un dispositivo. 

Estas instrucciones, al traducirse a lenguaje máquina o código ejecutable se transforman en software (conjunto de programas), el cual le describe a un hardware determinado, como puede realizar una o varias tareas (procesos) a partir de una entrada determinada (argumento) para producir una salida.

Los lenguajes de programación son viejos, tan viejos como el siglo IX, época en la que un grupo de eruditos árabes conocidos como los "Banu Musa " escribieron un estudio donde "describían

Un instrumento que sonaba por sí solo", y en el cual explicaban la forma en la que se podría construir un autómata que tocara la flauta siguiendo un algoritmo.

En la actualidad, los lenguajes de programación son parte inherente de todas las computadoras o dispositivos electrónicos, así como de todo lo que vemos a través de cualquier pantalla. 

Para llegar al punto en el que ya vemos el resultado de la ejecución del software, es necesario seguir una serie de pasos que nos permitirán llegar a la resolución de un problema determinado por medio del dispositivo, a esta serie de pasos se le llama algoritmo.

La palabra algoritmo, aunque es un término matemático, es muy usado en el mundo de la tecnología y nos remite nuevamente a lo que son los lenguajes de programación, ya que al final un programa es un algoritmo; el término se acuñó en honor al matemático árabe Al Khwarizmi.

Un algoritmo, en cuanto a la programación y el desarrollo de software se refiere, puede expresarse en diferentes formas, de las cuales las 4 principales son:

**1. Lenguaje Natural**: Una descripción detallada y paso por paso en lenguaje escrito de cada problema a resolver y como se espera resolverlo (requerimiento dentro de un sistema: *User Story*).

```
Problema: Lámpara no encendida.

Solución: Hay que verificar que la lámpara está conectada a la luz, si no está conectada, procederemos a enchufarla; si sí está conectada verificamos que el foco no esté fundido, sí sí está fundido se procederá a comprar otro foco y sustituirlo por uno nuevo; si el foco no está fundido, quiere decir que la lámpara está dañada, por lo que hay que comprar una nueva para sustituir la dañada.
```

**2. Diagrama de Flujo**: Diagrama visualmente entendible de un flujo de datos en el cual se dibuja cada paso o proceso determinado dentro de un sistema el cual resuelve un problema determinado.

**3. Pseudocódigo**: Es una combinación del lenguaje natural con las convenciones y sintaxis de algún lenguaje de programación con el cual se describen estructuradamente los pasos a seguir para resolver algún problema determinado o se definen procesos dentro de un sistema.

**Ejemplo de Pseudocódigo**

```
función validar_lámpara {

    establecer lámpara_funciona a falso;

    Si la lámpara no está enchufada entonces

        Enchufar lámpara;

    Si lampara enchufada enciende entonces

        establecer lámpara_funciona a verdadero;
    
    Fin Si

    Si no

    Si el foco está fundido entonces

        Cambiar el foco;

        Si con foco sustituido la lámpara enciende entonces

        establecer lámpara_funciona a verdadero;

    Fin Si

    Si no

        Cambiar lámpara;

    Fin Si

    Regresar lámpara_funciona;

}

```
**4. Programa**: Como ya lo comentamos, un programa es una serie de sentencias y métodos que se escriben siguiendo la sintaxis, reglas y estructura de un lenguaje de programación, lo cual permite que un dispositivo electrónico realice procesos determinados en base a una entrada, produciendo una salida.

Si un algoritmo define como se solucionará un problema aún haría falta implementar esa solución, para eso los lenguajes de programación ofrecen sus palabras clave y sentencias, pero el código se tiene que acomodar de manera uniforme y estructurada, de tal manera que a la acción de escribir y estructurar el código de otra manera es lo que se llama paradigma de programación.

# Paradigmas de programación

Así como existen diferentes tipos de lenguajes de programación también hay distintos paradigmas de programación los cuales, como ya se mencionó, definen como se escribe y estructura el código; algunos paradigmas que se usarán durante el curso son los siguientes:

**Programación estructurada**: Está basado en el uso de rutinas que realizan una tarea, cada una de las cuales puede tener 3 estructuras de control de flujo:

- **Secuencial**: Ejecución de una sentencia tras otra:

```javascript
/* SECUENCIAL */

// Inicializamos la constante `a` con el valor numérico `1`

const a = 1;

// Inicializamos la constante `b` con el valor numérico `2`

const b = 2;

// Realiza acción de sumar, `suma` es igual al valor numérico `3`

const suma = a + b;

// Imprime el valor `3` de la constante `suma` en la consola.

console.log(suma);

// Ejecución de un conjunto de sentencias sólo si se cumple una condición específica.

/* CONDICIONAL */

const c = 1;

const d = 2;

const sumaCondicional = c + d;

// Imprime el valor `3` de la constante `sumaCiclica` en la consola // sólo si éste es mayor o igual a 3.

if (sumaCondicional >= 3) {

console.log(sumaCondicional);

}
```

- **Cíclica**: Ejecución iterativa de un mismo conjunto de sentencias hasta que una condición específica deje de cumplirse.

```javascript

/* CÍCLICA */

const e = 1;

const f = 2;

const sumaCiclica = e + f;

// Imprime el valor del contador `i` en cada ciclo `0 1 2 3` en la consola

// hasta que el contador `i` sea mayor al valor de `suma`.

// En cada vuelta del ciclo, el contador `i` se incrementa en `1`

for (let i = 0; i <= sumaCiclica; i += 1) {

console.log(i);

}
```

- **Programación Funcional**: Establece que el programa debe dividirse en pequeños métodos o funciones que realizan actividades de manera atómica y determinística, esto quiere decir que el método debe realizar una sola acción de manera correcta (atómico) y que para un mismo valor de entrada, debe regresar siempre un mismo valor de salida (determinístico) con lo se intenta asegurar que los datos no se alteren accidentalmente; los siguientes puntos son importantes y deben tomarse en cuenta cuando se programe funcionalmente:

    - **Inmutabilidad de los datos que procesa una función**: esto quiere decir que los datos no deben cambiar, preservando el valor inicial, pero procesando esos valores para generar nuevos datos.

    - **Que los métodos sean funciones puras**: esto quiere decir que sean deterministas (el resultado será siempre el mismo para un mismo valor de entrada) y que no tengan ningún efecto secundario sobre los datos ajenos a la función (que no modifiquen variables globales o locales).

    -- **Si es necesario, se usan funciones de orden superior**: esto es que una función reciba una o más funciones y a su vez devuelva otra función, este concepto es bastante útil para cuando se requiere reusar métodos o usar callbacks.

    - Finalmente, de la mano con el punto anterior, la , que indica que el resultado de un método sirve como entrada para otro, lo que permite encadenar funciones.

```javascript
// Esta función cumple con la inmutabilidad

// No cambia el valor del parámetro `a` que está recibiendo

// Genera un nuevo valor `b` basado en `a`

const funcionPuraEInmutable = (a) => {

let b = a;

b += 1;

return b;

};

// Así mismo es pura, siempre que reciba 2 como parámetro

console.log(funcionPuraEInmutable(2)); // Imprime `3` // El prototipo de un arreglo en javascript

// tiene métodos de que hacen uso de funciones de orden superior

// y de la composición, `map` es uno de ellos

const arreglo = [1, 2, 3];

// Usamos el `map` del arreglo para invocar la función pura e inmutable

// al hacer esto, por cada elemento del arreglo, se invoca la función

// y la función recibe el elemento como parámetro

const mapaArreglo = arreglo.map(funcionPuraEInmutable);

// Lo que genera un nuevo arreglo con los elementos incrementados en `1`

console.log(mapaArreglo); // Imprime `[2, 3, 4]`

// Si se quiere reusar la función pura e inmutable, podemos hacerlo encadenando

// lo que permite el re-uso del código y la fácil lectura de este

const nuevoArreglo = [4, 5, 6];

// El primer `map` regresa un arreglo, con lo que componiendo y encadenando

// ese primer resultado se pasa al segundo `map` como parámetro

const resultadoEncadenado = nuevoArreglo

.map(funcionPuraEInmutable)

.map(funcionPuraEInmutable);

// El resultado será otro arreglo con los elementos incrementados en 2

console.log(resultadoEncadenado); // Imprime `[6, 7, 8]
```

- **Programación Orientada a Objetos**: Se basa principalmente en la definición de clases, que son un conjunto de métodos y propiedades que realizan una acción específica estructuradamente, lo que quiere decir que se nutre de la programación estructurada y la funcional. Ejemplos de este tipo de paradigma se verán a continuación.

Es necesario profundizar en la programación orientada a objetos (POO), este paradigma está soportado en la mayoría de los lenguajes de programación y provee una estructura uniforme que permite la reutilización de código y reimplementación de este de manera fácil y sencilla.

Este concepto de programación es el más usado actualmente para desarrollar cualquier tipo de aplicación y como su nombre lo indica, hace uso de representaciones abstractas de objetos reales proyectados computacionalmente; esto quiere decir que los objetos que se escriben y definen con código se pueden comparar a los objetos reales, ya que comparten las siguientes características:

- **Identidad**: Un objeto es siempre diferente a cualquier otro, aunque sean del mismo tipo, un gato determinado es diferente a cualquier otro gato, aunque probablemente tengan el mismo color de pelo y la misma edad.

- **Estado**: Es el conjunto de propiedades que tiene un objeto, los que con sus valores individuales hacen ser al objeto lo que es, por ejemplo, el nombre del gato, su color, su edad, etc.

- **Comportamiento**: Son los métodos o acciones que puede realizar un objeto determinado y dependen del tipo, por ejemplo, el gato no habla, pero puede maullar, si en lugar de un gato el objeto fuera un ave quizá podría volar.

# Principios básicos de la Programación Orientada a Objetos

Estas características otorgan a los objetos de propiedades que guardan datos así como de métodos que realizan acciones y procesan esos datos, pero para poder hacer uso de las mismas, es necesario definir esas propiedades y comportamientos en un concepto llamado Clase20 , básicamente una clase es una plantilla de código que sirve para instanciar objetos, esto es crear objetos en memoria, la cual debe seguir los principios básicos de la programación orientada a objetos21 , los cuales son los siguientes:

- **Encapsulamiento**: Este principio indica que hay que mantener el estado de un objeto privado, esto quiere decir que sólo el objeto pueda modificar características internas, en el ejemplo del gato el usuario puede alimentar al gato, pero no puede decidir qué tan hambriento se siente; así mismo, en la POO un objeto no puede comunicarse o alcanzar métodos o propiedades privados de otro objeto.


- **Abstracción**: Al aplicar el encapsulamiento, sólo unos cuántos métodos quedan accesibles externamente, lo que genera una interfaz de comunicación, esto quiere decir que un objeto no tiene porqué saber cómo ésta construido otro objeto o cómo funciona por dentro, sólo tiene que saber cómo comunicarse con él; tal cual como se interactúa con los objetos reales, muchas veces no se sabe cómo están construidos o cómo funcionan, el objeto con el que se interactúa expone una interfaz con la que se pueden realizar acciones en él. Si un usuario acaricia un gato y el gato como reacción empieza a ronronear, el usuario no tiene porqué saber cómo es que el gato ronronea, sólo interactúa a través del pelo y la piel del gato.

- **Herencia**: Muchas veces los objetos son bastantes similares, pueden compartir una lógica común, pero no siempre exactamente lo mismo; la herencia permite el re-uso del código al crear una clase hija con base en una clase padre, heredando las propiedades y métodos de la clase padre, haciendo posible que se escriban en la hija nuevas propiedades y métodos específicos de la clase hija. Por ejemplo, el gato es un animal y comparte algunas propiedades y acciones de otros animales, como el alimentarse las cuales se heredan de su clase "animal", pero tiene otros atributos y comportamientos específicos de los gatos, como el maullar.

- **Poliformismo**: En el ejemplo anterior, la acción de maullar también podría tomarse como una herencia de la clase "felino", ya que la mayoría de los felinos realizan exclamaciones con la boca, pero los gatos específicamente maúllan, ese pequeño cambio en como un objeto realiza una acción determinada es el polimorfismo y normalmente se logra sobrescribiendo o sobrecargando (overriding) los métodos de la clase padre.

```javascript

// La clase define las propiedades y comportamiento del objeto

class Persona {

nombre = '';

correo = '';

// El constructor instancia la clase

// es lo que hace que el objeto que se está creando

// tenga una identidad y un estado

constructor(nombre, correo) {

// La palabra reservada `this` hace referencia al ámbito `scope` del objeto

// en este caso hace referencia a sus propiedades internas.

this.nombre = nombre;

this.correo = correo;

}

// Los métodos definen el comportamiento tendrá el objeto

hablar(mensaje) {

console.log(`Persona ${this.nombre} dice: ${mensaje}`);

} decirCorreo() {

this.hablar(`Mi correo es: ${this.correo}`);

}

}

// La clase `Instructor` hereda las propiedades y métodos la clase `Persona`

// También se puede decir que `Instructor` es un tipo de `Persona`

class Instructor extends Persona {

// Se pueden crear nuevas propiedades para esta clase hija

materia = null;

// Así como crear nuevos métodos para esta clase hija

asignarMateria(materia) {

this.materia = materia;

}

explicar(tema) {

// Validamos si tiene materia asignada

if (!this.materia) {

console.log(`${this.nombre} no tiene materia asignada.`);

} else {

console.log(`Hoy, en clase de ${this.materia}, veremos el tema: ${tema}`);

}

}

// O se pueden sobrescribir métodos

hablar(mensaje) {

console.log(`${this.nombre} dice: ${mensaje}`); }

}

// Creamos o instanciamos un nuevo objeto de tipo `Persona`

// Al instanciarlo se le asigna una identidad.

const fulano = new Persona('Fulano', 'fulanito@de.tal');

// Se pueden realizar acciones por medio de su interfaz (abstracción)

// Imprime `Mi correo es: fulanito@de.tal`

fulano.decirCorreo();

// Imprime `Persona Fulano dice: Hola, qué tal!`

fulano.hablar('Hola, que tal!');

// Así mismo se puede crear un nuevo objeto de tipo `Instructor`

// El cual recibe una nueva identidad.

const instructorZutano = new Instructor('Instructor Zutano', 'instructor.zutano@de.tal');

// Al ser el objeto de tipo `Instructor` se tiene acceso a los nuevos métodos definidos en su clase

// Ya que aún no asignamos una materia

// imprime: `Instructor Zutano no tiene materia asignada`

instructorZutano.explicar('Programación orientada a objetos');

// Los métodos de las clases son los únicos que modifican las propiedades internas

// Por lo que las propiedades están encapsuladas

instructorZutano.asignarMateria('Desarrollo de Software');

// Ya que el Instructor tiene materia asignada

// imprime: `Hoy, en la clase de Desarrollo de Software, veremos el tema Programación orientada a objetos` 22

instructorZutano.explicar('Programación orientada a objetos');

// Se puede acceder a los métodos de la clase padre `Persona`

// Imprime `Mi correo es: instructor.zutano@de.tal`

instructorZutano.decirCorreo();

// O se pueden usar los métodos sobrescritos de la clase hija (polimorfismo)

// Imprime: `Zutano Instructor dice: Hola desde Instructor`

instructorZutano.hablar('Hola desde Instructor');

```

La POO es muy útil porqué permite la estructura del código de una manera ordenada, siempre y cuando se apliquen estos principios y se tenga siempre en mente que cada objeto tiene que hacer una sola cosa concreta y hacerla bien, todo esto en conjunto permitirá que un software escrito en un código de cualquier tamaño sea mantenible y legible ya que se reutiliza el código al máximo y provee un estándar uniforme que cualquier programador puede leer.

Si ya se sabe cómo se implementará la solución usando estas estructuras de código, hay que establecer cómo se comunicarán los objetos entre sí, aplicando buenas prácticas de arquitectura de software23 , esto es, conocer distintos diseños de arquitectura y plantillas de soluciones ya establecidas, sabiendo reconocer en qué momento del ciclo de desarrollo aplicar uno, otro o un conjunto de varios. Para eso se aplican patrones de diseño los cuales establecen la manera en la que la información va a fluir dentro de un sistema, siendo ya plantillas de solución probadas y aceptadas.

# Patrones de Diseño

Un patrón de diseño se define como una solución reusable a un problema en común dentro de un contexto específico, esto quiere decir que no hay que reinventar la rueda, en la mayoría de los casos ya hay soluciones probadas a determinados problemas y una arquitectura preestablecida que la implementa, por lo que no es necesario reimplementar, sólo conocer esas soluciones a problemas comunes y saber dónde implementarlas.

Los patrones de diseño, como ya se dijo, son soluciones ya probadas a problemas que son comunes a una arquitectura, en el desarrollo de software se aplican para solucionar problemas en la estructura de los objetos, por ejemplo si se ocupa de la funcionalidad de un objeto particular y éste objeto se va a usar en diferentes partes de la aplicación, lo ideal sería no instanciar el objeto en todas y cada una de las partes en las que se va a usar ya que cada vez que se instancia un objeto este ocupa espacio en memoria, por lo que si se aplica un patrón Singleton25 , sólo se instancia un sólo objeto y este mismo objeto es accesible y reusable en todos los lugares en donde se necesite.

Además de singleton, hay varios patrones de diseño que se pueden aplicar a problemas comunes de la arquitectura de software y son los siguientes:

- **MVC. Model-View-Controller**: hace referencia a dividir las responsabilidades de cada objeto (Single Responsibility Principle ) en un modelo que se encargará de obtener los datos necesarios de la aplicación, un controlador que se encargará de procesarlos y una vista que se encargará de mostrar los resultados del proceso, por lo que la separación de concerns queda definida y hace más mantenible el código. 

Este no es realmente un patrón de diseño, ya que se le considera más como una estructura base de arquitectura de software, la cual es de las más usadas. 

La arquitectura Frontend <-> Backend <-> Base de Datos trata de replicar este formato a gran escala (siendo el frontend la vista, el backend el controlador y la base de datos el modelo), así mismo dentro de cada uno de ellos se aplica el mismo formato para organizar las clases y los archivos que las definen.

- **Lazy Loading**: No todos los recursos u objetos se ocupan al momento de cargar una aplicación, por ejemplo, una imagen que se encuentre hasta el pie de una página web no es necesaria para iniciar la aplicación en sí, por lo que se puede cargar de manera perezosa, esto quiere decir que primero se carga lo importante o se cargan los recursos de manera priorizada, de tal manera que la aplicación sea funcional y luego se pueden ir cargando más recursos no tan importantes diferidamente (deferred).

- **Prototype**: Al momento de instanciar un objeto, normalmente lo que se hace es usar la palabra reservada `new` para crear una nueva instancia de la clase, pero eso ocasiona que las propiedades de esa instancia en particular no pueda cambiar nunca, está atada a la estructura de la clase que se definió, el patrón Prototype hace más flexible la estructura de las clases, ya que establece que en lugar de instanciar por medio de `new` se instancie `clonando`, lo que la convierte en un prototipo al cual se le pueden agregar o eliminar propiedades o métodos en tiempo de ejecución el código lo vaya necesitando. Javascript es un lenguaje orientado a prototipos, esto quiere decir que cuando instanciamos un objeto en JS, realmente lo que se está haciendo es clonar la clase e instanciar ese clon, eso ya lo hace internamente Javascript al momento de usar la palabra reservada `new`.

- **Decorator**: Cuando los objetos que se crean son estrictamente estáticos, lo que quiere decir que éstos siempre mantendrán la funcionalidad definida en su clase y no permiten nuevas funcionalidades una vez ya creados, se usan decoradores para extender la funcionalidad de un objeto en tiempo de ejecución, por lo que este patrón otorga flexibilidad al objeto en sí, al permitir agregar propiedades o comportamientos nuevos conforme se vayan usando. Al sere Javascript un lenguaje orientado a prototipos, cuando a un objeto que se haya creado se le agregan o modifican propiedades o métodos que no tienen definidos en su clase base, se dice que se está decorando ese objeto.

- **Iterator**: Muchas estructuras de datos, como los arreglos, son iterativas, esto quiere decir que se puede recorrer cada elemento dentro de la estructura de manera cíclica, ya sea para buscar un elemento en particular o para modificar la misma estructura del elemento y generar nuevas estructuras a partir de ésta (inmutabilidad), un iterador hace precisamente esto, provee métodos que recorren una estructura de datos de tal manera que se puede acceder a sus elementos de una manera estándar. En Javascript el prototipo Array ya implementa el patrón y provee métodos como `map`, `filter` o `reduce`, los cuales se usarán durante el proceso de escritura de código de los proyectos y actividades.

- **Composite**: Cuando se requiere que un objeto tenga objetos hijos y éstos a su vez tengan otros objetos hijos, puede que el árbol de jerarquías sea muy grande y difícil de seguir en el código, por lo que el patrón Composite provee la funcionalidad de crear componentes a partir de varios objetos relacionados entre sí, de tal manera que queden agrupados en un componente padre, el cual se encargará de manejar y pasarle propiedades a todos los objetos hijos. React hace uso extensivo de este patrón, lo cual se verá durante el curso.

- **State**: Como ya se mencionó, un objeto tiene estado y comportamiento definidos, el patrón state permite que el comportamiento dependa del estado actual del objeto, esto quiere decir que con cada cambio que el estado tenga, se generen comportamientos distintos, por ejemplo cuando el usuario introduce datos a una caja de texto, su estado puede cambiar y se puede validar la entrada al momento de que el usuario escriba, cambiando su comportamiento para dibujar un borde rojo y un mensaje de error si la entrada del usuario no es correcta o dibujando un borde verde si pasa el proceso de validación.

- **Observer**: En ocasiones un objeto cambia su estado y probablemente muchos otros objetos dependen de ese estado en particular, por lo que es necesario que los objetos intercomunicados sepan en el momento en que uno de ellos cambió su estado, para que éstos se adapten al mismo y así mismo cambien su estado si es necesario, por lo que el patrón observer provee el mecanismo para estar observando cambios de estado sobre objetos en tiempo de ejecución y comunicar a objetos dependientes del cambio de estado en el momento en el que éste ocurra. Los exploradores web usan este patrón para manejar parte del sistema interno de eventos, así mismo internamente React hace uso del patrón state y el patrón observer para comunicar cambios del estado entre los componentes y realizar cambios en las propiedades y comportamiento de los hijos, ajustando el estado de cada componente de esa manera, a este proceso React le llama reconciliación.

- **Adapter**: Muchas veces una aplicación necesita consumir un servicio o una librería que tiene otra forma diferente de comunicarse, esto quiere decir que usa otro formato de comunicación (por ejemplo un servicio que responda en XML 37 y la aplicación sólo usa JSON38 ), como en la vida real que muchas veces necesitamos adaptadores para conectar ciertos electrónicos a la red eléctrica de nuestras casa, así mismo muchas veces ocupamos adaptadores que comunican dos aplicaciones que tienen distinto protocolo de transmitir información, por lo que el patrón adapter abstrae la forma en la que se comunican los dos componentes y es el encargado de adaptar los datos de tal manera que sean entendibles para ambos componentes (por ejemplo, convirtiendo los datos en XML a un formato JSON o al revés); éste tipo de patrón se aplica normalmente cuando se consumen APIs REST o servicios web de terceros.

- **Proxy**: Una de las formas de consumir una API REST o servicios web de terceros es realizando peticiones directamente a los endpoints 41 de cada una de ellas, esperando el resultado del proceso y pasando los datos del resultado a un adapter, hay recursos públicos que pueden consumirse directamente desde el frontend sin ningún problema, pero muchas veces el recurso está protegido contra accesos indebidos y no permite el consumo directo, sino que necesita una forma de saber que el frontend que lo consume está autorizado a hacer ésta petición, por lo que se usa un proxy para realizar este tipo de peticiones seguras, ya que normalmente requieren del uso de tokens 42 de autorización que no deben ser vistos o compartidos directamente en el frontend, por lo que se crea un objeto del lado del servidor con los permisos necesarios para consumir los recursos y a su vez escucha las peticiones realizadas desde el frontend, consume los recursos protegidos y devuelve los datos del resultado al frontend. La librería axios 43 que se usará durante el curso para consumir la API REST del backend puede implementar este patrón en las peticiones que se le indique.

- **Publisher-Subscriber**: El patrón publisher-subscriber es parecido al patrón observer45 , pero normalmente se implementa para suscribirse a un servicio de stream de datos, esto quiere decir un servicio web o API que siempre esté mandando información o que comunique cambios internos, se puede ver como un mecanismo de escucha que siempre está conectado al flujo de datos, por ejemplo las notificaciones en una app web (como gmail), son escuchadas por medio de un subscriber el cual está observando cambios en el flujo de datos (publisher) y pasa esos cambios a la aplicación para que maneje los datos que cambiaron de forma conveniente.

- **Front Controller**: Este patrón de diseño se usa principalmente en aplicaciones frontend o móviles, ya que es usado para centralizar y manejar cualquier tipo de petición a la API REST del backend o a servicios de terceros, esto quiere decir que un sólo objeto se tiene que encargar de manejar y abstraer ésta funcionalidad, construyendo los modelos de datos que la aplicación va a usar. Se usa en conjunto con el patrón proxy, observer y adapter; envolviéndolos en un objeto que aplique estos patrones. Para poder tener una buena organización del frontend, React requiere este tipo de patrón para poder componentizar correctamente y separar la lógica de obtención de datos (peticiones directas por medio del proxy o aplicando subscribers) de la lógica de procesamiento de estos (adapter) y la presentación del resultado (MVC).

- **Façade**: Los sistemas grandes están formados por módulos o subsistemas, façade provee el estándar en la que cada módulo se va a comunicar con cualquier otro módulo, abstrae la mayor parte de los métodos de un sistema y provee una interfaz de métodos públicos de ese módulo en particular (fachada del módulo) que cualquier otro módulo puede usar. En sistemas grandes y complejos, aplicar este patrón se hace necesario, ya que en equipos de desarrollo grandes donde cada equipo se encargue de desarrollar un módulo del sistema en particular, debe proveer una interfaz fachada, que dé acceso al mismo desde otros módulos, normalmente se aplica para sistemas muy grandes en el backend.

- **Dependency Injection**: Normalmente un objeto depende de otros objetos para realizar su labor, por ejemplo, un objeto que se comunica con un servicio, puede depender de un adapter al cual pasarle los datos una vez que éstos se obtienen, por lo que para que el objeto pueda hacer eso, es necesario que se inyecte una instancia de éste adapter de tal manera que cuando el objeto lo necesite, éste no tenga que preocuparse por instanciarlo, sino simplemente usarlo. El proceso de inyección lo realiza un proveedor de dependencias o provider, el cual es el encargado de instanciar los objetos necesarios e inyectarlos dentro del objeto que los necesita. El uso de éste patrón habilita que el objeto dependiente se ocupe de usar la interfaz de su dependencia no importando que tipo sea ésta, lo que facilita la implementación y las pruebas unitarias49 , ya que de esta manera podemos inyectar un objeto falso (mock50 ) que implemente una interfaz falsa del objeto dependiente, por ejemplo en un objeto que use axios, podemos inyectar un objeto simulado de axios para que las llamadas a los servicios no se hagan realmente y para probar sólo la funcionalidad en sí.

- **Abstract Factory**: Algunas aplicaciones necesitan dependencias de la plataforma donde se estén ejecutando, por ejemplo el acceso al sistema de archivos o a distintas bases de datos, pero normalmente éste tipo de accesos la plataforma no las encapsula y su manejo y acceso es diferente entre sí (por ejemplo el sistema de archivos de Linux es EXT3 y el de Windows es NTFS y los dos guardan archivos de manera distinta), lo que quiere decir que al estar desarrollando este tipo de aplicaciones que requieren esos accesos, se tienen que validar sobre que plataforma se está ejecutando la aplicación y ejecutar las instrucciones necesarias para realizar las acciones que requiera la aplicación específicas para esa plataforma por lo que el código puede finalizar teniendo muchas validaciones (ifs anidados) y siendo menos mantenible, Abstract Factory resuelve ese problema ya que al implementarlo provee una fábrica abstracta de objetos de la misma familia que realizan una acción determinada sobre una condición específica, por lo que al final la aplicación en sí no sabe qué clase concreta está usando, sino simplemente accede a la interfaz y se comunica a través de ella directamente, delegando a la fábrica la responsabilidad de proveer el objeto de acceso que mejor convenga para esa acción. La librería de manejo de archivos File de NodeJS 52 implementa este patrón al igual que cualquier ORM 53 de acceso a base de datos.

- **Object Pool**: Cuando el performance de una aplicación es muy bajo, el costo en memoria que requiere instanciar objetos es alto y se requiere acceder a esos objetos muy seguido, se puede introducir una pool de recursos en la cual todos los objetos vivirán durante su ciclo de vida, esa pool puede ser accedida desde varios puntos de la aplicación y acceder a los objetos ya creados sin necesidad de volver a instanciarlos, usando la misma instancia siempre, eso es una object pool y se puede ver como un conjunto de singletons para muchos objetos. Las conexiones de acceso a base de datos normalmente son un pool de objetos de conexión aplicando este patrón, por lo que se aplica entre Mongoose y MongoDB.

Se puede ver que todos estos puntos forman un proceso definido y relacionados entre sí: solucionar un problema por medio de un algoritmo (en un lenguaje de programación) estructurar como se implementará esa solución (paradigma de programación) y establecer cuál va a ser la arquitectura dentro del sistema reusando soluciones ya probadas (patrón de diseño) es un proceso interactivo e iterativo, esto quiere decir que se debe repetir tantas veces como sea necesario por cada problema que el sistema requiera solucionar, a éste proceso de repeticiones se le llama ciclo de vida de desarrollo de software57 , el cual se compone de los siguientes pasos:

1. **Análisis**: Establecer el problema a solucionar y a manera general el algoritmo que solucionará ese problema en particular.

2. **Diseño**: Plasmar de forma visual o escrita la solución, especificando patrones de diseño si se necesitan y que se usarán para llegar a la solución.

3. **Implementación**: Escribir el código en un lenguaje de programación, siguiendo los principios y estándares definidos en el diseño.

4. **Pruebas**: Realizar las pruebas necesarias que verifiquen que la solución fue implementada correctamente y que realmente resuelve el problema y no introduce nuevos.

4. **Despliegue**: Subir la solución implementada y sin errores a la plataforma donde se vaya a ejecutar.

Los pasos de éste proceso se pueden repetir tantas veces sea necesario dependiendo de la cantidad de problemas o requerimientos que un sistema de software en particular tenga que solucionar, hay distintos marcos de trabajo que implementan éste proceso, el más usado actualmente es SCRUM58 , en el cual todos los problemas que tiene que solucionar un sistema, se especifican desde el principio (backlog59 ) y se van armando grupos de tareas (epics60 ) las cuales se van solucionando poco a poco en cada iteración (sprint61 ), por lo que en cada iteración se va construyendo el sistema incrementalmente, desplegando las soluciones a éstos pequeños problemas de manera ágil y rápida, por lo que al ir armando el sistema de manera incremental, se va entregando valor de forma expedita.

Como se puede observar, todos estos conceptos son universales al desarrollo de software, por lo que se aplican y adaptan a cualquier lenguaje de programación y se usan para construir software de calidad, mantenible y ordenado. Durante el desarrollo del curso se irá ahondando más en estos conceptos teóricos a través de la práctica, para ello se usará el lenguaje de programación JavaScript62 , los paradigmas de programación antes descritos, aplicando los patrones de diseño que se requieran en cada actividad a realizar.

Puedes descargar la siguiente [INFOGRAFÍA 1 - CICLO DE VIDA](https://github.com/U-Camp/BOOT-M0/blob/main/infografias/Semana_0_Infograf%C3%ADa_1_C.pdf)

# Full Stack Development

El desarrollo de soluciones web tiene dos componentes principales: el frontend y el backend, cada uno de los cuales está a cargo de realizar distintos procesos en la información que fluye a través de ellos, el frontend  es el encargado de renderizar todos los datos y la información ya procesada por el sistema y permite capturar los datos que introduzca el usuario o le permite interactuar con la interfaz de usuario (UI) proveyendo una experiencia de usuario (UX) intuitiva y fácil de usar, todo esto por medio de un explorador web, pero debido a que el explorador web no tiene acceso al sistema de archivos del sistema operativo en el que se está ejecutando no puede acceder directamente a bases de datos, se hace necesario el uso de un backend, desde donde el sistema pueda generar nuevos archivos de información (por ejemplo un PDF o un Excel que el usuario quiera descargar) o comunicarse con una base de datos  para procesar la información que se genera.

Un programador que puede configurar y desarrollar sistemas interactivos tanto en front como en back, sabe integrar ambos elementos conociendo como se comunican entre sí por medio de una API REST, así como guardar y acceder a información correctamente estructurada en una base de datos, se le llama Desarrollador Full Stack.

La arquitectura de una aplicación web está dada principalmente por el modelo cliente-servidor69 , en el cual un cliente (explorador web por medio del frontend) realiza peticiones de recursos a un servidor (backend) por medio de una API (API REST que es un protocolo de comunicación que ambas partes entienden) la cual devuelve un resultado que es presentado al usuario final.

El término Full Stack es aplicado a un conjunto de tecnologías específica (stack). Durante este curso se aplicará el siguiente stack de tecnologías:

Ejecución del lado del cliente, normalmente un explorador web (chrome, firefox, edge, safari) el cual ya tiene implementado un motor de ejecución de código 70 (engine), el cual puede interpretar las siguientes tecnologías:

Es un esquema estático que define como se acomodan los elementos en una página web. Puede ser modificado usando javascript, volviendo cualquier aplicación web interactiva.

Las hojas de estilo en cascada (Cascading Style Sheets) son un esquema utilizado para describir la presentación de los elementos en una página web, si HTML define como se acomodarán estos elementos dentro de la aplicación, CSS define cuál será su estilo y presentación al usuario final. Como ya se mencionó, JS es un lenguaje de programación ligero, interpretado, basado en prototipos y orientado a objetos. Provee los métodos necesarios que hacen la web interactiva.

Ejecución del lado del servidor, en el que un proceso está escuchando peticiones en sus endpoints (recursos) definidos en la API (Application Programming Interface), que expone esos recursos a la web. Así mismo es el encargado principal del proceso de los datos y de generar la información principal de un sistema con base en las reglas de negocio del problema que se quiere solucionar. La implementación de los procesos decisivos y más importantes de un sistema se realiza en el backend. Por ejemplo, las transacciones seguras de un proceso de pago en un e-commerce75 , deben realizarse del lado del servidor, normalmente estos procesos manejan tokens de acceso y claves, que si se filtran al frontend pueden implicar un riesgo de seguridad. Las tecnologías de backend que se usan son las siguientes:

Es un motor de ejecución de código Javascript del lado del servidor, esto quiere decir que permite programar sistemas con el mismo tipo de código con el que se programa el frontend, disminuyendo la curva de aprendizaje y haciendo el desarrollo más ágil. NodeJS extiende la funcionalidad de Javascript proveyendo mecanismos de acceso que no se tienen en el frontend, como el acceso al sistema de archivos o a bases de datos.

Es un servidor web desarrollado en Javascript, que se integra como un módulo en NodeJS y que permite la definición de endpoints, rutas y middlewares 78 de tal manera que se pueda crear una API Rest rápidamente.

Es un ORM (Object-Relational Mapping) que permite el mapeo de modelos de un esquema de MongoDB. Por ejemplo, un modelo de una entidad usuario, que es una representación esquematizada de todos los datos almacenados en MongoDB de un documento de un usuario. Así mismo da acceso a la base de datos y maneja las conexiones a la misma.

Es la base de datos en sí, donde se almacena toda la información del sistema en forma de un esquema de documentos. 1969: El Departamento de Defensa de los Estados Unidos desarrolla una red que conectaba varias universidades californianas, llamada ARPANET.

# Breve Historia de la World Wide Web

**1969 - 1991:** ARPANET se fue extendiendo en los centros académicos y militares de todo el mundo adoptando TCP/IP 82 de paso. En un principio la comunicación entre ordenadores era muy básica, sólo se intercambiaban mensajes o se ofrecía un acceso directo a los archivos compartidos en la red.

**1989:** Tim Berners-Lee83 , junto con el equipo con el que trabajaba en el CERN, inventó y desarrolló el protocolo de comunicación HTTP84 , el sistema de direcciones por medio de URLs85  y el HTML, lo cual permitía crear páginas con texto e imágenes que se enlazaban entre sí.

**1991:** ARPANET se vuelve pública. Tim-Bernes Lee y su equipo crearon el primer navegador web llamado "WorldWideWeb86 " que sólo funcionaba en computadoras NeXT y renderizaba solamente texto. (Primera página web de la historia: https://www.w3.org/History/19921103hypertext/hypertext/WWW/TheProject.html).

**1993:** Se crea Mosaic88 , el primer explorador web gráfico multiplataforma (Disponible para Mac, Windows y otros) al ser multiplataforma fue muy popular en los círculos académicos. Fue desarrollado en el NCSA (National Center for Supercomputing Applications) por Marc Andreessen y Eric Bina.

**1993:** Se crea el primer buscador de la historia AliWeb89 , el cual era un índice o lista recopilada a mano de varios sitios web.

**1994:** Se lanza al público Netscape Navigator90 , el primer navegador web de uso comercial, también desarrollado por Marc Andreeseen. El acceso a internet en esos momentos era muy limitado, lento y caro.

**1994:** Se crea el W3C 91 (World Wide Web Consortium) el cual genera recomendaciones y estándares que fomentan el crecimiento de la web. Dirigido por Tim Berners-Lee hasta la actualidad.

**1995:** Microsoft lanza Internet Explorer92 , como parte de su sistema operativo Windows 95, lo que permitió que se convirtiera en el explorador dominante.

**1995:** Netscape desarrolla y lanza Javascript, que permitía acceder al HTML de una página web por medio del DOM 93 para volverla más dinámica.

**1996:** Se crea CSS, que permite estilizar una página web y cambiar su estilo visual y diseño.

**1997:** Nace Google.

**1998 - 2001:** Se adaptan los lenguajes de programación para ser usados del lado del servidor (Perl, Python y Ruby) o se crean nuevos lenguajes como PHP y haciendo uso de las tecnologías existentes (HTML, CSS, Flash y Javascript) la web se vuelve más interactiva y atractiva para los usuarios. El internet es más accesible y barato.

**2002 - Actualidad:** Se desarrolla de manera orgánica la Web 2.094 , la cual es una evolución de las primeras páginas web. Boom de las páginas web y la burbuja de las .com explota. Surge la web social, páginas como MySpace, Facebook, YouTube se vuelven imprescindibles. El internet es ampliamente usado y asequible para la mayoría.

**2005:** Google lanza el paper de su algoritmo MapReduce95 , el cual permitía desarrollar un ranking de las páginas buscadas de forma distribuida, permitiendo su implementación open source, la cual se usa para desarrollar redes distribuidas, base de la computación en la nube actual.

**2009:** Se publica MongoDB, un motor de base de datos NoSQL 96 que surge como alternativa a las bases de datos relacionales97 , con el cual se intenta flexibilizar el guardado y manejo de grandes cantidades de información.

**2010:** Nace NodeJS, motor de tiempo de ejecución de javascript del lado del servidor.

**2013:** Se desarrolla y publica la primera versión de ReactJS98 , librería de código abierto para crear interfaces de usuario en Javascript, creado por un equipo de desarrollo de Facebook.

**Actualidad - Futuro:** W3C genera estándares para la web semántica99 , lo que permite y permitirá que las máquinas se entiendan entre sí, de tal manera que los metadatos describan una aplicación web, por lo que un cliente automatizado podrá consumir otro cliente, entendiéndolo desde su contexto.

Puedes descargar la siguiente [Infografía WWW 1era parte](https://github.com/U-Camp/BOOT-M0/blob/main/infografias/Semana_0_Infograf%C3%ADa_2_C.pdf)

Puedes descargar la siguiente [Infografía WWW 2da parte¨](https://github.com/U-Camp/BOOT-M0/blob/main/infografias/Semana_0_Infograf%C3%ADa_3_C.pdf)
