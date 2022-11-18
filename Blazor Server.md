Blazor Server es una implementación del marco de interfaz de usuario de Blazor como parte del marco de desarrollo web ASP.NET Core, implementado en un servidor web. El desarrollo de una aplicación con Blazor Server genera HTML en un servidor web a medida que lo solicitan los visitantes del sitio web, normalmente mediante un navegador web. Luego, ese HTML se envía al navegador del visitante y se mantiene una canalización de comunicación bidireccional mediante ASP.NET Core SignalR y se prefiere una conexión Web Sockets.

Las acciones de los usuarios que hacen clic en los botones, navegan y realizan otras interacciones con una aplicación del servidor Blazor se transmiten en esta conexión SignalR y el servidor responde con actualizaciones de la interfaz de usuario mediante la misma conexión. El marco del servidor Blazor actualiza automáticamente el navegador con el contenido generado en el servidor web.
Notar que Blazor Server y [[Blazor Assambly]] estan formados por componentes. Un ejemplo de un [[Componentes]] puede ser toda una pagina [[Paginas]]
![[Pasted image 20221117114829.png]] 


[[Mi inicio-Que es Blazor]]