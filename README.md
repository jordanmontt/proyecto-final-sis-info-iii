# Este es el proyecto final de la materia Sis. Info. II

Por cuestiones de recursos, se utilizó solamente el 20% de los datos del datasert: imbd_dataser.csv

Contiene los siguientes archivos:
- **Proyecto Final.ipynb** Contiene toda la lógica para entrenar los diferentes modelos que se utilizó, además de guardar las métricas y los objetos en un archivo.
- **LimpiadorTexto.py** Esta clase contiene toda la lógica para limpiar un crítica en inglés.
- **ClasificadorAPI.py** Este es el servicio REST el cual recibe un crítica y devuelve la clasificación de dicha crítica.
- **ETL_de_clasificacion_de_nuevas_criticas.ktr** El ETL encargado de enviar varios request a la API y guardas las preddicciones en un archivo csv.
- **eliminar_comas_del_comentario.ktr** Este es un ETL que se utilizó en un principio para eliminar las cosas de todo el archivo del data_set. Luego, se percibió que no es necesario. Pero se dejó el archivo para mostrar el trabajo realizado.

Informe con los detalles de la implementación:
https://docs.google.com/document/d/1uKznKLKW5eSQ-hvTq_8U_Ronj_5kPp3XFktxTEYS0BU/edit
