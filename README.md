# PROYECTO DE PRUEBAS JENKINS
Este proyecto se va a utilizar para hacer pequeñas pruebas con Jenkins:
* Conectar un Job de Jenkins con este repositorio
* Que un Job se lance cuando se haga un cambio en el repositorio
* Pasar pruebas unitarias con mocha
* Probar Webhook

# PRACTICA JENKINS
Para esta practica se tendran que realizar diversas tareas:
0. Crear Crear un repositorio propio de Github con el contenido de /code
1. Crear dos usarios en Jenkins
2. Instalar el plugin de sonar y NodeJS
3. Configurar los dos plugins en correctamente  
4. Crear un job que pase los test que vienen includido cada vez que se hace un push al repositorio
5. Crear un job que pase un escaner de SonarQube cada vez que se hace un push al repositorio
6. Crear un Job que envie un correo a los usuarios cuando el test se haya pasado correctamente

# AYUDA 
Para esta practica se puede instalar SonarQube y Jenkins como se quiera pero se recomineda que se 
instale por medio de Docker ya que es muy facil de crear los contenedores correspondientes.

Si se instala con Docker puede que tengamos dificultad a la hora de configurar el plugin de SonarQube en Jenkis,
en el caso de que nos salta el error "ERROR: SonarQube server [localhost:9000] can not be reached" al colocar 
como ubicación del servidor de SonarQube http://localhost:9000, deberemos cambiarla por la IP del contenedor,
para saber esto debemos ejecutar el siguiente commando: 

```
docker inspect -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' <nombre contenedor de sonar>
```

Y colocar esa ip seguida del puerto en la configuracion del SonarQube (ej: http://172.20.0.1:9000). Otra forma de
arreglar este problema es creando una nueva red de docker y colocando los contendores en ella, y en la configuración
de SonarQube poner el nombre del conatendor (ej: sonar:9000). 
kjashdkaksdkashdkasjkddksdh
lkasjdhksajhdjksahdkjsad
lkjahskdjhsakdhksajd
kjhsadksahdhksadk
ldashdkdaksdç
askdhsakdhasjkdhsdks

jfhdskjfhdsfhjkdsfhkjdshfjkdhfç
kjdsfhlkdshfkjl
khsdlflkdsjhfd
lksjdhflksdhf
lkjshdfkdshfsdkjfh