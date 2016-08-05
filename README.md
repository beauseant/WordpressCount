# WordpressCount
Notebook en PySpark para contar apariciones de palabras en los posts de una base de datos Wordpress

Es necesario descargar la base de datos a un formato CSV:

SELECT * FROM wp_posts INTO OUTFILE "/tmp/wp_posts5.sql" FIELDS TERMINATED BY ';' ENCLOSED BY '"' LINES TERMINATED BY '\n';

El notebook procesa ese fichero para generar estadísticas con las palabras, limpiando las stopwords y filtrando por año.
