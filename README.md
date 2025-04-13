# Despliegue de dos servidores web con Nginx en contenedores 

## 2. Tiempo de duración

**40 minutos**

## 3. Fundamentos

Docker es una plataforma de contenedores que permite ejecutar aplicaciones de forma aislada en un mismo sistema operativo. Uno de los usos más comunes de Docker es desplegar servidores web como Nginx de forma rápida, sin necesidad de instalarlo directamente en el sistema anfitrión.

Nginx, por su parte, es un servidor web de alto rendimiento que se utiliza para servir contenido estático, actuar como proxy inverso, balanceador de carga, entre otros. En esta práctica, lo utilizamos para servir páginas HTML personalizadas en dos contenedores distintos.

Los comandos `docker run`, `docker cp`, y `docker ps` son esenciales para gestionar los contenedores. Con `docker run` se puede crear y ejecutar un contenedor a partir de una imagen, mientras que `docker cp` permite copiar archivos entre el host y el contenedor, útil para modificar el contenido del sitio.

Además, entender cómo funcionan los puertos (`-p 8089:80`) permite mapear el puerto interno del contenedor al puerto del host, lo que facilita el acceso desde el navegador.

También se requiere una comprensión básica de HTML para editar los archivos `index.html` y personalizar el contenido que se desea mostrar.

## 4. Conocimientos previos

Para realizar esta práctica el estudiante necesita tener claro los siguientes temas:

- Comandos básicos de Linux
- Manejo de navegador web
- Uso básico de Docker (instalación, ejecución y gestión de contenedores)
- Estructura básica de un archivo HTML

## 5. Objetivos a alcanzar

- Implementar contenedores con Nginx utilizando Docker.
- Manipular archivos de configuración dentro de contenedores.
- Comprender la relación entre puertos del host y del contenedor.
- Servir contenido web personalizado desde distintos contenedores.

## 6. Equipo necesario

- Computador con sistema operativo Windows / Linux / MacOS
- Cuenta en [Docker Play](https://labs.play-with-docker.com/) o instalación local de Docker
- Docker versión 20.10 o superior
- Navegador web (Chrome, Firefox, etc.)
- Editor de texto (nano, vi, VS Code)

## 7. Material de apoyo

- Documentación oficial de Docker: https://docs.docker.com
- Guía de la asignatura proporcionada por el docente
- Linux Command Cheat Sheet: https://cheatography.com/davechild/cheat-sheets/linux-command-line/
- Tutoriales en línea sobre Nginx y HTML

## 8. Procedimiento

### Paso 1: Crear el primer contenedor Nginx
![imagen 1](https://github.com/user-attachments/assets/b3123135-4947-4bcb-b5ed-fa1e4ba9d39f)
### Paso 2: Crear el segundo contenedor Nginx
![image 2](https://github.com/user-attachments/assets/745047f5-6ec1-41e7-a7c1-4f3604aaf4a4)
### Paso 3: Copiar el archivo index.html del contenedor nginx1 al host
 ![image 3](https://github.com/user-attachments/assets/c06f9856-4ba2-4a95-85f4-b976e14b7ccf)
### Paso 4: Editar el archivo index1.html con contenido institucional
![image 4](https://github.com/user-attachments/assets/a8448f6e-024e-468c-94c6-f0a1f7259ae0)
### Paso 5: Copiar el archivo editado de vuelta a nginx1
![image 5](https://github.com/user-attachments/assets/cbbab002-496a-4f8d-b4b5-939f97ccf1e8)
### Paso 6: Repetir el proceso para nginx2 con información personal
![image 6](https://github.com/user-attachments/assets/bcfd5e61-99be-4e66-8b7d-edf8a19cc9de)
### Paso 7: Editar index2.html con contenido personal
![image 7](https://github.com/user-attachments/assets/67e20097-d1ac-4032-9e02-576465bb03d2)
### Paso 8: Copiar index2.html a nginx2
![image 8](https://github.com/user-attachments/assets/0a63d844-0ad2-46d2-b519-2ce2749b6d17)
### Paso 9: Acceder a los sitios web
![image 6](https://github.com/user-attachments/assets/2bf8ed93-783e-40cb-87fa-3b4a8e25f453)

## 9. Resultados esperados
Se espera que, al ingresar en el navegador a las direcciones http://localhost:8089 y http://localhost:8090, se visualicen las páginas personalizadas correspondientes.

## 10. Bibliografía
Docker Inc. (2023). Docker Documentation. Recuperado de: https://docs.docker.com

Nginx. (2023). Nginx Documentation. Recuperado de: https://nginx.org/en/docs/

Chávez, M. (2021). Guía práctica de Docker y Nginx. Editorial Universitaria.

García, J. (2020). Comandos esenciales de Linux. OpenTech Press.





