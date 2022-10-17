# Ejercicio 5
1. Creación de ramas:
- Crea la rama rama-TUNOMBRE
`$ git branch rama-Javier`
![alt text](fotos/1.png)
- Posiciona tu carpeta de trabajo en esta rama
`$ git checkout rama-Javier`
![alt text](fotos/2.png)
2. Añade un fichero y crea la rama remota
- Crea un fichero llamado despligue.md con únicamente una cabecera DESPLIEGUE DE APLICACIONES WEB
![alt text](fotos/3.png)
- Haz un commit con el mensaje “Añadiendo el archivo despliegue.md en la ramaTUNOMBRE”
`$ git commit -m "Añadiendo el archivo despliegue.md en la rama-Javier"`
 ![alt text](fotos/4.png)
- Sube los cambios al repositorio remoto. NOTA: date cuenta que ahora se deberá hacer con el comando git push origin rama-TUNOMBRE
`$ git push origin rama-Javier`
 ![alt text](fotos/5.png)
3. Haz un merge directo
- Posiciónate en la rama master
`$ git checkout main`
 ![alt text](fotos/6.png)
 - Haz un merge de la rama-TUNOMBRE en la rama master
`$ git merge rama-Javier`
 ![alt text](fotos/7.png)
4. Haz un merge con conflicto
- En la rama master añade al fichero despliegue.md una tabla en la que muestres los temas de la primera evaluación de Despliegue de Aplicaciones Web
 ![alt text](fotos/8.png)
- Añade los archivos y haz un commit con el mensaje “Añadida primera evaluación Despliegue”
`$ git commit -m "Añadida primera evaluación Despliegue"`
 ![alt text](fotos/9.png)
- Posiciónate ahora en la rama-TUNOMBRE
`$ git checkout rama-Javier`
 ![alt text](fotos/10.png)
- Escribe en el fichero despliegue.md otra tabla con los temas de la segunda evaluación de Despliegue de Aplicaciones Web
 ![alt text](fotos/11.png)
- Añade los archivos y haz un commit con el mensaje “Añadida tabla segunda evaluación Despliegue”
`$ git add .`
`$ git commit -m "Añadida segunda evaluación Despliegue"`
 ![alt text](fotos/12.png)
- Posiciónate otra vez en master y haz un merge con la rama-TUNOMBRE
`$ git checkout main`
 ![alt text](fotos/13.png)
`$ git merge rama-Javier`
 ![alt text](fotos/14.png)
5. Arregla el conflicto
- Arregla el conflicto editando el fichero despliegue.md y haz un commit con el mensaje “Finalizado el conflicto de despliegue.md”
 ![alt text](fotos/15.png)
`$ git commit -m "Añadida segunda evaluación Despliegue"`
 ![alt text](fotos/16.png)
6. Tag y borrar la rama
- Crea un tag llamado v0.2
`$ git tag v0.2`
 ![alt text](fotos/17.png)
- Borra la rama-TUNOMBRE
`$ git branch -d rama-Javier`
 ![alt text](fotos/18.png)
 7. Documenta todo y finaliza el ejercicio
 - En el fichero README.md crea una nueva sección en la que vayas documentando todo lo que vas realizando en esta tarea.
 ![alt text](fotos/19.png)
 - Documenta todos los puntos en el README.md, haz un commit y sube los cambios al servidor 
`$ git add .`
`$ git commit -m "ejercicio 5"`
  ![alt text](fotos/20.png)