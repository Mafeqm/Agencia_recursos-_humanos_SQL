# Agencia de Recursos Humanos - Estandarización de Datos 🏢

Este proyecto contiene la solución al reto de estandarización y transformación de datos personales para los reportes internos de una agencia de recursos humanos, utilizando funciones nativas de SQL en MySQL.

## 📁 Estructura del Proyecto

El repositorio está organizado siguiendo las buenas prácticas de bases de datos, separando los scripts según su propósito:

*   **`ddl.sql` (Data Definition Language):** Contiene la creación de la base de datos `rrhh_agencia` y la estructura de la tabla `empleados` con sus respectivas restricciones de integridad.
*   **`dml.sql` (Data Manipulation Language):** Contiene la inserción de los 5 registros iniciales de los empleados con datos realistas para las pruebas.
*   **`dql.sql` (Data Query Language):** Contiene la consulta de transformación que genera el reporte utilizando las funciones de texto requeridas.

## 🛠️ Tecnologías Utilizadas

*   **Motor de Base de Datos:** MySQL Server
*   **Cliente GUI:** MySQL Workbench

## 📊 Transformaciones Aplicadas (DQL)

En el script de consulta se implementaron las siguientes funciones para el reporte final:

1.  **`CONCAT()`**: Combina el nombre y el apellido en una sola columna llamada `nombre_completo`.
2.  **`LENGTH()`**: Calcula la longitud total de caracteres de la cadena del nombre completo.
3.  **`UPPER()`**: Transforma el primer nombre del empleado a mayúsculas sostenidas.
4.  **`SUBSTRING_INDEX()`**: Extrae y aísla el dominio del correo electrónico (todo lo que se encuentra después del `@`).

## 🚀 Cómo Ejecutar el Proyecto

1. Clona este repositorio o descarga los archivos.
2. Abre tu cliente de **MySQL Workbench** y conéctate a tu servidor local.
3. Ejecuta los scripts en el siguiente orden estricto:
   1. `ddl.sql`
   2. `dml.sql`
   3. `dql.sql`
4. Revisa la pestaña de resultados en Workbench para visualizar el reporte formateado.
