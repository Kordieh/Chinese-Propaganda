# Ficha técnica y diccionario de datos
### Fuente de los datos

Para armar esta base de datos se utilizó principalmente la información entregada por la [United Nations Trade and Development Data Hub](https://unctadstat.unctad.org/EN/About.html). En específico, la base de datos corresponde a las exportaciones e importaciones de bienes creativos.

### Metodología de la construcción de la base

La metodología utilizada para la construcción de la base de datos se basó en la recopilación y limpieza de diferentes tablas construidas con base a la información disponible de la [United Nations Trade and Development Data Hub](https://unctadstat.unctad.org/datacentre/dataviewer/US.CreativeGoodsValue).

Se utilizaron diversos filtros para ordenar la información y se seleccionaron ciertos países que, para efectos de este trabajo, son considerados los más importantes. En ese sentido, China representa el caso de estudio principal, junto con Corea del Sur y Japón al ser estas las mayores potencias culturales del Asia del este. Por su lado, la Unión Europea y Estados Unidos fueron seleccionados al ser las mayores hegemonías culturales occidentales, por lo cual representan los contrapesos naturales a las potencias asiáticas.

Se discriminaron los productos a únicamente aquellos del mundo audiovisual y literario, dejando de lado el relacionado con las manufacturas dado que se escapan del marco de análisis de este trabajo.

Una vez recopiladas todas las tablas de exportaciones e importaciones de las categorías seleccionadas, se procedió al armado de la base de datos, escogiendo específicamente las importaciones y exportaciones por parte de las potencias escogidas. Se decidió poner un foco especial en las exportaciones chinas al resto de potencias con el fin de descubrir en cuáles posee una presencia más fuerte y en especial cuándo comenzaron a aumentar las exportaciones culturales del gigante asiático.

### Alcance de los datos

Los datos aquí analizados corresponden a la información disponible y entregada por la United Nations Trade and Development Data Hub, específicamente entre los años 2002 y 2024, dado que corresponden a los datos más actualizados de los que dispone el organismo.

Si bien se intentó recurrir a otras fuentes como lo puede ser la UNESCO, los datos no se encontraban distribuidos de la misma manera, esto dado que la UNCTAD "encapsula" los datos de varias categorías en una sola (mezclando varios productos en una misma categoría difícil de desgranar de manera individual), por lo que se corría el riesgo de mezclar información errada en la base de datos, no porque fueran incorrectos, sino porque correspondían a cosas diferentes.
    
### Diccionario de datos 

Respecto al diccionario con las variables de la tabla, estos se encuentran divididos de la siguiente manera:
1. **País**: Representa cada nación analizada en este gráfico. Los países analizados son China, Japón, Estados Unidos, Reino Unido, República de Corea y la Unión Europea.
    * **Observación editorial**: Respecto al caso específico de **China**, la base de datos original proporcionada por [Naciones Unidas](https://unctadstat.unctad.org/datacentre/dataviewer/US.CreativeGoodsValue) divide al territorio chino en cuatro divisiones territoriales; "China" (continental), "China, Hong Kong SAR", "China, Macao SAR" y "China, Taiwan Province". Por motivos editoriales, los territorios fueron considerados como parte de la China continental **a excepción del territorio de Taiwán**. Si bien los territorios nombrados se encuentran en una situación política complicada, forman parte legalmente de la República Popular China, lo que no ocurre con Taiwán, la cual *de facto* se comporta y actúa como un país completamente independiente.
    * **Observación editorial 2**: Respecto a los países europeos se decidió analizarlos, para esta base de datos en específico y en concreto, como un conjunto de aquellos que se encuentren dentro de la Unión Europea dado que en ella se encuentran las mayores potencias europeas históricas de la industria (como lo pueden ser España, Francia, Alemania, Polonia, etc.). En ese sentido, se decidió incluir dentro del análisis también a Reino Unido, aunque no dentro del conjunto de la UE debido a que abandonó el "club europeo" en 2020.
2. **Producto**: Esta variable representa el tipo de producto analizado. Cada categoría fue colocada según la misma división que realiza la UNCTAD. Sobre qué productos se encuentran dentro de cada una, es recomendable visitar el documento que la misma organización [tiene disponible de manera pública.](https://unctad.org/system/files/official-document/ditctsce2024d1_en.pdf)
3. **Flujo**: Esta variable representa la dirección del intercambio monetario. Aquí existen dos valores posibles; exportación e importación.
4. **Destino**: Esta variable representa el lugar del cual provienen o se reciben las inversiones mostradas. Los datos representan los mismos países y territorios que se encuentran en el apartado de "País", sumado a la variable "Mundial", que representa el intercambio monetario con todos los países del mundo de los cuales la UNCTAD posee datos.
5. **(Año) Total en USD (Millones)**: Todas las variables que se encuentran categorizadas en este formato representan el total, en millones de dólares, del valor de las transacciones de un bien en concreto (descrito en la variable de "producto").