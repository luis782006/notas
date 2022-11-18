Blazor WebAssembly, a veces abreviado como Blazor WASM, es una implementación del marco de interfaz de usuario de Blazor que se ejecuta en el tiempo de ejecución estándar de WebAssembly HTML 5 presente en todos los navegadores modernos. La salida binaria de su aplicación, los archivos DLL, se transmiten al navegador y se ejecutan con una versión de .NET que ha sido optimizada para funcionar con el tiempo de ejecución de WebAssembly, independientemente del sistema operativo subyacente del dispositivo que navega al sitio web.

Dado que WebAssembly es una tecnología que se ejecuta completamente en el navegador, es posible implementar este modelo de aplicación Blazor mediante archivos que un servidor web no analiza ni interactúa. Este tipo de enfoque "estático" reduce los requisitos de un servidor web y traslada todo el procesamiento de la aplicación a la máquina del usuario.

El procesamiento y la lógica avanzados pueden tener lugar en el navegador. Cuando la aplicación necesita datos o para interactuar con otros servicios, puede usar tecnologías web estándar para comunicarse con los servicios HTTP.
Ambas tecnologias [[Blazor Server]] , Blazor Assembly estan formadas de componentes, un ejemplo global de un [[Componentes]] puede ser una [[Paginas]]
![[Pasted image 20221117114933.png]]



[[Mi inicio-Que es Blazor]]