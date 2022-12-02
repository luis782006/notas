Para agregar elementos de tareas pendientes a la lista, la aplicación requiere elementos de la interfaz de usuario. Agregue una entrada de texto (`<input>`) y un botón (`<button>`) debajo de la lista no ordenada (`<ul>...</ul>`):

Estando en el mismo componente agregamos los elementos de html para la tarea.


![[Pasted image 20221122144214.png]]
 Los elemento interactuan con el C# con las directivas @onclick se invoca el metodo que se va a ejecutar AddToDo. 
A su vez la funcion tiene un Condicional que evalua si el objeto string newTodo que a su vez esta bindeado con el input esta vacio, devuelve false y no continua, en caso contrario agrega a la LIST con su objeto TodoItem en su propiedad TITLE lo que ingreso por el input. Finalmente limpia el input mediante la variable newTodo=string.empty.
[[consideraciones de bindeado.]]

 El metodo se dispara y ejecuta su logica.
 ![[Pasted image 20221122145522.png]]
[[Funciones predeterminadas. ]]  [[Pasaje de parametros en funciones inplicitas. FUNCIONES LAMDBA]] [[Pasaje de variables entre componentes]]
 
 [[Enlace de lista de item]]  [[enlances y creacion de un componente.]] [[Componentes]]
 
