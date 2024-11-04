
# Hive

Antes de empezar deberas clonar mi repositorio con el contenido necesario con los contenidos de docker para poder realizar los siguientes pasos
```bash
git clone https://github.com/meellaadoo04/Hive.git
```

1.Primero creamos el docker-compose y ejecutamos el cluster 

```bash
docker-compose up -docker
```

2. Ejecutamos el contenedor de hive para poder acceder a la bash de ese contenedor
```bash
docker exec -it docker-hive-hive-server-1 bash
````

3. En esa bash escribimos hive para poder acceder a sus servicios
```bash
hive
```

4. Ahora creamos una base de datos y la usamos
```bash
create database jugadores_futbol;
```

```bash
use jugadores_futbol
```

5. Creamos una tabla en la base de datos
```bash
CREATE TABLE jugadores (
    id INT,
    nombre STRING,
    equipo STRING,
    posicion STRING,
    edad INT,
    goles INT
)
```

6. Insertamos dentro de la tabla datos para poder realizar las consultas
```bash
INSERT INTO jugadores VALUES (1, 'Lionel Messi', 'Inter Miami', 'Delantero', 36, 800);
INSERT INTO jugadores VALUES (2, 'Cristiano Ronaldo', 'Al-Nassr', 'Delantero', 39, 850);
INSERT INTO jugadores VALUES (3, 'Neymar Jr', 'Al-Hilal', 'Delantero', 32, 400);
INSERT INTO jugadores VALUES (4, 'Kylian Mbappé', 'PSG', 'Delantero', 24, 250);
INSERT INTO jugadores VALUES (5, 'Kevin De Bruyne', 'Manchester City', 'Mediocampista', 32, 100);
```


7. Ahora ya podremos  realizar agunas consultas:

7.1 Ver todos los jugadores 
```bash
select * from jugadores
```

7.2 Contar el número total de jugadores
```bash
SELECT COUNT(*) AS total_jugadores FROM jugadores;
```

7.3 Filtrar jugadores que son delanteros
```bash
SELECT * FROM jugadores WHERE posicion = 'Delantero';
```

7.4 Filtrar jugadores mayores de 30 años
```bash
SELECT * FROM jugadores WHERE edad > 30;
```

7.5 Obtener jugadores ordenados por el número de goles (de mayor a menor)
```bash
SELECT * FROM jugadores ORDER BY goles DESC;
```
# PowerBi
# PowerBi
# PowerBi
# PowerBi
# PowerBi
# PowerBi
# PowerBi
# PowerBi
# PowerBi
# PowerBi
# PowerBi
# PowerBi
# PowerBi
