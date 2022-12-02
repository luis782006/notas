Las variables en C# y tiene ssus funciones predeterminadas. clases que heredan sus funciones.
En este caso se emplea de la Clase TodoItems que al ser parte de la clase LIST<> y con la funcion COUNT permite devolver la cantidad de elementos en la lista.
![[Pasted image 20221123111124.png]]
de esta manera con la diretciva @bind tenemos se invoca el metodo COUNT quien recibe un parametro que pasa por la condicion "Si tarea distinto a true (ya que es una atributio booleano) pues que lo cuente"  

tambien se puede invocar una funcion desde una etiqueta html que se ejecuta cuando la misma es renderizada en el DOM.

     <h1>Hello, @getFullName()</h1>
     
	 @{
		  private string name = "Luis";
	
	      private string getFullName(){
	        return name + " Sanchez";
	      }
 
	 }


 
 
 
 
 
 
 
 
 [[Enlace de lista de item]]  [[enlances y creacion de un componente.]] [[Componentes]]
