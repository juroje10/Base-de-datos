## Práctica: Ejemplo básico de instalación y uso de un SGBDR ligero.

### 1. Sistemas de ficheros.

- Crea un fichero con la información de 5 mascotas.
- Analiza los problemas que pueden aparecer en la gestión de la información al trabajar con ficheros.

![text](Capturas/imagen_1.png)

### 2. Instalación de SQLite
   
En Windows -->

   1. Descarga SQLite desde la página oficial: https://www.sqlite.org/download.html
   2. Descarga el archivo sqlite-tools para Windows.

![text](Capturas/imagen_2.png)

   3. Descomprime la carpeta en C:\sqlite.

![text](Capturas/imagen_3.png)

   4. Abre la terminal CMD o PowerShell.
   5. Agrega la ruta C:\sqlite a las variables de entorno del sistema.

![text](Capturas/imagen_5.png)

Comprobar instalación:

![text](Capturas/imagen_4.png)


### 3. Creación de la base de datos

Abrir terminal y ejecutar; Aparecerá el prompt de SQLite.:

![text](Capturas/imagen_6.png)


### 4. Creación de tablas y Insercción de datos

```
CREATE TABLE mascotas (
id INTEGER PRIMARY KEY AUTOINCREMENT,
nombre TEXT NOT NULL,
especie TEXT NOT NULL,
edad INTEGER,
dueño TEXT
);
```

Comprobar que la tabla existe:

![text](Capturas/imagen_7.png)


### 5. Consultas básicas

Ver todos los registros, Ver solo los gatos; Contar cuántas mascotas hay:

![text](Capturas/imagen_8.png)


### 6. Actualización y eliminación
   
Actualizar la edad de "Luna"; Eliminar al pez "Nemo":

![text](Capturas/imagen_9.png)


### 7. Tareas
   
1. Inserta al menos 3 mascotas más de distintas especies.

![text](Capturas/imagen_10.png)


2. Crea una consulta que muestre solo los nombres y edades de los perros.

![text](Capturas/imagen_11.png)


3. Modifica la tabla para añadir un nuevo campo fecha_registro de tipo DATE.

![text](Capturas/imagen_12.png)


4. Inserta la fecha de registro en las nuevas mascotas.

![text](Capturas/imagen_13.png)


5. Elimina todas las mascotas con edad menor a 2 años.

![text](Capturas/imagen_14.png)





































