# Como recuperamos repositorios en Git.
Pues debemos saber utilizar el comando git reverse.
## Como utilizar el git reverse y en que se basa.
Imaginemos la siguiente situación: 
1. Estás trabajando en un archivo y añades y haces commit a tus cambios.
2. A continuación trabajas en otras cosas y haces algunos commits más.
3. Ahora te das cuenta de que, hace tres o cuatro commits, hiciste algo que te gustaría deshacer - ¿cómo puedes hacerlo?

Pues de forma fácil y sin complicaciones. Supongamos que te encuentras en el HEAD 5 y tus errores vienen sucediendo desde el HEAD 2.
Para volver al HEAD desde donde empezaron los fallos se necesitara del uso del comando git reverse de la siguiente forma:

**git reverse HEAD~2** 
