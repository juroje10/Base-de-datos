## Unidad 1: Introducción a las Bases de Datos


#### 1. Define las funciones del administrador de la base de datos.

El administrador (DBA) gestiona, mantiene y asegura la base de datos. Controla los accesos, realiza copias de seguridad, optimiza el rendimiento y garantiza la integridad de los datos.

---

#### 2. Indica las diferencias existentes entre las funciones de manipulación y de descripción.

Las funciones de manipulación permiten consultar, insertar, modificar o borrar datos. Las de descripción definen la estructura de la base, como tablas o relaciones.

---

#### 3. ¿Qué tipos de usuarios interaccionan con una base de datos?

Existen administradores, diseñadores y usuarios finales, cada uno con distintos niveles de acceso y responsabilidades.

---

#### 4. Indica qué es un lenguaje huésped y un lenguaje anfitrión.

El lenguaje huésped es el del programa principal (como C o Java), mientras que el anfitrión es el lenguaje de base de datos (como SQL) que se integra en el huésped para manejar los datos.

---

#### 5. La gestión del espacio de almacenamiento, ¿a qué nivel de la arquitectura ANSI/SPARC pertenece? ¿Qué es la arquitectura ANSI/SPARC?

Pertenece al **nivel interno**.  
La arquitectura ANSI/SPARC define tres niveles (interno, conceptual y externo) que separan el almacenamiento físico, la estructura lógica y las vistas de los usuarios.

---

#### 6. Dibuja un diagrama de la arquitectura de sistemas de bases de datos (ANSI/SPARC).

- **Nivel interno:** almacenamiento físico de los datos.  
- **Nivel conceptual:** estructura lógica de la base.  
- **Nivel externo:** vistas personalizadas para los usuarios.

---

#### 7. Indica las principales funciones realizadas por el SGBD.

Control de acceso, gestión del almacenamiento, manipulación de datos, recuperación ante fallos y mantenimiento de la integridad.

---

#### 8. Explica la diferencia entre la independencia física y lógica de los datos.

La independencia física permite cambiar el almacenamiento sin afectar a los programas.  
La independencia lógica permite modificar la estructura de datos sin afectar a las aplicaciones.

---

#### 9. ¿Qué es el diccionario de datos?

Repositorio que guarda información sobre la estructura, restricciones y relaciones de la base de datos.

---

#### 10. Diferencias entre el LDD y LMD de un sistema gestor de base de datos.

El **LDD** define la estructura (tablas, campos, relaciones).  
El **LMD** manipula los datos (consultar, insertar, borrar, actualizar).

---

#### 11. Indica los componentes principales de un sistema gestor de base de datos.

Hardware, software, datos, usuarios y procedimientos.

---

#### 12. ¿Qué es un modelo de datos?

Representación abstracta que describe cómo se organizan y relacionan los datos.

---

#### 13. ¿Qué son los lenguajes de cuarta generación? Pon ejemplos.

Lenguajes orientados a simplificar el trabajo con bases de datos, como **SQL**, **Access** o **PowerBuilder**.

---

#### 14. Indica las principales ventajas de un sistema de bases de datos. ¿Existen algunas desventajas?

**Ventajas:** reducción de redundancia, integridad, seguridad y facilidad para compartir datos.  
**Desventajas:** mayor complejidad y consumo de recursos.

---

#### 15. Dado el siguiente listado, clasifica cada elemento según corresponda a sistemas de ficheros o sistemas de bases de datos:

| Elemento | Clasificación |
|-----------|----------------|
| Archivos CSV | Sistema de ficheros |
| Oracle Database | Sistema de base de datos |
| MongoDB (JSON) | Sistema de base de datos |
| MySQL | Sistema de base de datos |
| Archivos de texto plano | Sistema de ficheros |

---

#### 16. Relaciona cada tipo de base de datos con su descripción correspondiente:

| Tipo | Descripción |
|------|--------------|
| Relacional | Organiza datos en tablas con relaciones |
| Documental | Usa documentos flexibles (JSON/BSON) |
| Grafos | Representa nodos y relaciones |
| Clave-valorD | Almacena pares clave-valor, ideal para cachés |

---

#### 17. Describe brevemente las principales diferencias entre bases de datos centralizadas y distribuidas, mencionando dos ventajas y dos desventajas de cada una.

- **Centralizadas:** un solo servidor.  
  - Ventajas: control y mantenimiento sencillos.  
  - Desventajas: punto único de fallo, menor rendimiento con muchos usuarios.  
- **Distribuidas:** datos repartidos en varios nodos.  
  - Ventajas: mayor disponibilidad y escalabilidad.  
  - Desventajas: más complejas y difíciles de sincronizar.

---

#### 18. Enumera cinco funciones principales de un Sistema Gestor de Bases de Datos y explique brevemente en qué consiste cada una.

1. **Definición de datos:** crear estructuras.  
2. **Manipulación:** consultar y modificar datos.  
3. **Control de seguridad:** gestionar accesos.  
4. **Recuperación:** restaurar datos tras fallos.  
5. **Optimización:** mejorar el rendimiento.

---

#### 19. Clasifica los siguientes SGBD según su tipo (relacional, documental, clave-valor, grafos) y su licencia (open source, comercial):

| SGBD | Tipo | Licencia |
|------|------|----------|
| MySQL | Relacional | Open source |
| Oracle Database | Relacional | Comercial |
| MongoDB | Documental | Open source |
| Redis | Clave-valor | Open source |
| PostgreSQL | Relacional | Open source |
| Neo4j | Grafos | Comercial (con versión libre limitada) |

---

#### 20. Analiza un caso práctico donde sería recomendable utilizar una base de datos distribuida en lugar de una centralizada, justificando su respuesta con al menos tres argumentos basados en las ventajas de este tipo de bases de datos.

En una empresa con sedes en distintos países, una base de datos distribuida es ideal porque ofrece mayor disponibilidad, acceso más rápido desde cada región y tolerancia a fallos si un nodo deja de funcionar.

---

#### 21. Explica el Teorema CAP y cómo afecta a las bases de datos distribuidas, describiendo qué significan cada una de sus letras y qué dos propiedades suelen elegir la mayoría de sistemas distribuidos modernos.

El teorema CAP afirma que un sistema distribuido no puede garantizar al mismo tiempo **Consistencia (C)**, **Disponibilidad (A)** y **Tolerancia a particiones (P)**.  
La mayoría de sistemas modernos priorizan **A** y **P**, sacrificando algo de consistencia para ganar rendimiento y disponibilidad.

---

#### 23. Completa la siguiente tabla comparativa: 

| Característica              | Sistema de Ficheros                                       | Sistema de Bases de Datos                                        |
|-------------------------------|---------------------------------------------------------|------------------------------------------------------------------|
| **Redundancia de datos**       | Alta: los mismos datos suelen repetirse en varios archivos.                         | Baja: los datos se centralizan y se evita duplicación innecesaria.              |
| **Control de concurrencia**    | Limitado o inexistente: varios usuarios pueden sobrescribir información.           | Sí: el SGBD gestiona accesos concurrentes para evitar conflictos.               |
| **Independencia de datos**     | Baja: cambios en la estructura de archivos afectan a los programas que los usan.  | Alta: se pueden modificar la estructura lógica o física sin afectar a las aplicaciones. |
| **Seguridad**                  | Básica: se limita al control de acceso al sistema de archivos.                     | Alta: el SGBD controla accesos, permisos y protege los datos frente a usuarios no autorizados. |
