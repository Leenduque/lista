<!DOCTYPE html>
<html>

    <head>
        <title>Lista de tarefas</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <h1>TAREFAS</h1>
        <input>
        <button onclick="add()">Adicionar</button>
        <ul>
            <li></li> 
        </ul>

        <script>

            function add(){
                const ul = document.querySelector("ul")
                const input = document.querySelector("input")
                const tarefa = input.value 
                
                if (tarefa === "" ) {
                    alert("Você precisa digitar uma nova tarefa");
                    return;
                }
                const li = document.createElement("li")
                li.innerText = tarefa 
                ul.appendChild(li)

                const botaoApagar = document.createElement("button");
                botaoApagar.textContent = "Apagar";
                botaoApagar.className = "apagar";
                botaoApagar.onclick = function () {
                li.remove(); // remove o item da lista
      };

      // Adicionar o botão ao item da lista
      li.appendChild(botaoApagar);





                input.value = ""
            }

            
            
        </script>
    </body>
</html>