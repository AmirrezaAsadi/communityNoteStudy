

# communityNoteStudy

Estudia notas de la comunidad utilizando análisis de datos con Python.

## Descripción general

Este repositorio contiene herramientas para analizar datos de Community Notes (anteriormente Twitter Birdwatch). Community Notes es un sistema colaborativo que permite a los usuarios agregar contexto a publicaciones que podrían ser engañosas.

## Archivos

- `community_notes_analysis.ipynb` - Cuaderno de Jupyter para cargar y analizar datos de Community Notes
- `notes-00000-2.tsv` - Conjunto de datos de ejemplo de Community Notes en formato TSV

## Uso

### Requisitos previos

Instala los paquetes de Python requeridos:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Ejecutar el análisis

1. Asegúrate de que el archivo `notes-00000-2.tsv` se encuentre en el directorio raíz del repositorio
2. Inicia Jupyter Notebook:

```bash
jupyter notebook community_notes_analysis.ipynb
```

3. Ejecuta todas las celdas para realizar el análisis completo

## Características del cuaderno

El cuaderno incluye:

- **Carga de datos**: Lee archivos TSV con pandas
- **Vista general de los datos**: Muestra la estructura del conjunto de datos, columnas y estadísticas básicas
- **Estadísticas descriptivas**: Resumen estadístico completo
- **Análisis de clasificación**: Distribución de las clasificaciones de las notas
- **Análisis temporal**: Tendencias basadas en el tiempo (si hay datos de marcas de tiempo disponibles)
- **Visualizaciones**: Múltiples gráficos que incluyen:
  - Distribuciones de clasificación
  - Patrones de datos faltantes
  - Distribuciones de características numéricas
  - Mapas de calor de correlación
- **Análisis de texto**: Conteo de palabras y análisis de contenido
- **Informe resumido**: Conclusiones y hallazgos clave

## Formato de datos

El archivo TSV debe contener datos de Community Notes con columnas como:
- `noteId`: Identificador único de la nota
- `tweetId`: ID del tweet asociado
- `classification`: Clasificación de la nota (p. ej., NOT_MISLEADING, MISINFORMED_OR_POTENTIALLY_MISLEADING)
- `createdAtMillis`: Marca de tiempo de creación en milisegundos
- `noteAuthorParticipantId`: Identificador del autor
- `summary`: Contenido de texto de la nota
- Columnas adicionales para calificaciones y metadatos

## Licencia

Este proyecto es con fines educativos y de investigación.
