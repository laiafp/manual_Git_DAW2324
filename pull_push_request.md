# Manual Git CicloSuperior
## Trabajo colaborativo - Pull request y Push Request
1. Lo pimero que debemos hacer es entrar en el repositorio público de la profesora **libro2** https://github.com/laiafp/libro2.
2. Hacemos un **Fork** para crearnos un proyecto nuevo a partir de **libro2** asignándole el nombre de **libroCarlos**.
3. Desde nuestro GitHub abrimos el repositorio libroCarlos que acabamos de generar y pulsamos en el botón **Code**. Esto nos permitirá copiar la url que posteriormente usaremos para clonarlo desde la terminal de ubuntu.
4. Abrimos la terminal de ubuntu y hacemos un **clone** del repositorio.<br />
 ***
 **Clone**: Copia exacta del repositorio, cuando un programador llega nuevo, lo primero que debe hacer es clonar el repositorio en su equipo local. A la copia de nuestro repositorio le hemos asignado el nombre de repositoriofork.
 ***
```
sudo git clone https://github.com/carlosvigan/libroCarlos.git repositoriofork
```
5. Nos colocamos dentro de la carpeta repositoriofork.
```
carlos@carlos-VirtualBox:~$ cd repositoriofork/ 
```
6. Nos creamos el fichero pruebaGit.txt y luego mostramos su contenido.
```
carlos@carlos-VirtualBox:~/repositoriofork$ sudo nano pruebaGit.txt 
carlos@carlos-VirtualBox:~/repositoriofork$ cat pruebaGit.txt  
Prueba de Carlos para ver como funciona el pull y merge
```
7. Subimos el fichero pruebaGit.txt al area de intercambio staging area.
```
carlos@carlos-VirtualBox:~/repositoriofork$ sudo git add pruebaGit.txt  
```
8. Hacemos un commit aplicandole un comentario para subir el fichero pruebaGit.txt a nuestro repositorio local.
```
carlos@carlos-VirtualBox:~/repositoriofork$ sudo git commit -m "Subiendo pruebaGit.txt al repositorio local" 
[main 9c3b716] Subiendo pruebaGit.txt al repositorio local 
1 file changed, 1 insertion(+) 
create mode 100644 pruebaGit.txt 
```
9. Hacemos un push para subir el fichero pruebaGit.txt desde nuestra rama main del respositorio local al repositorio de Github **libroCarlos**.
```
carlos@carlos-VirtualBox:~/repositoriofork$ sudo git push origin main 
Username for 'https://github.com': carlosvigan 
Password for 'https://carlosvigan@github.com':  
Enumerando objetos: 4, listo. 
Contando objetos: 100% (4/4), listo. 
Comprimiendo objetos: 100% (3/3), listo. 
Escribiendo objetos: 100% (3/3), 407 bytes | 407.00 KiB/s, listo. 
Total 3 (delta 0), reusado 0 (delta 0), pack-reusado 0 
To https://github.com/carlosvigan/libroCarlos.git 
ce4e04b..9c3b716  main -> main 
```
10. Desde nuestro repositorio de Github **libroCarlos** hacemos un **Pull request** para mandarle una petición de validacion al repositorio público de Laila **libro2**.
11. Si la profesora acepta la petición de validación que le mandamos a través del **Pull request**, ella misma se encargará de fusionar los cambios realizando un **merge**.
