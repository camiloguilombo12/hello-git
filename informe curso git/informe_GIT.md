# INFORME SOBRE GIT Y GITHUB

**NOMBRE:** Juan Camilo Guilombo Osorio

**FICHA:** 3145556

**tegnologo:** ADSO

### este informe lo hago con el fin de explicar con mis propias palabras los comandos que me enseñen en el curso, documentar como progreso y lo que aprendo.


**GIT :**  sistema de control de verciones.

**pagina principal de git:**

![alt text](image.png)

---

**apartado de instalacion:**

![alt text](image-1.png)

en este apartado elegimos para que sistema operativo lo queremos y la version que requiramos.

---

**en mi caso tengo descargada esta version de git:**

![alt text](image-2.png)

el comando es: `git --version` o `git -v`

---

El comando `git --help` o `git -h` nos sirve para pedir una ayuda o guia.

![alt text](image-3.png)

---

## algunos comandos para menejar git desde una terminal 

para acceder donde queremos crear nuestra carpeta usamos **cd** con la ruta de acceso en este caso la de el escritorio `cd C:\Users\JUAN CAMILO\OneDrive\Desktop`

y para crear nuestra carpeta usamos `mkdir` y en nombre que queremos para esta, en este caso `"hello git"` y entre comillas.

luego accedemos a la carpeta 

![alt text](image-4.png)

---

## configuracion de git

`git config --global user.name "Camilo"` lo que vamos a configurar es a nivel global dentro de mi directorio en git y ponemos nuestro nombre de usuario y `config --global user.email "cguilombo587@gmail.com"` para registrar nuentro email

![alt text](image-5.png)

con esto configuramos la base de git

## conceptos principales para comenzar en git

para crear un fichero de python`echo print("Hello Git!") > hellogit.py`

![alt text](image-6.png)

![alt text](image-7.png)

---

para iniciar nuestro directorio con git `git init`

con esto sabemos que este trabaja en un repositorio de control de versiones 

![alt text](image-8.png)

---

## ramas en git

pasar de master a la rama main `git branch -m main `

![alt text](image-9.png)

## git add y commit

para ver nuestro estado `git status`

![alt text](image-10.png)

para añadir mi fichero `git add hellogit.py`

![alt text](image-11.png)


para hacer mi primer commit, agregar el comentario de el y poder subir mi archivo `git commit -m "este es mi primer commit"`

![alt text](image-12.png)

para visualizar nuestra primera fotografia que es lo que subimos `git log` y podemos ver todo como tipo historial

![alt text](image-13.png)

creamos otro fichero que se llama hellogit2.py desde visual

![alt text](image-14.png)

con `git status` podemos ver 

![alt text](image-15.png)

luego añadimos nuestro nuevo fichero a la fotografia, lo momitiamos y procedemos a ver 

![alt text](image-16.png)

ya tengo dos ficheros ingresados y dos commit

---

edite mis dos ficheros y en la consola con git status nos avisa 

![alt text](image-17.png)

---

con `git checkout` nos situamos en un punto concreto

con `git checkout hellogit2.py` borramos lo que mofificamos y restablecemos lo que teniamos en la ultima fotografia guardada en la rama

![alt text](image-18.png)

con `git reset`
nos muestra cual esta editado aun

![alt text](image-19.png)

---

edito nuevamente mi hellogit.py desde visual y esta ves si guardo y actualizo mi commit

![alt text](image-20.png)

---

con `git log --graph` los separo

![alt text](image-21.png)

--

con `git log --graph --pretty=oneline`

![alt text](image-22.png)

con `git log --graph --decorate --all --oneline`

![alt text](image-23.png)

---

**para no tener que aprenderme todo esto utilizamos alias:**

`git config --global alias.tree "log --graph --decorate --all --oneline"`

aca de dimos un alia de `tree` a `log --graph --decorate --all --oneline"` para cuando vayamos a llamar este comando tengamos que solo utilizar `git tree`

![alt text](image-24.png) 

---

`type nul > .gitignore` para crar un tipo de archivo e ignorar otros

![alt text](image-25.png)

con `git diff` puedo ver los cambios que e realizado en mi repositorio

![alt text](image-26.png)

`git checkot id_del_commit` para situarnos en ese commit

para devolvernos a `git reset --hard 75af370` y borrar lo que esta despues de este 

![alt text](image-27.png)

con `git reflog`

![alt text](image-28.png)


 creamos un tag con `git tag clase_1`

![alt text](image-29.png) 

nombre identificativo clase_1

creo otro fichero llamado **hellogit3**

y lo añado con `git add .` que es para todos los ficheros que aigan sin guardar

`git checkout tags/clase_1` para movernos entre diferentes commits y en este caso nos movimos a la que tiene la etiqueta con el tag

**comando para trabajar por ramas**

creo una rama que se llama login `git branch login`

![alt text](image-30.png)

y cambio de rama en la que trabajo con `git switch login`

creo un nuevo fichero llamado **login.py** y le hago su commit   

![alt text](image-31.png)

para poder combinar ramas `git merge main`

con `git stash` almaceno temporalmente
con `git stash drop` lo borro

![alt text](image-32.png)

para ver si tenemos algun conficto `git diff login`

![alt text](image-33.png)

## eliminacion de ramas 

con `git branch -d login` borramos la rama login

![alt text](image-34.png)

con `git brench` vemos la ramas que tengo creada y vemos todo el historial con `git reflog`

![alt text](image-35.png)


## INTRODUCCION  GITHUB

es como tipo la nube o donde vamos a subir todos nuestros repositorios en una plataforma online

![alt text](image-36.png)

### primeros pasos

creo un repositorio con el nombre de camiloguilombo

![alt text](image-37.png)

creo otro repositorio llamado hello-git para subir mi proyecto

![alt text](image-38.png)

copeo este enlace `git remote add origin https://github.com/camiloguilombo12/hello-git.git`

y lo pego en la terminal donde estamos trabajando con nuestro proyecto para saber en que repositorio lo quiero

con `git push -u origin main ` para hacer el push a la rama principal del proyecto

![alt text](image-39.png)

ya queda subido nuestro proyecto a git hub

![alt text](image-40.png)



















































































