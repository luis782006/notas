para pasar los parametros se usa una funcion  Lambda que es el llamado a una funcion anonima que ejecuta un codigo o un llamado de una funcion. 
Sintaxis

      <input type="checkbox" @bind=todos[index].IsDone
       @onclick="( () => changeStatusTask(todos[index]))" />

@onclick es el metodo que ejecuta la funcion y a su vez invoca a una funcion. Esta funcion ya puede llevar parametros. 

*importante*

la funcion debe recibir un parametro del tipo de objeto que se este enviando cuando se ejecute.

       private void changeStatusTask(TodoItem todo) {
            todo.IsDone = true;
      
            StateHasChanged(); // le indica que esta funcion modificara el estado por 
                                              lo cual debe refresacarse.
        }

        <span>@(todos[index].IsDone ? "Task Complete" : "Incomplete Task")</span>

la ultima linea usa un ternario en el html el cual revisa que estado tiene el item en la posicion del LIST y le pasa el valor.

*importante*
tener en cuenta que esta si manejamos desde la logica(c# code), variables que tendran uso en el html, hay que
TENER EN CONDIDERACION QUE ESTA VARIABLE ES GLOBAL Y SI ESTA DENTRO DE UN OBJETO DE TIPO LIST, TOMARA EL VALOR PARA TODOS LOS ITEMS QUE SE VAYAN A RECORRER.
OJOOOOOOOOOOOOOOOOOOOOOOO.

[[agregar a la LIST los items.]]
