![[Pasted image 20221118014826.png]]
Dentro de ella nos encontramos con

![[Pasted image 20221118014855.png]]

@page "/counter" nos indica el path de la ruta a la que se navego dentro del explorador.
@page es una directiva de Blazor
La siguiente linea se setea el nombre de la pagina que va a figurar en la pestaña del navegador
<PageTitle></PageTitle>
EL resto de la pagina esta compuesto por codigo html y la logica que manejara esta pagina encerrado con la NOTACION @code{ logica }. Aunque tambien dentro del codigo html tambien se puede hacer uso de C# siempre con la @ y dentro del paretensis la logica en C#

			  <p>Esto es un parrafo @(2+2)</p>


[[Funciones predeterminadas.]]

nota: Este componente ya fue modifcado para ver el uso de variables indicado con ([ parameter] ) y declarando bajo de esta linea una variable. Esta variable tiene un get y set y se le da un valor incial de 1.
Luego viene el método  declarado .

El boton tiene la llamada al metodo para incrementar el numero que se muestra con el tag html "p" 
@onclick="incrementCount"

Como se especifico antes COUNTER  es un [[Componentes]] asi que se puede reutilizar agregando el componente a otro. [[Adiccion de componente]]
