# Este es el proyecto final de la materia Sis. Info. III

Por cuestiones de recursos, se utilizó solamente el 20% de los datos del dataset: *imbd_dataser.csv*

Contiene los siguientes archivos:
- **Proyecto Final.ipynb** Contiene toda la lógica para entrenar los diferentes modelos que se utilizó, además de guardar las métricas y los objetos en un archivo.
- **LimpiadorTexto.py** Esta clase contiene toda la lógica para limpiar un crítica en inglés.
- **ClasificadorAPI.py** Este es el servicio REST el cual recibe un crítica y devuelve la clasificación de dicha crítica.
- **ETL_de_clasificacion_de_nuevas_criticas.ktr** El ETL encargado de enviar varios request a la API y guardas las preddicciones en un archivo csv.
- **eliminar_comas_del_comentario.ktr** Este es un ETL que se utilizó en un principio para eliminar las comas de todo el archivo del *dataset*. Luego, se percibió que no es necesario. Pero se dejó el archivo para mostrar el trabajo realizado.

[Informe con los detalles de la implementación](https://docs.google.com/document/d/1uKznKLKW5eSQ-hvTq_8U_Ronj_5kPp3XFktxTEYS0BU/edit)

**Para hacer funcionar el ETL y la API Rest con el clasificador entrenado, ejecutar los siguientes pasos:**

1. Ejecuta la consola de Anaconda en la dirección donde se descargo este proyecto.
2. Ejecute el siguiente comando: 

	python ClasificadorAPI.py

    
    Si todo está bien, verás en la consola de anaconda el siguiente mensaje: * Running on http://127.0.0.1:8080/ (Press CTRL+C to quit)

3. Luego, abra el archivo ETL_de_clasificacion_de_nuevas_criticas.ktr con Pentaho(nosotros utilizamos la versión 8.3).
4. Ahora simplemente, ejecute el transformador y listo.
