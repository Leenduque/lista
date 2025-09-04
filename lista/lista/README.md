<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>lista</title>

</head>
<body>
    <h1>Tarefas</h1>
    <input>
    <button onclick="add()">criar mais</button>
    <ul>
        <li>html</li>
    </ul>

    <script>
        function add(){
            const ul = document.querySelector("ul")
            const input = document.querySelector("input")
            const tarefa = input.value

            const li = document.createElement("li")
            li.innerText = tarefa 
            ul.appendChild(li)
        }
            
          
    </script>

</body>
</html>