# Clean Code

## SUMMARY - Camilo Gonzalez

# CÓDIGO LIMPIO

### **El coste total de un desastre**

- Si no se maneja un código limpio un proyecto que inicia de manera productiva puede acabar avanzando  a paso de tortuga con el tiempo
- “Dedicar tiempo a que el código sea correcto no solo es rentable, es una cuestión de supervivencia profesional”
- Esto es debido a que no somos profesionales. Muchos desarrolladores se dejan presionar con los plazos de entrega sin darse cuenta que creando mal código una tarea sencilla puede convertirse en un verdadero problema
- Para crear código limpio se necesita aplicar una serie de técnicas usando un sentido de corrección (Capacidad de identificar un incorrecto, pero también capacidad de saber como solucionarlo)
- Luego nos mencionan el que es el concepto de código limpio para algunos grandes programadores, como por el ejemplo el inventor de C++ (Bjarne Stroustrup), quien menciona el tema de la elegancia  y la eficacia (La lógica debe de ser directa para evitar errores ocultos) y habla de reducir las dependencias para facilitar el mantenimiento. También hablan del concepto de otros programadores, los cuales la mayoría coinciden en que el código debe de ser legible y directo, un ejemplo: Asignar nombres con sentido. Mencionan que se deben realizar pruebas de unidad para asegurarse de que la logica del programa funcione correctamente de manera automática. Nos dicen que el código debe ser escrito pensando en que será leído por otra pesona.
- Esto se podría resumir en lo que llaman las 4 reglas de código simple de beck: Ejecuta todas las pruebas, no contiene duplicados, expresa todos los conceptos dle diseño del sistema , minimiza el numero de entidades.

(QUE SON LOS OBJETIVOS S.M.A.R.T)

- Specific (específico)
- Mensurable (medible)
- Achievable (alcanzable)
- Relevant (relevante)
- Timely (temporal)

### **Escuelas de pensamiento**

- Se ve el libro como una escuela de pensamientos, es decir, los conceptos, tecnicas y consejos que mencionan los autores tienen respaldo de años de estudio, analisis y pruebas. Sin embargo es imposible que alguien tenga la verdad absoluta sobre como se crea un código limpio.

### **Somos autores**

- Para resolver un problema, añadir una nueva funcionalidad, etc, se necesita leer el código ya creado. La proporción entre leer y escribir código es 10 a 1, siendo leer la parte mas significativa, por eso cuando escribimos código siempre querremos que la lectura sea sencilla. Por eso si se quiere ser mas eficiente, mas que pensar en que el código sea facil de escribir, se debe pensar en que el código sea facil de leer.

### La regla del Boy Scout

- No basta con escribir código correctamente. “Dejar el campamento mas limpio de lo que se ha encontrado”. Siguiendo esta lógica, para que el código no se corrompa debemos tomar un papel activo y limpiarlo constantemente con pequeños cambios (Cambiar el nombre de una variable, dividir una función demasiado extensa, eliminar elementos duplicados, simplificar una instrucción if compuesta)

### Conclusión

- Este libro por si solo no puede prometernos que nos convertiremos en un buenos programadores. Solo puede mostrarnos los procesos de pensamiento de buenos programadores, ademas de trucos, tecnicas y herramientas que emplean grandes programadores.

# NOMBRES CON SENTIDO

REGLAS BÁSICAS PARA CREAR NOMBRES CON SENTIDO

### **Usar nombres que revelen las intenciones**

- Un nombre de lo que sea debe indicar por qué existe, que hace y cómo se usa
- Si un nombre requiere un comentario, significa que no revela su contenido

### **Evitar la desinformación**

- Ej: No poner nombre lista a algo que no sea una lista en programación
- No usar nombres con variaciones mínimas
- Evitar usar la l minuscula o la O mayúscula, porque pueden parecerse a constantes como 1 o 0, o incluso una i mayúscula

### **Realizar distinciones con sentido**

- Ej: No usar variables como a1, a2, etc porque a pesar de que no desinforman, estos nombres no ofrecen información
- Evitar las palabras redundantes, como usar “El”, “Un”. Tampoco se debe añadir por ejemplo la palabra variable a una variable, o la palabra table a una tabla.

### **Usar nombres que se puedan pronunciar**

- Facilita mucho la comunicación con el equipo y la lectura del código

### **Usar nombres que se puedan buscar**

- Facilita mucho la comunicación con el equipo y la lectura del código

### **Evitar codificaciones***

(Codificar datos es asignar números a las modalidades observadas o registradas de las variables que constituyen la base de datos, así como asignar código (valor numérico) a los valores faltantes (aquellos que no han sido registrados u observados).

- Los nombres codificados son impronunciables y normalmente se escriben de forma incorrecta

- **Notación húngara***
    - Hoy en día los entornos nos advierten de errores de tipado, por lo que usar la notación húngara solo haría mas complicado el mantenimiento y dificultan la legibilidad del código
- **Prefijos de miembros***
    - (Los miembros de una clase son un conjunto de elementos que definen a los objetos (atributos ó propiedades), así como los comportamientos o funciones (métodos) que maneja el objeto)
    - Los prefijos son un indicio de código antiguo porque los usuarios aprenden a ignorar el prefijo o sufijo y fijarse en la parte con sentido del nombre
- **Interfaces e implementaciones***
    - Pendiente: Repasar concepto de implementación, codificación, factoría.

### **Evitar asignaciones mentales**

- Evitar crear un tipo de “marcador de posición que el lector debe asignar mentalmente a un concepto real”
- Ej: No puede pretender que el programador que está leyendo su código recuerde que “r”  es la versión en minúscula de una URL sin el host y el sistema

### **Nombres de clases**

- El nombre de una clase no debe ser un verbo
- Ej: Se deben usar nombres como Customer, WikiPage, Account

### **Nombres de métodos**

- Deben tener nombres de verbo
- Ej: Se deben usar nombres como deletePage, save
- Los metodos de acceso deben usar el prefijo “get”, “set”, o “is”

### **No se exceda con el atractivo**

- Optar por la claridad antes que por el entretenimiento
- No recurrir a bormas culturales

### **Una palabra por concepto**

- Elegir una palabra por cada concepto abstracto y mantenerla
- Ej: “fetch”, “retrieve” y “get” no se deben usar como métodos equivalentes de clases distintas

### **No haga juegos de palabras**

- Ej: Se tienen muchas clases que tienen el método add, si se quiere crear una nueva clase con un método que haga algo parecido a “add”, no es correcto llamarlo de la misma manera, ya que se entraría en un juego de palabras, en su lugar se podría llamar “insert” o “append”

### **Usar nombres de dominios de soluciones***

- Para los nombres, intentar usar términos informáticos, algoritmos, nombres de patrones, términos matemáticos, etc
- Pendiente: Repasar concepto de dominios de soluciones, JobQueue, Patrones

### **Usar nombres de dominios de problemas***

- Cuando no exista un término de programación para lo que se está haciendo, usar el nombre del dominio de problemas

Pendiente: Repasar concepto de dominio de problemas

### **Añadir contexto con sentido**

- Incluir los nombres en un contexto, como clases, funciones, espacios con nombres adecuados
- Ej: Si se usan variables como nombre, apellido, calle, numeroDeCasa es evidente que se está hablando de una dirección, por lo que lo ideal sería crear la clase “Address” y poner las variables ahí

### **No añadir contextos innecesarios**

- Ej: No añadir sufijos o referencias que no sean relevantes

### **Conclusión**

- La habilidad de elegir un buen nombre es mas un problema de formación que un problema técnico, por lo que muchos desarrolladores no aprenden a hacerlo bien, sin embargo es una práctica impresindible a la hora de escribir código de calidad ya que mejora drásticamente la legibilidad del código

# FUNCIONES

¿Que hay que hacer para que una función transmita su intención?

¿Que atributos podemos asignar a nuestras funciones para que el lector pueda intuir el tipo de programa al que pertenecen?

### **Tamaño reducido**

- Las funciones deben tener un aproximado de 20 líneas
- **Bloques y sangrado**
    - Los bloques de código en instrucciones if, else, while, y similares deben tener una sola línea de longitud (Que seguramente sea la invocación a una función)
    - Las funciones no deben tener un tamaño excesivo que tenga instrucciones anidadas
    - El nivel de sangrado de una función no debe ser mayor de uno o dos
    
    ```csharp
    
    public static int calculate (operationRequired) {
    	if (operationRequired == "addition") {
    		addition()
    	}
    	else if (operationRequired == "rest"){
    		rest()
    	}
    	//Rest of operations...
    }
    
    public static int addition(num1. num2){
     return num1 + num2
    }
    
    ```
    

### **Hacer una cosa**

- “Las funciones solo deben hacer una cosa. Deben hacerlo bien y debe ser lo único que hagan”
- Necesitamos que todos los pasos que realice la función se encuentren en el mismo nivel de abstracción
- **Secciones en funciones**
    - Las funciones que hacen solamente una cosa no se pueden dividir en secciones, como declaraciones, inicializaciones y filtros

### **Un nivel de abstracción por función***

Pendiente: Repasar concepto de niveles de abstracción

- **Leer código de arriba a abajo: La regla descendente**
    - El código debe leerse como un texto de arriba a abajo, tras cada función debe aparecer la del siguiente nivel de abstracción

### Instrucciones switch*

- En las instrucciones switch usamos el polimorfismo para asegurarnos de incluirlas en un nivel inferior y de no repetirlas

Pendiente: Repasar y aplicar concepto de polimorfismo

### Usar nombres descriptivos

- Cuanto mas reducida y concreta sea una función, sera mas fácil elegir un nombre descriptivo
- “Un nombre descriptivo extenso es mucho mejor que uno breve pero enigmático”

### Argumentos de funciones

Monádico: Funciones con 1 argumento

Diádico: Funciones con 2 argumentos

Triádico: Funciones con 3 argumentos

Poliadico: Funciones con mas de 3 argumentos

- Se deben evitar mas de 2 argumentos en una función
- Esto facilita la lectura de la función y la creación de pruebas unitarias

- Formas monádicas habituales
    
    Dos motivos principales para pasar un solo argumento
    
    - Realizar una pregunta sobre el argumento
    - Procesar el argumento, lo transforme en otra cosa y lo devuelva
- Argumentos de indicador
    - Evitar pasar como argumento un valor booleano, ya que complica la firma del método e indica que la función hace mas de una cosa
- Funciones diádicas
    - Las funciones con dos argumentos son comunes, sin embargo si puede convertirla en una con un único argumento, hágalo, las funciones monódicas son mas simples de leer
- Triadas
    - Se debe pensar dos veces antes de crear una función triádica. Son aún mas difíciles de entender
- Objeto de argumento
    - Cuando una función parece necesitar dos o mas argumentos, se puede hacer una reducción del número de argumentos mediante la creación de objetos
- Listas de argumentos
    - Si los argumentos variables de una función se procesan de la misma forma, pueden ser equivalentes a un único argumento de tipo List
- Verbos y palabras clave
    - El nombre de una función en formato monádico con su argumento deben formar un par de verbo y sustantivo: `writeField(name)`

### Sin efectos secundarios

- Debemos evitar que nuestras funciones hagan otras cosas ocultas, ya que esto puede generar cambios inesperados en el programa
- Argumentos de salida
    - Los argumentos de salida deben evitarse. Si la función necesita cambiar el estado de un elemento, se debe hacer que cambie el estado de su objeto contenedor

### Separación de consultas de comando*

Pendiente: Repasar ¿Que es separar la consulta del comando?

(Command–query separation (CQS) es un principio de la programación orientada a objetos. El principio afirma que cada método debe ser un comando que realiza una acción, o una consulta que devuelve datos al llamante, pero no ambos. En otras palabras, hacer una pregunta no debe cambiar la respuesta.)

### Mejor excepciones que devolver códigos de error*

- Devolver códigos de error de funciones de comando es un sutil incumplimiento de la separación de comandos de consulta, ya que hace que se generen estructuras anidadas

- Extraer bloques try/catch*
    
    Pendiente: Repasar concepto de try/catch
    
    - Los bloques try/catch confunden la estructura del código y mezclan el procesamiento de errores con el normal
    - Se debe extraer el cuerpo de los bloques try y catch en funciones individuales
    
    (El propósito de un bloque try-catch es detectar y controlar una excepción generada por código en funcionamiento. Algunas excepciones se pueden controlar en un bloque catch y es posible resolver el problema sin que se vuelva a producir la excepción, pero la mayoría de las veces lo único que se puede hacer es asegurarse de que se produzca la excepción adecuada.)
    
- El procesamiento de errores es una cosa
    - Una función que procese errores no debe hacer nada más
- El imán de dependencias Error.java*
    - Pendiente: Repasar concepto de excepciones

### No repetirse

- La duplicación es un problema porque aumenta el tamaño del código y requerirá mas tiempo si alguna vez se desea cambiar el algoritmo. También hace que se eleve el riesgo de errores
- Existen muchos principios y prácticas que nos ayudan a controlar o eliminar la duplicación

### Programación estructurada

- Todas las funciones deben tener una entrada y una salida
- Solo debe haber una instrucción `return`
- Un bucle no debe tener instrucciones `break` o `continue`
- Un bucle nunca debe tener instrucciones `goto` El propósito de la instrucción es transferir el control a un punto determinado del código, donde debe continuar la ejecución.

(Esto muchas veces no aplica a funciones de tamaño reducido)

(`goto` solo tiene sentido en las funciones de gran tamaño, aún así debe evitarse)

### Como crear este tipo de funciones

- Primero se estructuran las ideas y después el mensaje hasta que se lea bien
- El primer borrador puede estar desorganizado, es necesario retocarlo hasta que se lea de forma adecuada

### Conclusión

- Las funciones son los verbos del lenguaje y las clases los sutantivos
- Los programadores experimentados piensan en los sistemas como en historias que contar, no como en programas que escribir
- Siguiendo las reglas que se mencionan en este capítulo, estaremos en capacidad de crear funciones breves, con nombres correctos y bien organizadas

# COMENTARIOS

“No comente el código incorrecto, reescríbalo”

La verdad solo se encuentra en el código, es la única fuente de información precisa, por eso, aunque en ocasiones sean necesarios, hay que empeñarnos en minimizarlos lo mas posible

### Los comentarios no compensan el código incorrecto

En lugar de perder el tiempo escribiendo comentarios que expliquen un código mal escrito, dediquese a solucionarlo

- Explicarse en el código
    
    En muchos casos basta con crear una función que diga lo mismo que el comentario que se pensaba escribir
    
    ```csharp
    //Comprobar que el empleado tiene derecho a todos los beneficios
    if (horasDelEmpleado>1000 && edad empleado > 18)
    ```
    
    ```csharp
    if (Empleado.comprobarBeneficios())
    ```
    

### Comentarios de calidad

- Comentarios legales
    
    Ej: Comentarios de derechos de autor, son necesarios y deben incluirse al inicio de cada archivo
    
    ```csharp
    // Copyright (C) .....
    // Publicado bajo las condiciones de ............
    ```
    
    Siempre que se pueda haga referencia a una licencia estándar en otro documento en lugar de incluir todos los términos y condiciones en el comentario
    
- Comentarios informativos
    
    Muchas veces es posible usar por ejemplo el nombre de una función para transmitir la información necesaria, sin embargo puede hacerse uso de un comentario si es algo bastante específico, como el formato de retorno de una fecha
    
- Explicar la intención
    
    En ocasiones, un comentario puede ser mas que sólo información útil sobre una implementación, también puede proporcionar la intención de una desición del autor
    
- Clarificación
    - Conviene buscar que un valor devuelto sea claro por si mismo, sin embrago cuando hablamos de una biblioteca estándar o de código que no se pueda alterar, puede ser útil usar un comentario aclarativo
    - Sin embargo existe un riesgo, por eso, antes de usar comentarios alcarativos debe asegurarse de que no hay una mejor solución, y de no haberla, también debe asegurarse de que los comentarios sean precisos
- Advertir las consecuencias
    
    ```csharp
    // No ejecutar a menos que le sobre tiempo
    [Test]
    public void _pruebaDemoradaDeCorrer
    {
    }
    ```
    
- Comentarios TODO
    - TODO, FIXME, DEPRECATED → Codetags
    - Solicitud para buscar un nombre mas adecuado
    - Para realizar un cambio que dependa de un evento planeado
    
    ```csharp
    // TODO - ......
    public void funcionIneficiente
    {
    }
    ```
    
    ```csharp
    // FIXME - ....
    public void funcionQueElCodigoFallaYNoSabemosPorQue
    {
    }
    ```
    
    Sin embrago, no es una excusa para mantener código incorrecto en el sistema, examínelos y elimine todos los que pueda
    
- Amplificación
    
    Se puede usar un comentario para amplificar la importancia de algo que, en caso contrario parecería irrelevante
    
    ```csharp
    string[] listOfAnything = something.Trim();
    //El recorte es importante, ya que...
    ```
    
- Javadoc en API públicas*
    
    Pendiente: Repasar concepto de Javadoc
    
    [Qué es JavaDoc y cómo utilizarlo para generar documentación - Otro](https://spa.myservername.com/what-is-javadoc-how-use-it-generate-documentation)
    

### Comentarios incorrectos

- Balbucear
    
    Cualquier comentario que obligue a buscar su significado en otra parte del código o en otro módulo ha fallado en su intento de comunicación. Se debe ser claro con los comentarios y asegurarse de que están bien redactados
    
- Comentarios redundantes
    
    Cuando el comentario no es más informativo que el código, sobra
    
    ```csharp
    public bool comprobarSiEsMayorDeEdad(int edad)
    {
    	if (edad >= 18)
    	{
    		return true;
    	}
    	else
    	{
    		return false;
    	}
    }
    
    // La función recibe un argumento edad y comprueba si la edad del usuario es mayor o menor que 18
    comprobarSiEsMayorDeEdad(19);
    ```
    
- Comentarios confusos
    
    Se debe evitar que las afirmaciones de los comentarios sean poco precisas
    
- Comentarios obligatorios
    
    Es un error afirmar que todas las funciones deben tener un javadoc, o que todas las variables deben tener un comentario. Este tipo de comentarios ensucian el código y generan confusión y desorganización
    
- Comentarios periódicos
    
    ```csharp
    /* Cambios (11-Oct-2001)
    * -----------------------------
    * 11-Oct-2001 : Reorganización de la clase y cambio a un nuevo paquete com.jrefinery.date (DG);
    * 05-Nov-2001 : Se añade un método getDescription() y se elimina la clase NotableDate (DG);
    * 12-Nov-2001 : .........
    ```
    
    Hoy en día bloques de comentarios  de registros de todos los cambios realizados son inútiles
    
- Comentarios sobrantes
    
    Comentarios que no ofrecen información nueva, sobran. Es probable que comentarios tan inservibles como el siguiente, empiezan a mentir cuando cambia el código que los rodea
    
    ```csharp
    /* Día del més */
    private int dayOfMonth;
    ```
    
- Comentarios sobrantes espeluznantes
    
    ```csharp
    // El nombre 
    private string name;
    
    // La versión
    private string version;
    
    // El licenceName
    private string licenceName;
    ```
    
- No usar comentarios si se puede usar una función o una variable
    
    ```csharp
    // Este bloque de código se ejecuta cuando la serpiente esté llendo hacia la derecha
    if (map[row+1,column] == backgroundMap &&  map[row-1,column] != snakeBody && map[row,column+1] != snakeBody)
    {
        map[row+1,column] = snakeHead;
        map[row,column] = snakeBody;
        map[row,column-snakeBodyHorizontalCounter] = backgroundMap;
    
        this.snakeBodyVerticalCounter+=1;
        this.snakeBodyHorizontalCounter-=1;
        return;
    }
    ```
    
    ```csharp
    bool snake_is_going_to_the_right   = map[row+1,column] == backgroundMap &&  map[row-1,column] != snakeBody && map[row,column+1] != snakeBody;
    
    if (snake_is_going_to_the_right)
    {
        map[row+1,column] = snakeHead;
        map[row,column] = snakeBody;
        map[row,column-snakeBodyHorizontalCounter] = backgroundMap;
    
        this.snakeBodyVerticalCounter+=1;
        this.snakeBodyHorizontalCounter-=1;
        return;
    }
    ```
    
- Marcadores de posición
    
    Este tipo de estructuras son atractivas sin los usa demasiado y cuando el beneficio sea significativo, de lo contrario, acabarán por ser ignoradas
    
    ```csharp
    // Acciones ///////////////////////////////
    ```
    
- Comentarios de llave de cierre
    
    Si se tiene la nececidad de marcar las llaves de cierre, pruebe a reducir el tamaño de las funciones
    
    ```csharp
    
    public static void anyFunction()
    {
    	if(something == true)
    	{
    		while(somethingElse == true)
    		{
    			doSomething()
    		} // While
    	} // if
    } // main
    
    ```
    
- Asignaciones y menciones
    
    Los sistemas de control de código fuente recuerdan a la perfección quién ha añadido qué y cuando.
    
    ```csharp
    // Añadido por ....
    ```
    
- Código comentado
    
    No se debe tener código comentado en nuestro código, los lectores que lo vean no tendrán el valor de borrarlo
    
- Comentarios HTML
    
    Se debe evitar tener HTML en comentarios de código, ya que dificulta la lectura. Si los comentarios se van a extraer a una página web. debe ser responsabilidad de dicha herramienta. 
    
- Información no local
    
    Si se tiene que escribir un comentario, se debe asegurar de que describa el código que lo rodea. No se debe ofrecer información global en el contexto de un comentario local
    
- Demasiada informacíon
    
    “No incluya en su código interesantes reflexiones históricas ni irrelevantes descripciones de detalles”
    
- Conexiones no evidentes
    
    La conexión entre un comentario y el código que describe debe ser evidente
    
    “Es una lástima que un comentario requiera su propia explicación”
    
- Encabezados de función
    
    ```csharp
    // Esta función recibe dos numeros y los suma
    public void operar (a, b)
    {
    	return a + b
    }
    ```
    
    ```csharp
    public void sumar (num1, num2)
    {
    	return num1 + num2
    }
    ```
    
- Javadocs en código no público
    
    > La generación de páginas javadoc para clases y funciones de un sistema no suele ser útil y la formalidad adicional de los comentarios javadocs no es más que una distracción”
    > 

### Conclusión

Debemos evitar lo máximo que podamos los comentarios, orientando al código a que sea legible por sí mismo, en caso de que sean completamente necesarios, debemos tener en cuenta los consejos dados en “Comentarios de calidad” para hacer que nuestros comentarios aporten valor, además de tener en cuenta los consejos de “Comentarios incorrectos” para evitar que dichos comentarios entorpezcan la legibilidad de nuestro código

# FORMATO

“Debe preocuparse por el formato de su código. Debe elegir una serie de reglas que controlen el formato del código y después debe aplicarlas de forma coherente”

### La función del formato

El formato del código es la principal preocupación de un desarrollador profesional

### Formato vertical

Los archivos de menor tamaño se entienden mejor que los grandes

- La metáfora del periódico
    
    Un archivo de código debe ser como un artículo de periódico
    
    - Nombre sencillo pero claro
    - Los elementos superiores del archivo deben proporcionar conceptos y algoritmos de nivel superior
    - Los detalles deben aumentar según avanzamos
    
    Un periodico (Programa) se compone de varios artículos (Módulos)
    
- Apertura vertical entre conceptos
    - El código se lee de izquierda a derecha y de arriba a abajo
    
    Cada línea         → Expresión o Clausula
    
    Grupo de lineas → Pensamiento 
    
    ```csharp
    using System;
    using System.Collections.Generic;
    using System.Linq;
    using System.Threading.Tasks;
    
    namespace DistanciaVertical;
    
    public class Person
    {
        public string name;
    		public string lastname;
    		public int age;
    
    		public Person(string name, string lastname, int age)
    		{
    				this.name = name;
    				this.lastname = lastname;
    				this.age = age;
    		}
    		
    		public string obtainCompleteName ()
    		{
    				return $"{name} {lastname}";
    		}
    }
    ```
    
    ```csharp
    using System;
    using System.Collections.Generic;
    using System.Linq;
    using System.Threading.Tasks;
    namespace DistanciaVertical;
    public class Person{
        public string name;
    		public string lastname;
    		public int age;
    		public Person(string name, string lastname, int age){
    				this.name = name;
    				this.lastname = lastname;
    				this.age = age;}
    		public string obtainCompleteName (){
    				return $"{name} {lastname}";}}
    
    ```
    
- Densidad vertical
    
    Las líneas de código con una relación directa deben aparecer verticalmente densas
    
- Distancia vertical
    
    Los conceptos relacionados deben pertenecer al mismo archivo, debe evitar que el lector deambule entre archivos y clases
    
    - Declaraciones de variables
        - Las variables locales deben aparecer en la parte superior de cada función
        - Una variable podría declararse en la parte superior de un bloque o antes de un bucle en una función extensa
        
        ```csharp
        public int promedioResultadosTest(int[] resultadosTest) {
        		int sumaResultados = 0;
        		int cantidadDeEstudiantes = resultadosTest.Count();
        		int promedio;
        
        		for (int resultado = 0; resultado < cantidadDeEstudiantes; resultado++)
        		{
        		sumaResultados+=resultadosTest[resultado];
        		}
        	
        		promedio = sumaResultados/cantidadDeEstudiantes;
        		return promedio;
        }
        ```
        
    - Variables de instancia
        
        Las variables de instancia deben declararse en la parte superior de la clase
        
    - Funciones dependientes
        
        Si una función invoca a otra, deben estar verticalmente próximas, y la función de invocación debe estar por encima de la invocada siempre que sea posible
        
        ```csharp
        class calculadora 
        {
        		public void Operar (string operacionARealizar, int num1, int num2)
        		{
        				switch (operacionARealizar)
        				{
        					case "suma":
        						sumar(num1, num2);
        						break;
        		
        					case "resta":
        						restar(num1, num2);
        						break;
        		
        					default:
        						break;
        				}
        		}
        	
        		private int sumar(int num1, int num2)
        		{
        				return num1 + num2;
        		}
        	
        		private int restar(int num1, int num2)
        		{
        				return num1 - num2;
        		}
        }
        ```
        
    - Afinidad conceptual
        
        Cuanto mayor sea la afinidad entre conceptos de código, menor distancia vertical debe existir entre ellos
        
        - Dependencia directa como cuando una función invoca a otra, o cuando usa una variable
        - Cuando un grupo de funciones realice una operación similar
- Orden vertical
    
    Una función invocada debe situarse por debajo de la que realice la invocación
    
    ```csharp
    sumar(2,2);
    
    public int sumar(num1, num2)
    {
    	return num1 + num2;
    }
    ```
    

### Formato horizontal

(El límite de carácteres por línea personal del autor es de 120)

- Apertura y densidad horizontal
    - Rodear los operadores con espacios en blanco para destacarlos (Las instrucciones de asignación tienen dos elementos principales: El lado izquierdo y derecho. Los espacios acentúan esta separación)
    - No incluir espacios entre los nombres de las funciones y el paréntesis de apertura (La función y sus argumentos están estrechamente relacionados
    - Separar los argumentos con espacios en blanco (Asentuar la coma)
    
    ```csharp
    public float calculateRectangleArea(float length, float widht)
    {
    		rectangleArea = length * widht;
    
    		return rectangleArea
    }
    ```
    
- Alineación horizontal
    
    Se deben evitar estructuras como la siguiente:
    
    ```csharp
    
    public class SnakeGame
    {
    			private int    snakeBodyHorizontalCounter = 1;
    			private int    snakeBodyVerticalCounter   = 0;
    			public  int    score                      = 0;
    			private string snakeHead                  = "@";
    			private string snakeBody                  = "0";
    			private string backgroundMap              = ".";
    			private string fruit                      = "#";
    			private string horizontalBorder           = "_";
    			private string verticalBorder             = "|";
    }
    
    ```
    
- Sangrado
    - Las instrucciones al nivel del archivo, como las declaraciones de clases no se sangran
    - Romper el sangrado
        
        
        ```csharp
        class calculadora {
        		public void Operar (string operacionARealizar, int num1, int num2){
        				switch (operacionARealizar){
        					case "suma":
        						sumar(num1, num2);
        						break;
        		
        					case "resta":
        						restar(num1, num2);
        						break;
        		
        					default:
        						break;
        				}
        		}
        	
        		private int sumar(int num1, int num2){
        				return num1 + num2;
        		}
        	
        		private int restar(int num1, int num2){
        				return num1 - num2;
        		}
        }
        ```
        
        ```csharp
        class calculadora 
        {
        		public void Operar (string operacionARealizar, int num1, int num2)
        		{
        				switch (operacionARealizar)
        				{
        					case "suma":
        						sumar(num1, num2);
        						break;
        		
        					case "resta":
        						restar(num1, num2);
        						break;
        		
        					default:
        						break;
        				}
        		}
        	
        		private int sumar(int num1, int num2){return num1 + num2;}
        	
        		private int restar(int num1, int num2){return num1 - num2;}
        }
        ```
        
- Ambitos ficticios
    
    Es preferible evitar instrucciones wuile o for que no contengan cuerpo. En caso de no poder evitarlas, es necesario sangrar el cuerpo ficticio
    
    ```csharp
    while (something == true && somethingElse == false)
    		;
    ```
    
- Reglas de equipo
    
    Un equipo de programadores debe acordar un único estilo de formato y todos los integrantes del equipo deben aplicarlo
    
    - Donde añadir las llaves
    - Que tamaño de sangrado utilizar
    - Los nombres de las clases, variables, métodos, etc

# OBJETOS Y ESTRUCTURAS DE DATOS

“Hay una razón para que las variables sean privadas, no queremos que nadie más dependa de ellas”

### Abstracción de datos

```csharp
public class Point 
{
		public int x;
		public int y;
}

```

```csharp
public interface IPoint
{
		int getX();
		int getY();
		
		void setCartesian(int x, int y)
}
```

Los métodos refuerzan una política de acceso. Se fuerza a establecer x-y de forma conjunta como una coordenada

---

“Para ocultar la implementación no basta con añadir una capa de funciones entre las variables. Se basa en la abstracción. Una clase no fuerza sus variables a través de métodos de establecimiento y recuperación, por el contrario, muestra interfaces abstractas que permiten a sus usuarios manipular la escencia de los datos sin necesidad de conocer su implementación”

```csharp
public interface IVehicle
{
	double getFuelTankCapacityInGallons();
	double getGallonsOfGasoline();
}
```

```csharp
public interface IVehicle
{
	double getPercentFuelRemaining();
}

```

Esta opción es preferible, ya que no queremos mostrar los detalles de los datos, sino expresarlos en términos abstractos

### Antisimetría de datos y objetos

> Diferencia entre objetos y estructuras de datos: Los objetos ocultan sus datos tras abstracciones y muestran funciones que operan en dichos datos. Las estructuras de datos muestran sus datos y carece de funciones con significado
> 

```csharp
// Código por procedimientos (El que usa estructuras de datos)

public class Square
{
	public double side;
}

public class Rectangle
{
	public double height;
	public double width;
}

public class Circle
{
	public double radious;
}

public class Geometry
{
	Square square;
	Rectangle rectangle;
	Circle circle;

	public Geometry(Square square, Rectangle rectangle, Circle circle)
	{
		this.square = square;
		this.rectangle = rectangle;
		this.circle = circle;
	}
	public const double PI = 3.1416;

	public double area(Object shape)
	{
		if (shape.GetType() == square.GetType())
		{
			return square.side * square.side;
		}
		else if (shape.GetType() == rectangle.GetType())
		{
			return rectangle.height * rectangle.width;
		}
		else if (shape.GetType() == circle.GetType())
		{
			return PI * circle.radious * circle.radious;
		}
		return 0;
	}
}

```

- Facilita la inclusión de nuevas funciones sin modificar las estructuras de datos existentes
- Dificulta la inclusión de nuevas estructuras de datos ya que es necesario cambiar todas las funciones

```csharp
// Código orientado a objetos

public interface IShape
{
	double area();
}

public class Square : IShape
{
	private double side;

	public double area()
	{
		return side * side;
	}
}

public class Rectangle : IShape
{
	private double height;
	private double width;

	public double area()
	{
		return height * width;
	}
}

public class Circle : IShape
{
	private double radious;
	private const double PI = 3.1416;

	public double area()
	{
		return PI * radious * radious;
	}
}
// El método area() es polimórfico
// No se necesita una clase Geometry
```

- Facilita la inclusión de nuevas clases sin cambiar las funciones existentes
- Dificulta la inclusión de nuevas funciones ya que es necesario cambiar todas las clases

### La ley de Demeter

Afirma que un módulo no debe conocer los entresijos (Aspecto o característica poco conocidos u ocultos de una persona o cosa)  de los objetos que manipula.

Un metodo f de una clase C solo debe invocar métodos de:

- C
- Un objeto creado por f
- Un objeto pasado como argumento a f
- Un objeto de una variable de instancia de C

- Choque de trenes
    
    ```csharp
    // " Camilo_Gonzalez "
    const string NombreConFormato = Person.nombre.trim().replace("_", " ").ToLower();
    ```
    
    Este tipo de cadenas de invocaciones debenm evitarse y se recomienda dividirlas de las siguiente forma:
    
    ```csharp
    string NombreSinEspacios = Person.nombre.trim();
    string NombreSeparado = NombreSinEspacios.replace();
    const string NombreConFormato = NombreSeparado.ToLower();
    ```
    

- Híbridos
    
    Se generan cuando se crea una estructura mitad objeto y mitad estructura de datos, estos híbridos dificultan la inclusión de nuevas funciones y también de nuevas estructuras de datos
    
- Ocultar la estructura
    
    Si Person es un objeto deberíamos indicarle que hiciera algo, no preguntar sobre sus detalles internos
    
    ```csharp
    const string Nombre = Person.añadirFormatoAlNombre();
    ```
    
    Así permitimos a Person ocultar sus detalles internos e impedimos que la función actual incumpla la ley de Demeter y se desplace por objetos que no debería conocer
    

### Objetos de transeferencia de datos

Un objeto de transferencia de datos (DTO) es una estructura de datos con variables públicas y sin funciones. Los DTO son muy útiles para comunicarse con bases de datos o analizar mensajes de conexiones, etc

- Registro activo
    
    Son estructuras de datos pero suelen tener métodos de navegación como `save` y `find`, por lo general, estos registros activos son traducciones directas de tablas de base de datos.
    

### Conclusión

- Los objetos muestran comportamiento y ocultan datos
- Las estructuras de datos muestran datos y carecen de comportamiento significativo

- En ocasiones necesitaremos la flexibilidad de:
    - Añadir nuevos tipos de datos (Por lo que preferimos objetos para esa parte del sistema)
    - Añadir nuevos comportamientos (Por lo que preferimos estructuras de datos y procedimientos)
- Los buenos programadores entienden estos problemas sin prejuicios y eligen el enfoque mas adecuado para cada tarea concreta

# PROCESAR ERRORES

“El control de errores es importante, pero si oscurece la lógica, es incorrecto”

Diver**sas técnicas y consideraciones que puede usar para crear código limpio y robusto, código que procese los errores con elegancia y estilo:**

### **Usar excepciones en lugar de códigos devueltos**

```csharp
public void GuardarEdad()
{
	int edad;
	Console.WriteLine("Ingrese su edad:");
	edad = Convert.ToInt32(Console.ReadLine());

    if (edad.GetType() != edad.GetType())
    {
        Console.WriteLine($"{edad} no es una edad válida");
    }
}
```

- Confunde al invocador, y éste debe comprobar inmediatamente los errores después de la invocación

```csharp
void GuardarEdad()
{
		int edad;
    Console.WriteLine("Ingrese su edad:");
    try
    {
			  edad = Convert.ToInt32(Console.ReadLine());
    }
    catch (FormatException ex)
    {
        Console.WriteLine($"No has introducido un valor numérico válido");
				edad = 0;
    }
}
```

- Genera una excepción al detectar un error
- El código de invocación es más limpio
- Su lógica no se oscurece por el control de errores

### **Crear primero la instrucción try-catch-finally**

- Catch debe salir del programa en un estado coherente, independientemente de lo que suceda en try
- Por este motivo, se recomienda iniciar con una instrucción try-catch-finally el código que genere excepciones. Asi se define lo que debe esperar el usuario del código, independientemente de que se produzca un error en try

### **Usar excepciones sin comprobar**

[Excepciones en Java](https://juanjosecanbus.wordpress.com/2014/10/20/excepciones-en-java/)

[[S.O.L.I.D.] Open-Closed Principle / Principio Abierto-Cerrado - Adictos al trabajo](https://www.adictosaltrabajo.com/2014/10/23/solid-2/)

- El precio de las excepciones comprobadas es un incumplimiento del principio abierto/cerrada, ya que si se genera una excepción comprobada desde un método de su código y la cláusula catch se encuentra tres niveles por debajo, forzaría cambios de firma en muchos niveles superiores.
- Las excepciones comprobadas pueden ser útiles si se tiene que crear una biblioteca crítica. Pero en el desarrollo de aplicaciones generales, los costes de dependencia superan las ventajas

### **Ofrecer contexto junto a las excepciones**

Las excepciones deben dar un contexto para saber el origen y la ubicación de un error

- Redactar mensajes informativos y pasarlo junto a las excepciones
- Mencionar la operación fallida y el tipo de fallo

### **Definir clases de excepción de acuerdo a las necesidades del invocador**

Formas de clasificar los errores:

1. Por origen: Cuando provienen de uno u otro componente
2. Por tipo: Fallos del dispositivo, de la red, o errores de programaciónDefinir el flujjo normal

```java
ACMEPort port = new ACMEPort(12);

try 
{
	port.open();
} 
catch (DeviceResponseException e)
{
	reportPortError(e);
	logger.log{“Device response exception”, e);
}
catch (ATM1212UnlockedException e) 
{
	reportPortError(e);
	logger.log(“Unlock exception”, e);
}
catch (GMXError e) {
	reportPortError(e);
	logger.log(“Device response exception”);
}
finally 
{
...
}
```

Podemos usar una clase como un simple envoltorio que captura y traduce excepciones.

Simplificamos el código si incluimos la API invocada y nos aseguramos de que devuelve un tipo de excepción común

```java
LocalPort port = new LocalPort(12);

**try 
{
	port.open();
} 
catch (PortDeviceFailure e)
{
	reportError(e);
	logger.log(e.getMessage(), e);
} 
finally
{
…
}
```

```java
public class LocalPort 
{
	private ACMEPort innerPort;

	public LocalPort(int portNumber) 
	{
		innerPort = new ACMEPort(portNumber);
	}
		
	public void open() 
	{
		try 
		{
			innerPort.open();
		} 
		catch (DeviceResponseException e) 
		{
			throw new PortDeviceFailure(e);
		} 
		catch (ATM1212UnlockedException e)
		{
			throw new PortDeviceFailure(e);
		} 
		catch (GMXError e) 
		{
			throw new PortDeviceFailure(e);
		}
	}
	…
}
```

Al envolver la API de terceros se minimizan las dependencias

### **Definir el flujo normal**

El patrón de caso especial: Se crea una clase o se configura un objeto que procese un caso especial. Al hacerlo, el código cliente no tiene que procesar comportamientos excepcionales. Dichos comportamientos se encapsulan en un objeto de caso especial

```java
try {
		MealExpenses expenses = expenseReportDAO.getMeals(employee.getID());
		m_total += expenses.getTotal();
} catch(MealExpensesNotFound e) {
		m_total += getMealPerDiem();
}
```

```java
MealExpenses expenses = expenseReportDAO.getMeals(employee.getID());
m_total += expenses.getTotal();
```

Podemos cambiar `ExpenseReportDAO` para que siempre devuelva un objeto `MealExpense`. 

```java
public class PerDiemMealExpenses implements MealExpenses {
	public int getTotal() {
		// devolver la dieta diaria predeterminada
	}
}
```

### **No devolver null**

- Si siente la tentación de devolver null desde un método, pruebe a generar una excepción o a devolver un objeto de caso especial
- Si invoca un método que devuelva null desde una API de terceros, envuélvalo en un método que genere una excepción o devuelva un objeto de caso especial

### **No pasar null**

Devolver null desde métodos es incorrecto, pero es peor pasar null a métodos. A menos que se trabaje con una API que espere que pase null

En la mayoría de lenguajes de programación no hay una forma correcta de procesar un null pasado por accidente, El enfoque racional es imperidr que se pase el null de forma predeterminada, 

```java
public class MetricsCalculator
{
	public double xProjection(Point p1, Point p2) {
	return (p2.x – p1.x) * 1.5;
	}
…
}
```

Esto soluciona la documentación, pero no el problema

```java
public class MetricsCalculator (
	public double xProjection{Point p1, Point p2) {
		assert p1 != null : "p1 should not be null";
		assert p2 != null : "p2 should not be null";
		return (p2.x - pl.x) * 1.5;
	}
}
```

### **Conclusión**

- El código limpio es legible pero también debe ser robusto
- Podemos crear código legible y robusto si consideramos el control de errores una preocupación diferente, algo que vemos de forma independiente desde nuestra lógica principal

# LIMITES

No es común que controlemos todo el software de nuestros sistemas. Adquirimos paquetes de terceros, usamos código abierto, etc. De algún modo debemos integrar este código externo con el nuestro

Prácticas y técnicas para definir con claridad los límites de nuestro software

### Útilizar código de terceros

- Los proveedores de paquetes y estructuras de terceros abogan por una capacidad de aplicación global para poder trabajar en diversos entornos y atraer a un público más amplio
- Los usuarios desean una interfaz centrada en sus necesidades concretas

Esta tensión puede provocar problemas en los límites de nuestros sistemas

Ejemplo con `java.util.map`

```java
Map sensors = new HashMap();
...
Sensor s = (Sensor)sensors.get(sensorId);

```

- El cliente del código es responsable de obtener un objeto de `Map` y convertirlo al tipo correcto

```java
Map<Sensor> sensors = new HashMap<Sensor>();
...
Sensor s = sensors.get(sensorId);

```

- Se mejora la legibilidad del código mediante el uso de genéricos

```java
public class Sensors {
	private Map sensors = new HashMap();

	public Sensor getById(String id) {
		return (Sensor) sensors.get(id);
	}

	//corte
}
```

- Soluciona el problema de que map<Sensor> ofrezca más prestaciones de las que necesitamos o deseamos
- La interfaz en el límite (`Map`) está oculta. Ha conseguido evolucionar sin apenas impacto en el resto de la aplicación
- La conversión y la administración de tipos se procesa dentro de la clase `Sensors`
- Se ajusta y limita a las necesidades de la aplicación
- Genera código más fácil de entender y con menor probabilidad de errores

### Explorar y aprender límites

- Nuestra labor no es probar el código de terceros, pero sí crear pruebas para el código de terceros que utilicemos
- En lugar de experimentar y probar el nuevo material en nuestro código de producción, deberíamos crear pruebas que analicen nuestro entendimiento del código de terceros. (Pruebas de aprendizaje — Jim Newkirk)
- En dichas pruebas, invocamos las API de terceros como supuestamente la usaríamos en nuestra aplicación. Básicamente realizamos experimentos controlados para comprobar si las entendemos. Las pruebas se centran en lo que queremos obtener de la API

### Aprender log4j

[Log4j - Wikipedia, la enciclopedia libre](https://es.wikipedia.org/wiki/Log4j)

### Las pruebas de aprendizaje son algo más que gratuitas

Las pruebas de aprendizaje no son solo gratuitas, sino rentables

- Si el paquete de terceros cambia de una forma incompatible con nuestras pruebas, lo sabremos al instante

Independientemente de que se necesiten los conocimientos proporcionados por las pruebas de aprendizaje, un limite claro debe estar respaldado por un conjunto de pruebas que ejerciten la interfaz de la misma forma que hace el código en producción

Sin estas pruebas para facilitar la transición, podríamos conservar la versión antigua mas de lo necesario

### Usar código que todavía no existe

Otro tipo de límite que separa lo conocido de lo desconocido: Cuando nuestro conocimiento del código parece desvancerse. Cuando lo que hay al otro lado del límite es desconocido (Al menos por el momento).

Para no quedarnos bloqueados al momento de toparnos con este tipo de límites, solo es necesario saber como queremos que fuera la dicha interfaz desconocida. Asi podemos seguir trabajando y determinar después los detalles. 

### Límites limpios

- Los límites son suceptibles al cambio. Los diseños de código correctos acomodan estos cambios sin necesidad de grandes modificaciones
- Cuando usamos código que no controlamos, hay que prestar especial atención a proteger nuestra inversión y asegurarnos de que los cambios futuros no sean demasiado costosos
- El código en los límites requiere una separación evidente y pruebas que definan expectativas
- Debemos evitar que el código conozca detalles de terceros. Es mas aconsejable depender de algo que controlemos de algo que no controlemos
- Usando los conocimientos expuestos en este capítulo:
    - El código se lee mejor
    - Promueve el uso coherente e interno en el límite
    - Hay menos puntos de mantenimiento cuando cambie el código de terceros

# PRUEBAS DE UNIDAD

Cada vez se vuelve mas importante escribir pruebas de unidad para nuestros programas. De hecho deberíamos verlas como obligatorias

### Las tres leyes de DGP

1. No debe crear código de producción hasta que haya creado una prueba de unidad que falle
2. No debe crear más de una prueba de unidad que baste como fallida y no compilar se considera un fallo
3. No debe crear más código de producción que el necesario para superar la prueba del fallo actual  

### Realizar pruebas limpias

- Tener pruebas incorrectas puede ser igual o peor que no tener pruebas
- Las pruebas cambian de acuerdo a la evolución del código, cuanto menos limpias sean, son más dificiles de cambiar

***El código de prueba es tan importante como el de producción. Requiere concentración, diseño y cuidado. Debe ser tan limpio como el código de producción***

- Las pruebas propician posibilidades
    - Las pruebas de unidad son las que hacen que el código de produccíón sea flexible y se pueda mantener y reutilizar. Si tiene pruebas, no tendrá miedo a realizar cambios en el código
    - Son la clave para mantener limpio el diseño y la arquitectura. Proporcionan posibilidades ya que permiten el cambio

### Pruebas limpias

La legibilidad es más importante en las pruebas que en el código de producción → Claridad, simplicidad y densidad de expresión

- Lenguage de pruebas específico del dominio
    - Es recomendable en lugar de usar las API que los programadores emplean para manipular el sistema, crear una serie de funciones y utilidades que usan dichas API y que facilitan la escritura y lectura de las pruebas
    - Los programadores disciplinados hacen refactorizaciones a su código de prueba
- Un estandar dual
    - Es necesario entender que las pruebas se hacen en un entorno diferente al de producción, y cada entorno tiene sus propias necesidades
    - La naturaleza del estándar dual dice que hay cosas que nunca se haría en un entorno de producción pero que son totalmente válidas en un entorno de pruebas

### Una afirmación por prueba

Hay que intentar que todas las funciones de prueba solo tengan una instrucción de `Assert`. Podemos dividir una prueba en 2, cada una con una afirmación concreta

Esta regla no es una camisa de fuerza, lo que si podemos decir que el número de afirmaciones debe ser mínimo

- Un solo concepto por prueba
    - No queremos extensas funciones que prueben diferentes cosas
    - Al combinar varios comportamientos en la misma función se obliga al lector a determinar por qué cada sección se ubica en ese punto y qué prueba dicha sección

### F.I.R.S.T

1. Fast (Rapidez)
    
    Si las pruebas se ejecutan lentamente, no las ejecutará con frecuencia, por ende, no detectará los problemas con suficiente antelación como para solucionarlos
    
2. Independent - Isolated (Independencia - Aislamiento)
    - Las pruebas no deben depender entre ellas. Una prueba no debe establecer condiciones para la siguiente
    - Se debe poder ejecutar cada prueba de forma independiente y en el orden que desee
    
3. Repeatable (Repetición)
    
    Las pruebas deben poder repetirse o ejecutarse en cualquier entorno
    
4. Self validating (Validación automática)
    
    Las pruebas deben tener un resultado booleano, o pasan,  o fallan
    
5. Thorough (Puntualidad)
    
    Las pruebas deben crearse en el momento preciso (Antes del código de producción)
    

### Conclusión

- Las pruebas son tan importantes para la salud de un proyecto como el código de producción, incluso puede que mas
- Las pruebas conservan y mejoran la flexibilidad, capacidad de mantenimiento y reutilización del código de producción
- Si las pruebas no son limpias o se corrompen, sucederá lo mismo con el código de producción

# CLASES

“No obtendremos código limpio hasta que nos fijemos en los niveles superiores de su organización”

### Organización de clases

```csharp
public class OrganizacionDeClases
{
		/*

		1. Constantes estáticas públicas
		2. Variables estáticas privadas
		3. Variables de instancia privadas.
		4. variables públicas (No suele ser necesario)

		5. Funciones públicas
		6. Regla descendente

		*/
}
```

- Encapsulación de clases
    
    Queremos que nuestras variables y funciones de utilidad sean privadas, pero no es imprescindible
    

### Las clases deben ser de tamaño reducido

- El tamaño reducido es lo principal a la hora de crear una clase
- Para medir el tamaño de una clase en vez de usar líneas físicas, lo medimos por responsabilidades
- Si no podemos derivar un nombre conciso para una clase, seguramente sea demasiado extensa o contenga muchas responsabilidades (También aplica si el nombre es demasiado ambiguo). También debemos ser capaces de escribir una breve descripción (25 palabras) sin usar las palabras si, o, y, pero

- El principio de responsabilidad única
    
    [[S.O.L.I.D.] Single responsibility principle / Principio de Responsabilidad Única - Adictos al trabajo](https://www.adictosaltrabajo.com/2014/10/22/solid-1/)
    
    - Indica que una clase o módulo debe tener uno y solo un motivo para cambiar
    - Un sistema con clases multipropósito obliga al programador a buscar entre numerosos elementos que no siempre necesitamos conocer
    - Los sistemas deben estar formados por muchas claves reducidas, no por algunas de gran tamaño.
    
    - **Cada clase reducida encapsula una única responsabilidad, tiene un solo motivo para cambiar y colabora con algunas otras para obtener los comportamientos deseados del sistema**
    
- Cohesión
    - Una clase en la que cada variable se usa en cada método tiene una cohesión máxima
    
    ```java
    public class Stack {
    		private int topOfStack = 0;
    		List<Integer> elements = new LinkedList<Integer>();
    
    		public int size() {
    				return topOfStack;
    		}
    
    		public void push(int element) {
    				topOfStack++;
    				elements.add(element);
    		}
    
    		public int pop() throws PoppedWhenEmpty {
    				if (topOfStack == 0)
    						throw new PoppedWhenEmpty();
    
    				int element = elements.get(--topOfStack);
    				elements.remove(topOfStack);
    				return element;
    		}
    }
    ```
    
- Mantener resultados consistentes en muchas clases de tamaño reducido
    - Cuando las clases pierdan cohesión, dividalas
    - Dividir una gran función en otras más reducidas también nos permite dividir varias clases en clases más reducidas
    - De este modo mejora la organización del programa y su estructura ahora es más transparente
    
    - A la hora de refactorizar
        - Suite de pruebas
        - Numerosos cambios mínimos
        - Tras cada cambio se ejecuta el programa para garantizar que el comportamiento no varía
    

### Organizar los cambios

- En un sistema limpio organizamos las clases para reducir los riesgos de los cambios
- Aislarnos de los cambios
    - Una clase `cliente`  que dependa de detalles concretos está en peligro si dichos detalles cambian. Podemos recurrir a interfaces y clases abstractas para aislar el impacto de dichos detalles
    - El uso de interfaces también ayuda a la creación de pruebas
    - Al minimizar  las conexiones de esta forma, nuestras clases cumplen otro principio de diseño: *Dependency Inversion Principle.* Que afirma que nuestras clases deben depender de abstracciones, no de detalles concretos
    
    [[S.O.L.I.D.] Dependency inversion principle / Principio de inversión de dependencias - Adictos al trabajo](https://www.adictosaltrabajo.com/2014/10/28/solid-5/)
    

# SISTEMAS

“La complejdad es letal. Acaba con los desarrolladores y dificulta la planificación, generación y pruebas de los productos”

### Como construir una ciudad

Una ciudad funciona porque tienen equipos que controlan partes concretas de la ciudad, el alcantarillado, la red eléctrica, el tráfico, la seguridad, las normativas urbanisticas, etc. Algunos se encargan de aspectos generales y otros en los detalles

En este capítulo veremos cómo mantener la limpieza en niveles superiores de abstracción, en el sistema

### Separar la construcción de un sistema de su uso

“Los sistemas de software deben separar el proceso de inicio, en el que se crean los objetos de la aplicación y se conectan las dependencias, de la lógica de ejecución que toma el testigo tras el inicio”

La separación de la construcción del sistema de su uso: 

- Reduce la complejidad del sistema
- Aumentar la calidad del código
- Facilita la construcción del sistema al permitir que cada módulo sea desarrollado por diferentes equipos o desarrolladores
- Facilita el mantenimiento del sistema a largo plazo al permitir que cada módulo sea actualizado o modificado de manera individual sin afectar el resto del sistema.

- Separar Main
    
    Es una forma de separar la construcción del uso. Trasladar todos los aspectos de la construcción a `Main` o módulos invocados por `Main` y diseñar el resto del sistema suponiendo que todos los objetos se han creado y conectado correctamente
    
    ![Untitled](Clean%20Code%2007e5b496146a46dcbc24ad00dc388f83/Untitled.png)
    
    La línea del medio representa la barrera entre main y la aplicación
    
- Factorías
    
    En ocasiones, la aplicación tendrá que ser responsable de la creación de un objeto. En este caso podemos usar el patrón de factoría abstracta para que la aplicación controle cuando crear dicho objeto, pero mantener los detalles de dicha construcción separados del código de la aplicación. En este ejemplo, la aplicación se desconecta de los detalles de creación de LineItem.
    
    ![Untitled](Clean%20Code%2007e5b496146a46dcbc24ad00dc388f83/Untitled%201.png)
    
- Inyectar dependencias
    
    Es un potente mecanismo para separar la construcción del uso
    
    En el proceso de construcción, el contenedor de inyección de dependencias crea instancias de los objetos necesarios, y usa los argumentos del constructor o métodos de establecimiento proporcionados para conectar sus dependencias
    

### Evolucionar

“Conseguir sistemas perfectos a la primera es un mito. Debemos implementar hoy, y refactorizar y ampliar mañana”

“Los sistemas de software son únicos si los comparamos con los sistemas físicos. Sus arquitecturas pueden crecer incrementalmente, si mantenemos la correcta separación de los aspectos”

- Aspectos transversales
    
    La **programación orientada a aspectos** (AOP) consiste en  asignar responsabilidades de forma transversal a la aplicación. Aspectos  transversales como la persistencia, la seguridad, las transacciones o  el almacenamiento en caché, se separan del resto de lógica de negocio para mantener un código más limpio.
    

---

### Proxies de Java

Una proxy en Java es una clase que implementa una interfaz que es idéntica a la interfaz del objeto que se está protegiendo. El cliente interactúa con la proxy como si fuera el objeto real, pero la proxy puede interceptar y controlar las llamadas al objeto real antes de pasarlas a través de la interfaz. Esto permite que la proxy realice tareas adicionales, como la validación de entrada o la manipulación de los resultados.

### Estructuras AOP Java puras

Permite la modularización del código que no está directamente relacionado con la funcionalidad principal del programa, como la seguridad, el registro, la transacción, etc.

- Aspectos de AspectJ
    
    AspectJ es una extensión del lenguaje Java que permite la implementación de AOP utilizando anotaciones y sintaxis específicas de AspectJ. También proporciona una API para programación basada en aspectos.
    

---

### Pruebas de unidad de la arquitectura del sistema

No es necesario hacer un gran diseño por adelantado  (BDUF Big Design Up Front). Podemos iniciar un proyecto de software con una arquitectura simple pero bien desconectada.

POJO: Su objetivo primordial es que las clases de la lógica de negocios no generen dependencias con el framework. Un pojo no hereda ni implementa nada en particular. lLos POJOs se utilizan comúnmente en el desarrollo de aplicaciones Java empresariales para representar objetos de negocio simples y sencillos, como entidades, DTOs (Data Transfer Objects), VO (Value Objects) y otros objetos de dominio. Debido a su simplicidad y flexibilidad, los POJOs son fácilmente comprensibles y reutilizables

**En resumen, un sistema POJO es simplemente un sistema que utiliza clases simples y sencillas que no contienen lógica de negocios compleja o acoplamiento a tecnologías específicas**

> Una arquitectura de sistema óptima se compone de dominios de aspectos modularizados, cada uno implementado con POJO. Los distintos dominios se integran mediante aspectos o herramientas similares mínimamente invasivas. Al igual que el código, en esta arquitectura se pueden realizar pruebas
> 

### Optimizar la toma de desiciones

- La modularidad y la separación de aspectos permite la descentralización de la administración y la toma de desiciones.
- También permite posponer las desiciones hasta el último momento. Si decidimos demasiado pronto, tendremos menos información del cliente, reflexión mental sobre el proyecto y experiencia con las opciones de implementación

> La agilidad que proporciona un sistema POJO con aspectos modularizados nos permite adoptar desiciones óptimas a tiempo, basadas en los conocimientos más recientes. Además se reduce la complejidad de estas desiciones
> 

### Usar estándares cuando añadan un valor demostrable

> Los estándares facilitan la reutilización de ideas y componentes, reclutan individuos con experiencia, encapsulan buenas ideas y conectan componentes. Sin embargo, el proceso de creación de estándares puede tardar demasiado para el sector, y algunos pierden el contacto con las verdaderas nececidades de aquello para lo que están dirigidos
> 

### Los sistemas necesitan lenguajes específicos del dominio

Un DSL es un lenguaje de programación diseñado para resolver problemas específicos en un dominio particular. A diferencia de los lenguajes de programación generales como Java, Python o C++, un DSL está enfocado en un dominio específico, lo que permite una mayor expresividad y simplicidad para resolver los problemas en ese dominio. Puede ser implementado como un lenguaje independiente o como una extensión de otro lenguaje existente, y puede tener una sintaxis y semántica específicas para el dominio en cuestión.

Un buen DSL (Domain-specific language) minimiza el vacío de comunicación entre un concepto de dominio y el código que lo implementa. Optimiza la comunicación entre un equipo y los accionistas del proyecto

Si se usan de manera eficaz

- Aumentan el nivel de abstacción por encima del código  y los patrones de diseño
- Permiten al desarrollador revelar la intención del código en el nivel de abstracción adecuado

### Conclusión

- Los sistemas también deben ser limpios
- Una arquitectura invasiva afecta:
    - la lógica de dominios (Si se ve afectada, la calidad se resiente, ya que los errores se ocultan y las historias son más difíciles de implementar)
    - La agilidad (Si se ve afectada, la productividad sufre y se pierden las ventajas del TDD)
- En todos los niveles de abstracción, los objetivos deben ser claros (Esto solo sucede si crea POJO y usa mecanismos similares a aspectos para incorporar otros aspectos de implementación de forma no invasiva)
- Independientemente de que diseñe sistemas o módulos individuales, no olvide usar los elementos más sencillos que funcionen

# EMERGENCIA

### Limpieza a través de diseños emergentes

Las 4 reglas de kent Beck de diseño sencillo. Un diseño es sencillo si cumple estas cuatro reglas:

- Ejecuta todas las pruebas
- No contiene duplicados
- Expresa la intención del programador
- Minimiza el número de clases y métodos

### Primera regla del diseño sencillo: Ejecutar todas las pruebas

- Los sistemas que no se pueden probar no se pueden verificar, y un sistema que no se puede verificar no debe implementarse
- Crear sistemas testables hace que diseñemos clases de tamaño reducido y un solo cometido. Resultan mas clases que cumplen el *Single Responsability Principle*
- Hacer que nuestro sistema se pueda probar nos ayuda a crear mejores diseños

- Las conexiones rígidas dificultan la creación de pruebas. Cuantas más pruebas creemos, más usaremos principios como DIP y herramientas con inyección de dependencias, interfaces y abstracción para minimizar dichas conexiones

### Reglas 2 a 4 de diseño sencillo: Refactorizar

En la fase de refactorización, podemos aplicar todos los aspectos del diseño de software correcto:

- Aumentar la cohesión
- Reducir las conexiones
- Separar las preocupaciones
- Modularizar aspectos del sistema
- Reducir tamaño de funciones y clases
- Elegir nombres más adecuados

### Eliminar duplicados

El patrón Método de plantilla es una técnica muy utilizada para eliminar duplicados de nivel superior

Es una forma de escribir código que define los pasos que deben seguirse en un algoritmo, pero deja algunos detalles específicos para que sean implementados por subclases.

```csharp
public class RecetaTorta
{
    public void Cocinar()
    {
        MezclarIngredientes();
        Hornear();
        Enfriar();
        Decorar();
    }

    public void MezclarIngredientes()
    {
        Console.WriteLine("Mezclando ingredientes de torta");
    }

    public void Hornear()
    {
        Console.WriteLine("Horneando...");
    }

    public void Enfriar()
    {
        Console.WriteLine("Enfriando...");
    }

    public void Decorar()
    {
        Console.WriteLine("Haciendo decoración de torta");
    }
}

public class RecetaGalleta
{
    public void Cocinar()
    {
        MezclarIngredientes();
        Hornear();
        Enfriar();
        Decorar();
    }

    public void MezclarIngredientes()
    {
        Console.WriteLine("Mezclando ingredientes de galleta");
    }

    public void Hornear()
    {
        Console.WriteLine("Horneando...");
    }

    public void Enfriar()
    {
        Console.WriteLine("Enfriando...");
    }

    public void Decorar()
    {
        Console.WriteLine("Haciendo decoración de galleta");
    }
}
```

```csharp
public abstract class Receta
{
    public void Cocinar()
    {
        MezclarIngredientes();
        Hornear();
        Enfriar();
        Decorar();
    }

    public abstract void MezclarIngredientes();

    public void Hornear()
    {
        Console.WriteLine("Horneando...");
    }

    public void Enfriar()
    {
        Console.WriteLine("Enfriando...");
    }

    public abstract void Decorar();
}

public class RecetaTorta : Receta
{
    public override void MezclarIngredientes()
    {
        Console.WriteLine("Mezclando los ingredientes para la torta...");
    }

    public override void Decorar()
    {
        Console.WriteLine("Decorando la torta...");
    }
}

public class RecetaGalleta : Receta
{
    public override void MezclarIngredientes()
    {
        Console.WriteLine("Mezclando los ingredientes para las galletas...");
    }

    public override void Decorar()
    {
        Console.WriteLine("Decorando las galletas...");
    }
}
```

### Expresividad

Cuanto más claro sea el código, menos tiempo perderán otros en intentar comprenderlo. Esto reduce los defectos y el coste de mantenimiento. Algunas formas de expresarse…

- Nombres adecuados:  El objetivo es ver el nombre de una clase y función y que sus responsabilidades no nos sorprendan
- Reducir el tamaño de funciones y clases: Al hacerlo, resulta más sencillo asignarles nombres, crearlas y comprenderlas
- Nomenclatura estándar: Los patrones de diseño, por ejemplo, se basan en la comunicación y en la capacidad de expresión
- Pruebas de unidad bien escritas: Uno de los principales objetivos de una prueba es servir de documentación mediante ejemplos. Los que lean las pruebas deben entender con facilidad para que sirve una clase
- La práctica: A menudo conseguimos que el código funcione y pasamos al siguiente problema sin detenernos en facilitar la lectura del código para otros. No olvide que seguramente sea el próximo que lea el código

“Afronte su creación con orgullo. Dedique tiempo a sus funciones y clases. Seleccione nombres mejores, divida las funciones extensas en otras mas reducidas y cuide su obra. El cuidado es un recurso precioso”

### Clases y métodos mínimos

En un esfuerzo por reducir el tamaño de clases y métodos, podemos crear demasiadas clases y métodos reducidos. Esta regla también sugiere minimizar la cantidad de funciones y clases

Una gran cantidad de clases y métodos suele indicar un dogmatismo sin sentido. Imagine un estándar de código que insista en la creación de una interfaz para todas las clases, o a programadores que insisten en qué campos y comportamientos siempre deben separarse en clases de datos y clases de comportamientos. Este dogma debe evitarse y cambiarse por un enfoque más pragmático

![Untitled](Clean%20Code%2007e5b496146a46dcbc24ad00dc388f83/Untitled%202.png)

### Conclusión

Las prácticas descritas en este capítulo y en el libro son una forma cristalizada de décadas de experiencia de muchos autores. La práctica del diseño correcto anima y permite a los programadores a adoptar principios y patrones que en caso contrario tardarían años en aprender