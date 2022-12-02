Funciones inplicitas en evento onclick
			
		<h1>@variable</h1>
       <button @onclick=@(()=>{   variable="algo";  })>Click</button>

Esta funcion se ejecuta dentro del evento onclick del boton. Al tener una variable bindeada en el HTML la funcion se ejecuta y le envia el nuevo valor.
La variable debe estar declarada dentro de la porcion @code{

}

[[Directiva @ para pasar codigo C# en HTML]]