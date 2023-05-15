# Los pormenores de las herramientas de datos centrales


- Atributo es el encabeczado que va a describir una caracterísitca o propiedad de datos.
- Formula es una acción especifica que se realiza en un conjunto de celdas


1. En una tabla, un atributo es una característica o calidad de los datos que se usan con el siguiente fin:
   - Etiquetar una columna
     - Correcto
       - En una tabla, un atributo es una característica o calidad de los datos usados para etiquetar una columna.


2. En una hoja de cálculo, ¿para qué se usa el ajuste de texto?
- Para cambiar automáticamente la altura de la cenda a fin de que entre todo el texto
  - Correcto
    - Es una hoja de cálculo, el ajuste de texto se utiliza para cambiar automáticamente la altura de la celda a fin de que entre todo el texto.

3. Las columnas de una hoja de cálculo se ordenan por letra y las filas se ordenan por número.
   - Verdadero
     - Es una hoja de cálculo, las columnas se ordenan por letra y las filas se ordenan por número.

4.  Completa el espacio en blanco: En una tabla de datos, una fila se denomina observación. Una observación incluye todos los _____ de lo contenido en la fila.
   - Atributos
     - Correcto
       - Es una tabla de datos, una fila se denomina observación. Una observación incluye todos los atributos de lo contenido en la fila. Un atributo es una cualidad o característica de los datos.



# SQL en acción
- Store 
- Organize
- Analyze
 
 - Query
   - Es una solicitud de datos o información de la base de datos.

## ¿Qué es una consulta?
La sintaxis de cada consulta SQL es la misma: 

- Usa SELECT para elegir las columnas que deseas devolver.

- Usa FROM para elegir las tablas donde se encuentran las columnas que deseas.

- Usa WHERE para filtrar determinada información.

```SQL
SELECT first_name
FROM customer_data.customer_name
WHERE first_name = 'Tony';
```
La consulta anterior usa tres comandos para localizar clientes que se llaman Tony:

1. **ELEGIR (SELECT)** la columna denominada nombre (first_name)

2. **DESDE (FROM)** una tabla denominada **nombre_del_cliente (customer_data)** (en un conjunto de datos denominado **nombre_del_cliente [customer_data]**) (el nombre del conjunto de datos siempre va seguido de un punto y, a continuación, del nombre de la tabla).

3. Pero solo se devuelven los datos **DONDE (WHERE)** el primer_nombre (first_name) es Tony


### arias columnas en una consulta.

```SQL
SELECT customer_id, first_name, last_name
FROM customer_data.customer_name
WHERE first_name = 'Tony';
```

La consulta anterior usa tres comandos para localizar clientes que se llaman Tony:

1. **ELEGIR (SELECT)** las columnas denominadas **id_del_cliente (customer_id)**, **nombre (first_name)** y **apellido (last_name)**

2. **DESDE (FROM)** una tabla denominada **nombre_del_cliente (customer_data)** (en un conjunto de datos denominado **nombre_del_cliente [customer_data]**) (el nombre del conjunto de datos siempre va seguido de un punto y, a continuación, del nombre de la tabla)3. Pero solo se devuelven los datos DONDE (WHERE) el nombre (first_name) es Tony”

 3. Pero solo se devuelven los datos **DONDE (WHERE)** el nombre (first_name) es **Tony**



```SQL
SELECT customer_id, first_name, last_name
FROM customer_data.customer_name
WHERE customer_id > 0 AND first_name = 'Tony' AND last_name = 'Magnolia';
```

La consulta anterior usa tres comandos para localizar clientes con un ID de cliente válido (mayor que 0) cuyo nombre es Tony, y su apellido es Magnolia.

1. **ELEGIR (SELECT)** las columnas denominadas **id_del_cliente (customer_id)**, **nombre (first_name)** y **apellido (last_name)**

2. **DESDE (FROM)** una tabla denominada **nombre_del_cliente (customer_data)** (en un conjunto de datos denominado **nombre_del_cliente [customer_data]**) (el nombre del conjunto de datos siempre va seguido de un punto y, a continuación, del nombre de la tabla).

3. Pero solo devuelve los datos **DONDE (WHERE)** el ID_del_cliente (customer_id) es mayor que **0**, el **nombre (first_name)** es **Tony** y el apellido (last_name) es **Magnolia**.

### Conclusión clave
Lo más importante es recordar cómo usar SELECT, FROM y WHERE en una consulta. Una vez que hayas practicado cómo escribir tus propias consultas SQL más adelante en el programa, las consultas con varios campos serán más sencillas.


#  Angie: La lucha cotidiana al aprender nuvas habilidades 

# Las posibilidades de SQL con infinitas

```SQL
SELECT field1
FROM table
WHERE field1 = condition;
```
## Condición WHERE

En la consulta que se mostró anteriormente, la cláusula SELECT identifica la columna de la cual deseas extraer datos por nombre, field1, y la cláusula FROM identifica la tabla donde se encuentra la columna por nombre, table. Por último, la cláusula WHERE restringe la consulta para que la base de datos devuelva solo los datos con una coincidencia de valor exacta, o los datos que coincidan con una determinada condición que deseas satisfacer. 

Por ejemplo, si estás buscando a un cliente específico con el apellido Chavez, la cláusula WHERE sería: 

**WHERE field1 = 'Chavez'**

Sin embargo, si estás buscando a todos los clientes que tienen un apellido que empieza con las letras “Ch”, la cláusula WHERE sería:

**WHERE field1 LIKE 'Ch%'**

En conclusión, la cláusula LIKE es muy poderosa porque te permite decirle a la base de datos que busque un patrón determinado. El signo de porcentaje (%) se usa como comodín para que coincida con uno o más caracteres. En el ejemplo anterior, se devolverían tanto Chávez como Chen. Ten en cuenta que en algunas bases de datos se usa un asterisco (*) como comodín en lugar de un signo de porcentaje (%).


### Pon a prueba ts conocimeentos sobre SQL 

- ¿Cuáles son algunas de las razones por las cuales un analista de datos podría usar visualizaciones de datos ? 
  - Reforzar el análisis de datos
    - Correcto:
      - Los analistas de datos usan visulizaciones de datos para explicar datos complejos rápidamente, deforzar el análisis de datos y crear diagramas graficos.
  - Explicar datos complejos rápidamente
  - Crear gráficos interesantes


# Pon a prueba tus conocmientos sobre la visualizaión de datos

1. Pregunta 1
Completa el espacio en blanco: Una visualización de datos es la representación _____ de la información.
- Gráfica 
  - Correcto 
    - Una visualización de daots es la repsretación gráfica de la información 


2. ¿Cuándo un gráfico circular sería una visualización efectiva?

-  Al mostrar una lase desgoosada por edad
   -  Un gráfico circular muestra cómo un todo se divide en partes y es una visualización efectiva para una clase desglosada por edad.


3. Pregunta 3
¿Cuáles son los beneficios clave de las visualizaciones de datos? Selecciona todas las opciones correctas.

- Pueden ilustrar las relaciones entre los puntos de dato s
- Pueden demostar claramente patrones y tendencias 
- Pueden ayudar a los interesasados a comprender los datos complejs y más rápidamente 

--  Correcto 
  Las visualizaciones de datos pueden demostrar claramente patrones y tendencias, ayudar a los interesados a comprender los datos complejos más rápidamente e ilustrar las relaciones entre los puntos de datos.





# Desafío semana 4

1. Pregunta 1
En la fila 1 de la siguiente hoja de cálculo, ¿cómo se denominan las palabras rango, nombre, población y condado? 

- Caracterísitcas incorrecto
-

2. En la siguiente hoja de cálculo, la observación de Greensboro describe todos los datos de la fila 4.

- Verdadero 
  - Correcto
    - La observación de Greenboro describee todos

3. Completa el espacio en blanco: En la siguiente hoja de cálculo, la función _____ se utilizó para ordenar alfabéticamente los nombres de las ciudades de la columna B.

- Rango de clasificación

4. Un analista de datos escribe =POPULATION(C2:C11) para encontrar la población promedio de las ciudades en esta hoja de cálculo. Sin embargo, se dan cuenta de que usaron la fórmula equivocada. ¿Qué sintaxis corregirá esta función?

- La sintaxis correcta para la función AVERAGE es la siguiente: =AVERAGE(C2:C11).Cuando usas la función AVERAGE, obtienes el promedio de los valores incluidos en un rango seleccionado. C2:C11 es el rango especificado.

5. Estás trabajando con una tabla (base de datos) denominada genre que contiene datos sobre géneros musicales. Quieres revisar todas las columnas de la tabla.

Escribes la consulta en SQL a continuación. Agrega una cláusula FROM que recupere los datos de la tabla genre.

- La cláusula FROM genre recuperará los datos de la tabla genre. La consulta completa es SELECT * FROM genre. La cláusula FROM especifica qué tabla de la base de datos hay que consultar. El género del álbum con número de ID 3 es Metal.

6. Pregunta 6
Estás trabajando con una tabla de una base de datos que contiene datos de facturas. La columna customer_id enumera el número de ID de cada cliente. Te interesan los datos de facturación del cliente con el número de ID 54.

Escribes la consulta en SQL a continuación. Agrega una cláusula WHERE que te muestre solo los datos sobre el álbum con número de ID 54.

- La cláusula WHERE customer_id = 54 solo te mostrará los datos del cliente con el número de ID 54. La consulta completa es SELECT * FROM invoice WHERE customer_id = 54. La cláusula WHERE filtra los resultados que cumplen con ciertas condiciones. La cláusula WHERE incluye el nombre de la columna, un signo de igual y el valor o los valores a incluir en la columna. La dirección de facturación del cliente con el número de ID 54 es 110 Raeburn Pl. 

7. Un analista de datos crea la siguiente visualización para demostrar claramente cuánto más poblada es Charlotte que la siguiente ciudad más grande de Carolina del Norte, Raleigh. ¿Qué tipo de gráfico es?

- El gráfico es un gráfico de columnas. Un gráfico de columnas es eficaz para demostrar las diferencias entre varios elementos de un rango de valores específico. 

8. Un analista de datos quiere demostrar cómo aumentó la población de Charlotte con el tiempo. Crean el gráfico que aparece a continuación. ¿Cómo se llama este tipo de gráfico?

- Correcto
Se trata de un gráfico de líneas. Los gráficos de líneas son eficaces para demostrar tendencias y patrones, por ejemplo, cómo cambia la población a lo largo del tiempo.
