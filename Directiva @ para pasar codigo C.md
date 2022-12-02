La directiva @ permite escribir codigo C# dentro del codigo HTML y asi se puede tener cierta logica de programacion que sea sencilla.

Ej
		@if (numero  = = 1){
		         
			<p>El numero es 1 : @numero</p>
		}else{

			<p>El numero no es 1 es: @numero</p>
		}

		@code{
			private int numero=5;
		}




[[Pasaje de parametros en funciones inplicitas. FUNCIONES LAMDBA]]
