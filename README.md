# Tarea B.D.Events

## 1. Obtener la edad promedio de los miembros
  - Sentencia:
  ```
  SELECT AVG(age) 
  AS edad_promedio 
  FROM members;
  ```
  - Captura:

<img width="500" alt="cap1" src="https://github.com/leon1611/tarea/assets/146900826/a8d65c2d-36ca-4aeb-9946-cc541f836c1d">

## 2. Obtener la edad mínima de los miembros
  - Sentencia:
  ```
  SELECT MIN(age) 
AS edad_minima 
FROM members;
  ```
  - Captura:
<img width="500" alt="Captura2" src="https://github.com/leon1611/tarea/assets/146900826/1e7841cf-cc81-454d-b29b-249e50e9b7ce">



## 3. Obtener el número total de registros asistidos
  - Sentencia:
  ```
  SELECT COUNT(*) 
AS total_registros_asistidos 
FROM register WHERE assisted = 'Yes';

  ```
  - Captura:
<img width="500" alt="Captura3" src="https://github.com/leon1611/tarea/assets/146900826/635b48a4-ae78-44ef-bd09-b25179b38470">

## 4. Obtener el número total de asistentes a todas las conferencias
  - Sentencia:
  ```
  SELECT COUNT(DISTINCT member_id)
 AS total_asistentes_conferencias 
FROM register;
  ```
  - Captura:
<img width="500" alt="Captura4" src="https://github.com/leon1611/tarea/assets/146900826/fe589ffd-002d-4d3d-acb5-454c9ace8d4f">



## 5. Obtener el número total de eventos por cada ciudad:
  - Sentencia:
  ```
  SELECT city,
COUNT(*) AS total_eventos 
FROM event 
GROUP BY city;

  ```
  - Captura:
<img width="500" alt="Captura5" src="https://github.com/leon1611/tarea/assets/146900826/63117df4-b5cb-4cca-aebd-b975be288c40">



## 6. Obtener el número de registros por cada miembro
  ```
  SELECT member_id,
 COUNT(*) AS total_registros 
FROM register 
GROUP BY member_id;

  ```
  - Captura:
<img width="500" alt="Captura6" src="https://github.com/leon1611/tarea/assets/146900826/5b51c718-1d4c-4105-bf3c-efb077d95499">



## 7. Obtener el número de registros por cada conferencia
  - Sentencia:
  ```
  SELECT conference_id, 
COUNT(*) AS total_registros 
FROM register
 GROUP BY conference_id;
  ```
  - Captura:
<img width="500" alt="Captura7" src="https://github.com/leon1611/tarea/assets/146900826/64567864-b703-42b1-bea5-dd7ec06baf8b">




