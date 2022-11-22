	Las directivas de Razor son marcado de componente que se usa para agregar C# en línea con HTML. Con las directivas, los desarrolladores pueden definir instrucciones, métodos o bloques de código más grandes.

### Directivas de código

Las directivas de código deberían resultar familiares a los desarrolladores que han usado Razor en MVC o en páginas.

Puede usar `@expression()` para agregar una instrucción de C# alineada con el código HTML. Si necesita más código, use la directiva `@code` para agregar varias instrucciones entre paréntesis.

También puede agregar una sección `@functions` a la plantilla para los métodos y las propiedades. Se agregan a la parte superior de la clase generada, donde el documento puede hacerles referencia.
### Directiva Page

La directiva `@Page` es un marcado especial que identifica un componente como una página. Puede usar esta directiva para especificar una ruta. La ruta se asigna a una ruta de atributo que el motor de Blazor reconoce para registrar la página y acceder a ella.

Ejemplo de [[enlances y creacion de un componente.]]


[[agregar la logica]]
