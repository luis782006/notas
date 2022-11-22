## Agregue el componente Todo a la barra de navegación.

El componente `NavMenu` de la aplicacion Blazor se usa en el diseño de la aplicación. Los diseños son componentes que le permiten impedir la duplicación de contenido en una aplicación. El componente `NavLink` proporciona una indicación en la interfaz de usuario de la aplicación cuando la aplicación carga la dirección URL del componente.

En la sección `<nav>...</nav>` del componente NavMenu, agregue el elemento siguiente `<div>...</div>` nuevo y el componente `NavLink` para el componente `Todo`.

En `Shared/NavMenu.razor`:

![[Pasted image 20221122121950.png]]

El NavLink es un tag que ademas de la clase tiene un atributo "HREF" al cual se le pasa el valor de la ruta relativa que se declaro en el componente [[enlances y creacion de un componente.]]

Crear un elemento dentro del componente todo a traves de una [[clase c#]]  

