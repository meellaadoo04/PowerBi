# Power Bi con Hive

En esta guia vamos a conectar Hadoop + YARN + Hive + PowerBI

Para ello lo primero que debemos hacer es clonarnos el docker que contenga hive y ejecutarlo

```bash
git clone https://github.com/meellaadoo04/Hive.git
```

```bash
docker-compose up -d
```
![image](https://github.com/user-attachments/assets/9ba0ae8e-c065-48b4-bb29-c83a061f25a2)

Ahora deberemos instalar Power Bi desde la microsoft store y seguir los siguientes pasos para su configuración

1. Hacemos click en obtener datos de otros orígenes

2. En el menu izquierdo deberemos hacer click en otros y seleccionar Hive

3. Ahora te pedira tu servidor donde tendras que establecer el que hayas escogido en tu contenedor de hive que en este caso es "localhost:10000" y poner el nombre de la base da datos que quieras cargar en este caso "jugadores_futbol"

   Respecto al thrif deberemos seleccionar estandar y la conectividad de datos "importar"

4. En nombre de ususario y contraseña deberemos poner "root"

5. Ya podremos ver la tabla en Power Bi con nuestros datos cargados desde la base de datos de hive

6. En la derecha en datos desplegamos la tabla jugadores_futbol donde podremos ver un gráfico con los datos de nuestra nuestra tabla.

   
