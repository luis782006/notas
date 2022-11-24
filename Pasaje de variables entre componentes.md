Para los pasajes de variables entre componentes requiere el uso de funciones / metodos donde recibe parametros que son variables de uno u otro componente. bajo el patrón
_“props-down & events-up”_  

Componente que manda la info.

      <button class="btn btn-primary" @onclick="metodoEnviar" >Click me</button>

Se crea un boton que ejecutara un metodo el cual se va a encargar de enviar el valor de la variable.

   @code {
    [Parameter] // anotacion 
    public string apellido { get; set; } // se declara na variable la cual llevara los metodos 
                                                        //get y set

    [Parameter]
    public EventCallback<string> NombreCompleto{ get; set; }
    //Este EventCallback es el tipo de evento que ejecutara el propio evento 
    //NombreCompleto que como indica es de tipo <string>
    // Este FullName forma parte de la clase EventCallback es por ello que tendra 
     //acceso a sus metódos
    
    //Evento ClickCambiarNombre
    public void ClickCambiarNombre(){
        NombreCompleto.InvokeAsync(apellido="Sanchez");
    }
    // Este evento invoca FullName y llama al metodo InvokeAsync y por parametros 
     //envia la variable.

			// Este es el metodo que invoca el CLick del boton que a su vez invoca el 
             //metodo
    private void metodoEnviar()
    {
        ClickCambiarNombre();
        // Metodo que ejecuta la clase NOmbreCOmpleto con su metodo InvokeAsync
        // Pasando por parametro la variable.

        StateHasChanged();// indica que este metodo va a hace un cambio en el DOM.
    }

    }

    

Ahora el componente que recibe la variable

        <Counter apellido="apellido" ClickCambiarNombre="UpdateName" />
        // Declaro el componente y con el le paso dos parametros con sus valores.
    


		@code{
    public string? apellido; // apellido1 es la variable  que viene del otro 
     //componente y la variable "apellido" es la que esta declarada en el 
     //componente actual.

    // Este el metodo que recibe una variable y se la pasamos al la variable 
     //apellido. Este metodo esta enrolado con el ClickCambiarNombre
    private void UpdateName(string nombre){
        apellido = nombre;
    }
}

[[Funciones predeterminadas. ]]  [[Pasaje de parametros enfunciones FUNCIONES LAMDBA]] 
 
 [[Enlace de lista de item]]  [[enlances y creacion de un componente.]] [[Componentes]]
