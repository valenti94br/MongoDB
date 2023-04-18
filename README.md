# Investigación MONGODB 🔍



*¿Qué es MongoDB?*

MongoDB es un sistema de base de datos NoSQL, lo que significa que no utiliza la estructura de tabla de una base de datos relacional tradicional. En lugar de ello, MongoDB almacena los datos en documentos JSON (JavaScript Object Notation). Cada documento es una entidad independiente y contiene su propio conjunto de atributos y valores.

* * *

*¿Cuáles son las características principales de MongoDB?*

Las características principales de MongoDB incluyen:

**Escalabilidad tanto horizontal como vertical:** MongoDB se puede escalar fácilmente añadiendo más nodos a la red, lo que permite manejar grandes volúmenes de datos. El escalado vertical funciona agregando más potencia a una máquina existente, mientras que el escalado horizontal funciona agregando más máquinas a los recursos de un usuario.

**Alta disponibilidad:** MongoDB utiliza replicación automática para mantener varias copias de los datos en diferentes nodos, lo que permite una alta disponibilidad y recuperación ante fallos.

**Flexibilidad en la estructura de datos:** MongoDB no requiere un esquema predefinido, lo que permite añadir campos o cambiar la estructura de los documentos sin necesidad de modificar el esquema de la base de datos.

**Soporte para consultas avanzadas:** MongoDB ofrece una variedad de operadores para consultas avanzadas, incluyendo consultas geoespaciales y consultas de texto completo.

**Compatibilidad con la nube:** MongoDB tiene soporte incorporado para entornos en la nube, con integraciones para los principales proveedores de la nube como AWS, Azure y Google Cloud Platform.

* * *

*¿Cómo se estructuran los datos en MongoDB?*

En MongoDB, los datos se organizan en **colecciones**, que son similares a las tablas en una base de datos relacional. Cada colección contiene **documentos**, que son los registros individuales. Los documentos se componen de **pares clave-valor**, la unidad básica de datos de MongoDB. Los documentos son similares a la notación de objetos de JavaScript (JSON), pero usan una variante llamada **Binary JSON (BSON)**. El beneficio de usar BSON es que admite más tipos de datos.



| MongoDB (NoSQL Database)  | RDBMS (SQL Server, Oracle, etc.)  |
|---------------------------|-----------------------------------|
| Database                  | Database                          |
| Collection                | Table                             |
| Document                  | Row (Record)                      |
| Field                     | Column                            |

* * *

*¿Qué ventajas ofrece MongoDB en comparación con las bases de datos relacionales?*

MongoDB ofrece varias ventajas sobre las bases de datos relacionales tradicionales, incluyendo:

**Flexibilidad en la estructura de los datos:** MongoDB puede manejar una variedad de estructuras y tipos de datos sin necesidad de esquemas estrictos. Esto puede ser particularmente útil para manejar datos no estructurados o semiestructurados.

**Escalabilidad:** Gracias a su escalabilidad horizontal y vertical, el rendimiento de MongoDB es mucho mayor que el de cualquier base de datos relacional.

**Alto rendimiento:** MongoDB utiliza indexación y consultas optimizadas para ofrecer un alto rendimiento en la recuperación de datos.

**Lenguaje de consultas simple:** El lenguaje de consulta de documentos admitido por MongoDB es muy simple en comparación con las consultas SQL. Tampoco se necesitan uniones complejas en MongoDB. No hay relación entre los datos en MongoDB.

**Orientado a documentos:** Una de las ventajas de usar documentos es que los objetos se asignan a tipos de datos nativos en varios lenguajes de programación.

* * *

*¿Cuáles son las desventajas de MongoDB? ¿Cuándo no es recomendable utilizarlo?*

MongoDB también tiene algunas desventajas y situaciones en las que no es recomendable utilizarlo:

**No es adecuado para aplicaciones que requieren transacciones complejas y relacionales**.
* MongoDB no proporciona integridad referencial completa mediante el uso de restricciones de *foreign keys*, lo que podría afectar la coherencia de los datos. Sus operaciones *join* son limitadas. Esto puede dificultar el modelado de relaciones complejas entre datos.
* MongoDB no tiene soporte de transacciones. El soporte de transacciones significa que todas las operaciones se completan con éxito, o ninguna de ellas, para mantener la integridad de los datos. Si una operación falla en medio de una secuencia de operaciones relacionadas, no hay garantía de que los datos se mantengan en un estado coherente.


**No es tan maduro ni tan seguro** como las bases de datos relacionales tradicionales en términos de herramientas y características. Si bien MongoDB proporciona funciones de seguridad básicas como autenticación y autorización, no llegan al nivel de los RDBMS tradicionales.

**Uso de memoria alto:** MongoDB usa mucha memoria para el almacenamiento de datos.

* * *

*¿Cómo se instala y configura MongoDB? ¿Cuáles son los requisitos mínimos de hardware y software?*

Para instalar MongoDB, se necesita un sistema operativo compatible, como Windows, Linux o Mac OS X. MongoDB se puede descargar desde el sitio web oficial y se instala mediante un archivo de instalación. Los requisitos mínimos de hardware y software dependerán del tamaño de la base de datos y la cantidad de tráfico que se espera manejar. En general, MongoDB puede ser ejecutado en una máquina con un procesador de 64 bits y 4 GB de RAM o más.