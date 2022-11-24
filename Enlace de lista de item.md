-   Agregue un campo a los elementos de tareas pendientes en un bloque `@code`. El componente `Todo` utiliza este campo para mantener el estado de la lista de tareas pendientes.
- 
-   Agregue el marcado de la lista no ordenada y un bucle `foreach` para que cada elemento de la lista se represente en un elemento de la lista de tareas pendientes (`<li>`).
![[Pasted image 20221122131903.png]]
Esto hara que se recorra el objeto todos (variable creada de tipo TodoItem, clase creada) y asi mostrar todos los items, ya que esa clase se le pasa a una LIST.

****Importante****
si se recorre la funcion con un foreach los objetos son inmutable, lo cual no permitira que se modifique los elementos.
Para esto se utilizara un for comun.


[[clase c]]     [[enlances y creacion de un componente.]]

La siguiente tarea es [[agregar a la LIST los items.]]


