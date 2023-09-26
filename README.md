# Git-diff-and-Git-checkout-plus-caracteristicas-github

Aqui veremos que son y para que se utilizan los comando "git diff" y "git checkout".

git diff: Con este comando podremos ver las diferencias que existen entre el repositorio y el branch donde estamos trabajando. 
Para ello seguiremos los siguientes pasos: 

    1. git status <!--para ver el stado actual del area de trabajo-->
    2. Selecionaremos el archivo que queramos modificar usando el comando "nano" + la dirección de ese archivo o carpeta. 
        2.1 nano colores/rojo.txt <!--con este comando abriremos el archivo en la terminal para poder editarlo-->
        2.2 Hacemos un cambio en el archivo, en este caso, cambiaremos la frase "Las fresas son de color rojo" por "Las rosas pueden ser de color rojo" 
        2.3 Guardamos los cambios con el comando ctrl+O 
        2.4 Saldremos del modo edición con el comando ctrl+X 
    3. Luego de modificar el archivo "colores/rojo.txt" comprobamos el cambio con el comando "git diff"
        3.1 Aplicamos el comando "git diff"
        3.2 las siguientes lineas de codigo que aparecen son cada uno de los elementos del comando "git diff". 
        3.3 Se nos muestra con un "-" y de color rojo la frase que se cambio en el archivo y con un "+" y de color verde la frase por la que se cambio la frase anterior.
    

    git checkout: este comando nos sirve para cambiar entre los diferentes commits que se han hecho a lo largo del area de trabajo. Necesitaremos el indice de la version a la que queremos acceder. 

    1. Utilizamos el comando "git log" para ver los distintos commits que se han hecho. Cada commit tendra la siguiente estructura: 
        1.1 primera linea: commit <indice> <!--El indice es un conjunto de numeros y letras que identifican al commit-->
            segunda linea: El autor del commit
            tercera linea: fecha en que se hizo el commit
            Luego se mostrara el comentario con el que fue realizado el commit
    2. Tomamos el indice del commit al que queramos acceder 
    3. Salimos de la lista de commits presionando la letra "q"
    4. Aplicamos el comando "git checkout" seguido del indice al que queremos acceder
    5. Ahora entramos en un area donde podemos hacer cambios sin que afecte a las versiones anteriores. Si por alguna razón queremos guardar estos cambios, utilizamos el comando "git switch -c <nombre-del-nuevo-branch>. Si no, podemos utilizar el comando "git switch -" para volver a la versión en la que estabamos antes de utilizar el comando "git checkout". 


video explicativo 

    https://www.youtube.com/watch?v=ZomKZan8mBw&ab_channel=AdrianLovera