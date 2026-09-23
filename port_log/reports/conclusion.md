# Conclusión del análisis

El dataset heredado presentó problemas de calidad que requirieron descartar el 16.33% de los registros debido a inconsistencias insalvables. Entre los errores mas comunes detectados en el archivo de origen se encontraron fechas no válidas o corruptas, horas faltantes o con formatos erróneos, y lecturas nulas o anómalas en las mediciones de velocidad.

Al analizar los registros válidos de infracciones, se observa una marcada concenctración en los turnos Madrugada (135) y Tarde (127). En cuanto a la infraestructura portuaria, los puntos con mayor recurrencia fueron los Muelles B, C y D empatados con 83 infracciones cada uno. Respecto a la mercadería transportada, las infracciones se concentraron principalmente en buques con carga de trigo (74) y contenedores (69).

Incorporar esta información al nuevo sistema sin una etapa de depuración previa habría generado reportes y estadísticas completamente distorsionadas. Se habrían procesado operaciones sin marca temporal confiable, dificultand ola trazabilidad de los ingresos, y se podrían haber emitido penalizaciones erróneas a las embarcaciones a partir de sensores de velocidad defectuosos o lecturas incorrectas.

Para optimizar la captura de datos en el puerto, se propone implementar validaciones automáticas en el software de carga que impidan guardar campos con formatos de fecha y hora incompletos o fuera del rango establecido.