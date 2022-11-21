Las páginas serían difíciles de crear si tuviera que volver a escribir cada línea de HTML sin reutilizarlas entre páginas. Puede crear _componentes_ con Razor a los que se puede hacer referencia y utilizar en otros componentes o páginas.

Un archivo Razor define los componentes que conforman una parte de la interfaz de usuario de la aplicación. Los componentes en Blazor son análogos a los controles de usuario en ASP.NET Web Forms.

Si explora el proyecto, verá que la mayoría de los archivos son archivos .razor.

En el momento de la compilación, cada componente de Razor se integra en una clase .NET. La clase incluye elementos de interfaz de usuario comunes como estado, lógica de representación, métodos de ciclo de vida y controladores de eventos.
Ejemplo de ello es el componente [[Componente Counter]]
