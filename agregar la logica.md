Ha definido la interfaz de usuario de la aplicación web. Ahora, vamos a explorar cómo agregar lógica a la aplicación. En una aplicación Blazor, puede agregar código de C# en archivos .cs independientes o insertados en los componentes de Razor.

En Blazor se puede agregar codigo archivos de c# directo a la aplicacion . Se le llama codigo subyacente.
Esta técnica usa archivos de código independientes para almacenar la lógica de la aplicación. Los archivos independientes son una estrategia excelente cuando la lógica de negocios es compleja, es larga o tiene varias clases. NO asi cuando es una aplicacion simple.

## Componentes de C# en línea

Es habitual mezclar HTML y C# en un único archivo de componente de Razor. Para los componentes simples con requisitos de código más ligeros, este enfoque funciona bien. Para agregar código a un archivo Razor, usará [[directivas]].

Ejemplo

@code{
 logica dentro de un razor.cs
}



