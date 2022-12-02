
En una aplicación Blazor Server, puede crear un servicio registrado para representar un origen de datos y obtener datos de él.

Para esto se crea un Modelo de clase con sus atributos de obejtos

Es conveniente llevar un orden entre las carpetas que se van a usar.
Siguiendo el ejemplo pizza, se crea una clase Pizza que tendra sus atributos.

      namespace BlazingPizza.Model;
        public class Pizza {
        public int PizzaId { get; set; } 
        public string Name { get; set; } 
        public string Description { get; set; } 
		public decimal Price { get; set; } public bool Vegetarian { get; 
        set; } 
        public bool Vegan { get; set; } 
        }
Lo siguiente seria registrar el servicio. Se crea una Clase, se le da un nombre y por buenas prazticas le colocamos el sufijo Service, esto nos indica que sera un servicio. Ademas de tener en cuenta de crease una carpeta que nos mantenga ordenado el los servicios.
Para ello se necesita crear un clase

    namespace BlazingPizza.Model;
	     public class PizzaService { 
		     public Task<Pizza[]> GetPizzasAsync() { 
	    // Call your data access technology here
		     } 
     }
La clase usa una llamada Async para devolver los datos, coleccion de objetos Pizza. Esto da la posibilidad de ir ejecutando otro codigo mientras esta esperando los datos que de necesitan.

Siguiente paso es agregar el servicio en el Program.cs

    builder.Services.AddRazorPages(); 
    builder.Services.AddServerSideBlazor(); // Register the pizzas service  
    builder.Services.AddSingleton<PizzaService>();

Esto construye en servicio.

Ahora queda pasar al componente donde se va a usar el servicio.
el componente lleva las siguientes lineas.

	<!--// indica que se hara uso de la caperta Model y asi se tiene 
     acceso a las clases-->
    @using BlazingPizza.Data
    
    <!--// agrega el servicio al componente e inicia una nueva 
     instancia.PizzaSvc= Al nombre del Servicio que sera instanciado-->
     @inject PizzaService PizzaSvc

PizzaSvc es el nombre del servicio instanciado el cual se hara uso.

[[Metodo OnInitializedAsync()]] [[Paquetes para manejo de Base de Datos]]


