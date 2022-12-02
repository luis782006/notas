Para agregar clases a componentes Blazors se puede hacer de varias formas.
Desde la raiz donde se crean las clases y cualquier componente puede acceder a esa clase.
Otra variante es inyectar styles dentro de los elemento html de forma directa.
La siguiente variante es crear una etiqueta style dentro del componente y manejar las clases y estilos de los elementos del componente.
La ultima seria crear un archivo razor.css y manejar lass clases y los estilos.
Ej:
 miComponente.razor
 miComponente.razor.css
 Esto lo que hace es meter dentro del componente el archivo css. Ya estan conectados no hay que indicar nada.

 ![[Pasted image 20221129112326.png]]
 