# Informe-Tendencias
Realizar Informes
PASO 1:

Crear una cuenta en docker

![image](https://user-images.githubusercontent.com/91167254/197311024-d17ed63d-ca2e-46bb-8e72-d37b1eb2e11d.png)


PASO 2:

Ingresar a PlayWith Docker

![image](https://user-images.githubusercontent.com/91167254/197311192-90b8086f-68ad-4985-88b9-5c557d1e2a99.png)


PASO3:

Para cargar las librerias usar el comando: docker run --name serverweb -p 80:80 -d nginx

![image](https://user-images.githubusercontent.com/91167254/197311265-1dd18312-369d-4a24-930d-86a89c8f34bc.png)


PASO 4:

Para ver los contenedores que estan corriendo usar el comando: docker ps

![image](https://user-images.githubusercontent.com/91167254/197311293-8634f532-95de-4dc7-bd6b-1fe61d767372.png)

DOCKER RUN ---> CORRER UN CONTENEDOR

DOCKER PS ---->> LISTAN LOS CONTENEDORES QUE ESTAN CORRIENDO 

(-- NAME SERVERWEB) -----> ES PARA COLOCAR UN NOMBRE Y SIRVE PARA IDENTIFICAR EL DOCKER Y DONDE ESTA CORRIENDO

80:80 ---> MAQUINA ANFITRIONA 


-d ===> nos sirve o permite seguir ocupando la linea de comandos caso contrario no se va a poder ,ademas si usamos el proceso pasa a segundo plano 

nginx ==> imagen que se descargan ,en base a esa imagen se crea el contenedor


EJECUCIÒN DE CONTENEDORES WEBSERVER

Primero se crea un archivo HTML en el repositorio y junto a esto crear un codigo html, poner el nombre de quien hizo el codigo para verificar si funciona bien.

![WhatsApp Image 2022-10-21 at 21 46 05](https://user-images.githubusercontent.com/91167254/199111932-07cf372b-2756-4d69-91a5-82d253562568.jpeg)

Se ingresa el comando : wget(junto a esto el link del repositorio donde se creó el codigo html)//https://github.com/dflandi/Informe-Tendencias/blob/main/index2.html

![WhatsApp Image 2022-10-21 at 21 45 43](https://user-images.githubusercontent.com/91167254/199112663-76e0cb5a-11ff-4ab1-b3f9-dac2c68f002f.jpeg)

Ingresar el código ls para ver si se pudo adjuntar el codigo con el Docker

![WhatsApp Image 2022-10-21 at 21 46 18](https://user-images.githubusercontent.com/91167254/199112872-8e3d721f-8b9c-4f04-b831-2c36c7587528.jpeg)

Luego de esto ingresar el comando docker cp index2.html miweb:/urs/share/nginx/html/index2.html (El comando sirve para añadir la informacion del html)

Abrir el puerto y poner 80 para verificar si se ve el html.

![WhatsApp Image 2022-10-21 at 21 46 18](https://user-images.githubusercontent.com/91167254/199113343-cde9a7cc-0f5d-445b-931e-1274c68e9275.jpeg)

Si al abrir el port y poner 80, nose inicia nada o sale error poner los siguientes comandos:

- vi index2.html
- git clone https://github.com/dflandi/Informe-Tendencias (el respositorio donde esta el html)
- y ls para verificar si se cargó con exito
- 
![WhatsApp Image 2022-10-21 at 21 46 54](https://user-images.githubusercontent.com/91167254/199114122-d506cdfa-a3dc-4ea2-9f33-be2f160e9a3d.jpeg)

Nuevamente utilizar el comando docker cp index2.html miweb:/urs/share/nginx/html/index2.html

![WhatsApp Image 2022-10-21 at 21 46 56](https://user-images.githubusercontent.com/91167254/199114140-58401d55-4181-44e0-a30d-7cf58a9ca674.jpeg)

Entrar en la carpeta del repositorio donde está el html con el comando cd Informes-Tendencias/ (el nombre que pusieron en la carpeta de su repositorio)

![WhatsApp Image 2022-10-21 at 21 47 06](https://user-images.githubusercontent.com/91167254/199114357-24e0a9bc-3cc8-4a5c-a7c2-55a48b5a92cb.jpeg)

Por ultimo, abrir el port y poner 80, esta vez si se abra con la informacion que se puse en el repositorio del html

al abrir la paguina en el link o enclace al final se debe poner /index2.html 

![WhatsApp Image 2022-10-21 at 21 47 17](https://user-images.githubusercontent.com/91167254/199114711-05c38f97-2288-46a1-beb3-93d69d3d4d59.jpeg) 

El contenido no se puesto que no puse nada en el body del codigo del html, si no en el tittle del html.





