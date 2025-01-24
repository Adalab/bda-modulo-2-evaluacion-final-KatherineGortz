# bda-modulo-2-evaluacion-final-KatherineGortz
bda-modulo-2-evaluacion-final-KatherineGortz created by GitHub Classroom

Para la evaluación final de Módulo 2: SQL, he seguido los siguientes pasos:
- Recepción del enunciado el 23 de enero
- Revisión del anunciado para apuntar dudas a alcarar en el soporte técnico el 24 de enero (8:30-14:00h)
- Realización de las consultas dentro de la base de datos, Sakila, que se instaló al príncipio del Módulo 2
- Conversar con Yanelis para resolver dudas
- Creación del repo, entrega del fichero SQL ya completado

Anotaciones sobre aspectos técnicos de las consultas: 
1. Dentro de la tabla film
2. Dentro de la tabla film, con una condición en la cláusula WHERE
3. Dentro de la tabla film, con una condición en la cláusula WHERE, tener en cuenta que %amazing% incluiría cualquier string que incluya esa palabra, como 'amazingly', por tanto no busca estrictamente la palabra 'amazing'
4. Dentro de la tabla film, con una condición en la cláusula WHERE, 120 excluido
5. Dentro de la tabla actor, se incluye apellido además de nobmre, y ORDER BY apellido para mejorar la consulta y su posterior visualización.
6. Dentro de la tabla actor, con una condición en la cláusla WHERE, %gibson% tiene la misma limitación explicada en 3.
7. Dentro de la tabla actor, BETWEEN es inclusive, se interpretó que había que incliuir el ID 10 y 20
8. Dentro de la tabla film, con cláusa WHERE con una exclusión: NOT IN
9. Dentro de la tabla film, con función agregada COUNT, es necesario incluir un GROUP BY con COUNT
10. Había que hacer JOIN con rental y customer para poder incluir nombre y apellido. Uso de INNER JOIN para buscar solo registros que coinciden, GROUP BY id_cliente para mostar el número correspondiente de alquileres.
11. JOINS para unir category y rental, en cada paso incluir el campo que coincida en el ON, usar función agregada COUNT para sumar las veces que el id_inventario de cada peli apareciá en la tabla de rental
12. Dentro de la tabla film, con función agregada de calcular promedio (AVG), es necesario usar un GROUP BY
13. Hbaía que unir la tabla actor con la tabla film, luego poner la condicion WHERE el titulo de la pelicula que queríamos saber los actores
14. Dentro de la tabla film, con la mimsa limitación explicada en consulta 3.
15. JOIN actor con film_actor con LEFT JOIN para que pudieran aparecer valores NULOS, es lo que buscamos aqui, pero no había.
16. Dentro de la tabla film, BETWEEN es inclusive de los años 2005 y 2010.
17. JOINS para unir la tabla film y category, condición WHERE con el nombre de la category que queremos filtar
18. y 21. La mimsa consulta con un HAVING distinto, aunque da el mismo resultado. INNER JOIN actor y film actor para solo incluir coincidencias, función agregada COUNT para sumar número de pelis en las que sale cada actor. Filtro en HAVING.
19. Dentro de la tabla film, con dos condiciones en la cláusula WHERE
20. Unir tablas category y film. Usar función agregarada para calcular el promedio de duración con su correspondiente GROUP BY, y filtrar por 120 minutos en la cláusla HAVING.
22. Primero realizar subconsulta para identificar los rental_id con una duración de mas de 5 días usando función DATEDIFF, que toma 2 fechas y hace la resta. Luego en la consulta principal había que unir film con rental, y en la cláusula WHERE buscar rental_id que cumplan la condicion en el subquery.
23. En el subquery, unir tablas actor y category. Usar a2 para no confundir con la tabla actor en la query principal. Usar NOT IN con el subquery para excluir registros que cumplen con la condición de salir en una película horror.
24. Unir tablas film y category, poner dos condiciones en la cláusula WHERE.
