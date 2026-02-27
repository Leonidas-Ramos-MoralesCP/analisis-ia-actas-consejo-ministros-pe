# Actas de Consejo de Ministros durante el Gobierno de José Jerí (Colab + API ChatGTP)

Este proyecto presenta el resumen y análisis con IA de actas del Consejo de Ministros del Perú, conectando Google Colab con la API de ChatGPT. Se trabajó con actas del periodo del gobierno de José Jerí, halladas en el repositorio oficial del Perú. Se subieron doce archivos (uno por cada consejo) al entorno de Colab y, a partir de ellos, se solicitó al API de ChatGTP: un resumen de cada acta, sus palabras clave, un contexto noticioso asociado a lo que estaba ocurriendo en ese momento y un análisis de discrepancias entre los temas tratados en el Consejo de Ministros y dicho contexto de noticias. El producto final es un archivo Excel que se presenta como resultado del procesamiento.

# Problema
En la actualidad, la publicación de las actas del Consejo de Ministros constituye una obligación. Este es un espacio clave de toma de decisiones que reúne al presidente de la República, al presidente del Consejo de Ministros y a los ministros de Estado. Las sesiones se realizan con cierta regularidad —en algunos casos, de manera semanal—, aunque en circunstancias especiales su frecuencia puede aumentar o disminuir. Esta exigencia se establece desde 2023, cuando el Congreso aprobó que la convocatoria y/o agenda de las sesiones del Consejo de Ministros debe publicarse antes de su inicio, y que las actas que consignan los acuerdos deben difundirse en un plazo no mayor de 24 horas después de su aprobación.

En ese contexto, nos planteamos las siguientes preguntas para el gobierno de José Jeri: ¿qué temas se abordaron en estos consejos durante su gestión según estas actas y qué decisiones se adoptaron? ¿Qué eventos noticiosos generaron mayor discusión en el Perú durante ese periodo? ¿Y en qué medida existieron discrepancias entre lo tratado en esas sesiones y lo debatido en la agenda pública y mediática nacional? Para la ciencia política, resulta especialmente relevante analizar estas actas —disponibles desde 2023— para observar qué se discute, qué se decide y bajo qué circunstancias se adoptan determinadas decisiones. Este trabajo constituye un primer ejercicio en esa dirección.

# Proceso
1. Encontrar las actas: En la página oficial del Estado peruano se encontraron 12 PDF con las actas de los Consejos de Ministros. 

Aquí la página web: https://www.gob.pe/institucion/presidencia/colecciones/2226-actas-de-sesiones-del-consejo-de-ministros

Aquí los 12 PDF bajados y que luego fueron subidos al Google Colab: https://github.com/Leonidas-Ramos-MoralesCP/analisis-ia-actas-consejo-ministros-pe/blob/main/Actas%20Jer%C3%AD.zip 

2. Escribir el código en Google Colab y conectar al API de ChatGTP: 
Aquí encontrará el script utilizado en el Google Colab y su conexión al API: https://github.com/Leonidas-Ramos-MoralesCP/analisis-ia-actas-consejo-ministros-pe/blob/main/analisis_actas_jos_jeri_conectado_a_chatgtp.py   

Conviene recordar que el uso de la API requiere un pago a través de la plataforma de desarrolladores de ChatGPT. En este caso específico, se evidencia la rapidez con la que la IA realizó: 

(i) el ordenamiento cronológico de las fechas de las actas (columna fecha_acta).

(ii) el resumen de cada acta (columna temas_tocados). 

(iii) la identificación de palabras clave (columna palabras_clave). 

(iv) la búsqueda del entorno noticioso externo (columna contexto_noticioso_externo).

(v) el análisis de discrepancias entre lo consignado en el acta y el contexto noticioso (columna analisis_discrepancia). 

No obstante, queda pendiente evaluar sistemáticamente la calidad y consistencia de los resultados producidos.

# Resultados

Este es la muestra del resultado producido. En el link debajo podrá encontrar el análisis total. 

https://github.com/Leonidas-Ramos-MoralesCP/analisis-ia-actas-consejo-ministros-pe/blob/main/Resultado_Analisis_Jer%C3%AD_TextMining.xlsx 

<img width="1003" height="648" alt="image" src="https://github.com/user-attachments/assets/c6d05fae-1cc0-47e2-addd-f56dee0c5cef" />



