Los parámetros del componente se especifican mediante atributos o contenido secundario, que permiten establecer propiedades en el componente secundario. Defina un parámetro en el componente de contador para especificar en cuánto se incrementa con cada clic de botón:
![[Pasted image 20221122112445.png]]

[Parameter] public int IncrementAmount { get; set; } = 1;
Esto es una nueva variable que se impacta en la funcion toda variable se crea pasando su metodo de acceso el tipo y entre llaves { get; set}  sus metodos getters y setters. Para finalizar su incializacion.

En `Index.razor`, actualice el elemento `<Counter>` para agregar un atributo `IncrementAmount` que cambie la cantidad de incremento a diez, como se muestra en la última línea del código siguiente:
De esta manera se pueden traer las variables declaradas en cada reutilizacion del componente.
![[Pasted image 20221122112954.png]]

Notar la novedad de que la variable creada IncrementAcount fue declarada en el componente e inicializada en 1, y luego en la reutilizacion del componente de Index nos traemos la variable y le pasamos el valor de 10. Lo cual permite que se comporte de manera individual el componente.

Uno se aumentara en 10 y otro en 1.

Lo sigiuentes es ver como [[agregar la logica]] a la aplicacion desde ambos lados

[[Adiccion de componente]] [[Componente Counter]] [[Componentes]] 

