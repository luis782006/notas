Una clase contiene los atributos y metodos mas su constructores. Los metodos get y set  se definen en la creacion de la variable.

      namespace BlazorPizza.Model //hace referencia al proyecto.
	{
	    public class PizzaSpecial // nombre de clase
	    {
	    //artributos
	        public int id { get; set; }
	        public string Name { get; set; }
	        public decimal BasePrice { get; set; }
	        public string  Description { get; set; }
	        public string ImageUrl { get; set; }
	        public string GetFormattedBasePrice() => BasePrice.ToString("0.00");
	    }
	}
La sintaxis de los atributos viene con su metodo get y set. Los mismo son modificable. 
Dentro de los get y set se puede hacer uso del atributo para por defecto darle un comportamiento. Una vez se tiene acceso desde los metodos se debe tener en cuenta que el metodo get debe esta declarado con el return, no importa que el mismo no realice nada.
        public string Name
        { get
            {
                return Name;
            }
            set
            {
                Name.ToUpper();  // es el nombre del atributo o el parametro value Ej: value.ToUpper()
            } 
        }
En caso contrario si queremos usar solo el get y no el set si permite que el metodo set quede sin instanciarse.
      public string Name
        { get
            {
                return Name.ToUpper();
            }
            set
            {
            
            } 
        }

[[Proyecto Pizza]] 
