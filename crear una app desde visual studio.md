lazor permite que los desarrolladores de C# usen sus habilidades para crear aplicaciones web con C# y Microsoft.NET.

Imagine que está creando una aplicación web del lado del cliente y ya tiene un equipo de desarrolladores de .NET. Además, imagine que desea implementar su aplicación como una aplicación web progresiva. Luego, los usuarios podrían descargar la aplicación y usarla sin conexión.

Con Blazor, los desarrolladores pueden crear lógica de front-end y back-end para aplicaciones web con lenguajes, marcos y herramientas comunes.

Usar el mismo lenguaje para el código front-end y back-end puede:

-   Acelerar el desarrollo de aplicaciones.
-   Reduzca la complejidad de la canalización de compilación.
-   Simplifique el mantenimiento.
-   Permita que los desarrolladores entiendan y trabajen tanto en el código del lado del cliente como del lado del servidor.

Desde  [Visual Studio 2022](https://visualstudio.com/) después de entender como funciona [[Mi inicio-Que es Blazor]] puede aplicar sus conceptos mediante un entorno de desarrollo como Visual Studio para Mac (macOS) o continuar con el desarrollo mediante Visual Studio Code (Windows, Linux y macOS) o Visual Studio.

Para configurar un proyecto de Blazor con el que trabajar, usaremos Visual Studio 2022. Visual Studio Code incluye plantillas integradas y un compilador, lo que facilita la creación y creación de un nuevo proyecto.

1.  En Visual Studio 2022, seleccione **Archivo** > **Nuevo proyecto** .
    
2.  En el cuadro de búsqueda en la parte superior del cuadro de diálogo "Crear un nuevo proyecto", ingrese "Blazor Server", seleccione **Blazor Server App** y seleccione **Next** .

![[visual-studio-2022-create-new-project.png]]
En la siguiente pantalla, nombre su proyecto "BlazorApp", especifique una ubicación en el disco con configuraciones como las siguientes, luego seleccione **Siguiente** :
]]![[visual-studio-2022-configure-project.png]]
1.  En la pantalla _Información adicional , seleccione_ **.NET 6.0 (soporte a largo plazo)** en el cuadro combinado Framework. Deje las demás configuraciones como predeterminadas y seleccione **Crear** .
    
2.  Este comando crea un proyecto de servidor Blazor básico con todos los archivos y páginas necesarios.
    
Habiendo hecho esto podemos pasar a ejecutar la aplicacion [[Ejecutando la app]]