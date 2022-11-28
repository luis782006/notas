Los componentes se crean añadiendolo desde el explorador de solucion  
	    
	    <h1>Welcome to Pizza<h1/>				
		@code{
			private string nombre="Luis";
		}
 Esto seria lo basico al crear un compomente. Luego queda el uso de directivas en caso que se necesite, como por ejemplo el de @page 
 La cual indica la ruta de la pagina siendo este componente una pagina.
			
			@page "/" 
Esta directiva indica cual seria el nombre de la pagina.

		 @page "/home"

Bindear variables con componentes solo requiere una variable en la parte de codigo c# dentro de 

		@code{
			private string nombre="Luis";
		}
A la hora de mostrar esta variable en el html del componente solo queda usar la directiva del bind 

	<h1>@nombre</h1>
    @code{
	   private string nombre="Luis" ;
    }

-   **La directiva `@page`**: esta directiva proporciona una plantilla de ruta a Blazor. En tiempo de ejecución, Blazor busca una página para representarla emparejando esta plantilla con la dirección URL solicitada por el usuario. En este caso, puede coincidir con una dirección URL con el formato `http://yourdomain.com/index`.

-   **La directiva `@code`**: esta directiva declara que el texto del bloque siguiente es código C#. Puede colocar tantos bloques de código como necesite en un componente. Puede definir miembros de clase de componente en estos bloques de código y establecer sus valores mediante cálculo, operaciones de búsqueda de datos u otros orígenes. En este caso, el código define un único miembro de componente denominado `welcomeMessage` y establece su valor de cadena.

-   **Directivas de acceso de miembros**: Si quiere incluir el valor de un miembro en la lógica de representación, use el símbolo `@` seguido de una expresión C#, como el nombre del miembro. En este caso, la directiva `@welcomeMessage` se usa para representar el valor del miembro `welcomeMessage` en las etiquetas `<p>`.

[[Proyecto Pizza]]