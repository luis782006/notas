Se crea un proyecto Blazor Server comun.
 crear una carpeta Model.  La misma tiene almacena una [[Clase]] 
Una vez creado el modelo que vamos a manipular podemos instanciar una lista para llevarlo a un componente.

En su codigo C# se crea una lista con el Modelo de la Clase pizza.

	@namespace BlazorPizza.Model // importar el modelo al componente
	@page "/" //ruta del componente
	<PageTitle> Pizza </PageTitle>	 
	<h1>Welcome to Pizza Hot!!!!</h1>
	
	@code{
	    // create Pizza calling Pizza Class from Model
	
	    List<PizzaSpecial> pizzaList = new(); // instancia de la Clase en una lista
	    protected override void OnInitialized()
    {
        pizzaList.AddRange(new List<PizzaSpecial>
        {
	            new PizzaSpecial { Name = "The Baconatorizor", BasePrice = 11.99M, 
                Description = "It has EVERY kind of bacon", ImageUrl = 
                "img/pizzas/bacon.jpg" },
                
                 new PizzaSpecial { Name = "Buffalo chicken", BasePrice = 12.75M, 
                 Description = "Spicy chicken, hot sauce, and blue cheese, guaranteed to 
                 warm you up", ImageUrl = "img/pizzas/meaty.jpg" },
                 
                 new PizzaSpecial { Name = "Veggie Delight", BasePrice = 11.5M, 
                 Description = "It's like salad, but on a pizza", ImageUrl = 
                 "img/pizzas/salad.jpg" },
                 
                new PizzaSpecial { Name = "Margherita", BasePrice = 9.99M, Description 
                = "Traditional Italian pizza with tomatoes and basil", ImageUrl = 
                "img/pizzas/margherita.jpg" },
 
        });
    }

  EL metodo """""protected override void OnInitialized()""""
   protected y override de tipo void llama al metodo por defecto OnInitialized() el cual es parte del ciclo de vida de Blazor. Este se ejecuta al incializar la pagina cuando ya tiene todos los valores y parametros para renderizarse.
 En la lista que se creo de tipo Clase Pizza se creo una variable la cual se ocupara de recibir una clase por el metodo heredado de la clase List y como parametro recibe una nueva List de tipo PizzaSpecial.
					     
	pizzaList.AddRange(new List<PizzaSpecial>
El metodo Add y AddRange