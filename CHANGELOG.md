[Ejercicio 5]
- Creación y población de la base de datos transito_portuario.

[Ejercicio 4]
- Implementación del modelo definido en el diagrama.
- Definición de la función procesar_fila_csv(row: dict) -> Movimiento.

[Ejercicio 3]
- Creación de diagrama entidad-relación para modelado de base de datos.

[Ejercicio 2]
- Migración a DVC de imágenes
- Migración a DVC de gráficos
- Migración a DVC de dataset procesado

[Ejercicio 1]
- Clonación del repositorio remoto.
- Creación de rama 'Sprint_3'

[Ejercicio 6]
- Redacción y guardado de la conclusión del trabajo.

[Ejercicio 5]
- Análisis de los datos obtenidos en el paso previo.

[Ejercicio 4]
- Cruzar matrículas extraídas de imagenes con dataset de infracciones
- Guardar columnas nuevas con datos del cruce de datos y matrícula extraída

[Ejercicio 3]
- Convertir imágenes originales a escala de grises y guardar
- Aplicar ecualización de histograma y guardar imágenes
- Aplicar blur gaussiano y guardar imágenes
- Aplicar Canny (detección de bordes) y guardar imágenes

[Ejercicio 2]
- Construir el diccionario group_images con 'plates' y 'completes'
- Definición de función mostrar_muestra

[Ejercicio 1]
- Clonación del repositorio remoto.
- Creación de rama 'Sprint_2'
- Descarga y unzip de imágenes

[Ejercicio 7]
- Redacción y guardado de la conclusión del trabajo.

[Ejercicio 6]
- Cálculo y análisis de datos varios sin modificación de los archivos.

[Ejercicio 5]
- Creación y guardado Gráfico de barras: Top 10 matrículas más reincidentes
- Creación y guardado Gráfico de torta: Total de infracciones por turno
- Creación y guardado Gráfico de barras: Total de infracciones por mes
- Creación y guardado Histograma de exceso de velocidad real
- Creación y guardado Gráfico de barras: Exceso de velocidad promedio por muelle
- Creación y guardado Gráfico de barras: Infracciones con fecha válida vs fecha inválida

[Ejercicio 4]
- Creación de la clase PortAnalyzer
- Creación de método top_infractores(n: int) -> pd.DataFrame
- Creación de método infracciones_por_turno() -> pd.DataFrame
- Creación de método exceso_promedio() -> float
- Creación de método exceso_promedio_tolerancia() -> float
- Creación de método infracciones_por_muelle() -> pd.DataFrame
- Creación de método infractores_por_tipo_carga() -> pd.DataFrame

[Ejercicio 3]
- Normalización de fechas de ingreso y egreso al formato YYYY-MM-DD. Las fechas inválidas se completaron con 1900-01-01.
- Normalización de horas con el formato de 24hs. Las horas inválidas se completaron con 00:00.
- Calculo y adición de la columna duracion_horas.
- Normalización de matrículas.
- Normalización de muelles.
- Eliminación de registros con valores nulos en columnas consideradas críticas.
- Eliminación de outliers en tonelaje_declarado y velocidad_ingreso utilizando IQR.
- Cálculo y creación de la columna exceso_velocidad_real
- Cálculo y creación de la columna exceso_velocidad
- Eliminación de registros sin infracción
- Guardado de dataset limpio en interim
- Exportación de resumen estadístico rápido de pandas

[Ejercicio 2]
- Descarga del dataset raw.

[Ejercicio 1]
- Clonación del repositorio remoto.
- Configuración del usuario de git.
- Creación de rama 'Sprint_1'
- Creación de estructura de carpetas

