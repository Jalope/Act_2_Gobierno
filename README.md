# Gobierno del Dato y toma de Decisiones. UNIR 2025

Este repositorio contiene el desarrollo completo de la Actividad 2 de la asignatura de Gobierno del Dato. Para revisar el proyecto, se recomienda seguir los siguientes pasos:

1. **Informe**: Memoria\_Lopez\_Gismeros\_Javier.pdf
2. **Explorar la base de datos**: abre modelo\_estrella.db con DB Browser for SQLite (o similar) para ver la estructura en estrella y los datos.
3. **Consultas SQL**: revisa SQL\_query.txt para ver las seis consultas que arman los KPI del CMI.
4. **Levantamiento de Metabase y restauración del entorno**:

   * En terminal, sitúate en la carpeta del repositorio y ejecuta:

     ```
     docker-compose up -d
     ```
   * Restaura el backup del volumen (sustituye la ruta {PWD} por la que corresponda):

     ```
     docker run --rm -v metabase-cmi_metabase-data:/data -v "{PWD}:/backup" alpine tar xzf /backup/metabase-data.tar.gz -C /data
     ```
   * Abre tu navegador en [http://localhost:3001](http://localhost:3001)
   * Ve a la colección **ACT\_2**, donde encontrarás todas las preguntas y el dashboard **CMI\_ACT2** ya configurados.
5. **Vista previa del CMI**: consulta la imagen incluida más arriba para comprobar el resultado final.

Resultado final esperado: 
![image](https://github.com/user-attachments/assets/9b6cb3b2-706e-4da8-aabf-ceae3d236694)
