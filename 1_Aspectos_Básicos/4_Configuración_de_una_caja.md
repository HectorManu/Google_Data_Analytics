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



