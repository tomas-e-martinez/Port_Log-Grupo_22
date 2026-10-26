# Conclusión integradora

El sistema resuelve el control del puerto de punta a punta: primero limpia y corrige los datos corruptos de origen (como fechas mal cargadas o mediciones de velocidad nulas), vincula las fotos del barco a cada movimiento y guarda todo en una base relacional y otra vectorial para generar reportes y controlar las infracciones de manera automática.

La gran ventaja de sumar la base vectorial con OpenCLIP frente a usar solo OCR es que el OCR falla seguido si la foto de la patente sale borrosa, movida, de noche o desde muy lejos. En esos casos, la búsqueda vectorial sirve como un excelente respaldo, ya que puede reconocer al barco analizando la forma general de su estructura y silueta.

La principal limitación actual es que la busqueda por imagen solo funciona bien si le pasamos fotos de barcos completos (completes). Si intentamos buscar usando el recorte de una patente (plate), el modelo se confunde al comparar un texto chico con fotos de barcos enteros. Además, si un buque no tiene una foto clara en la base relacional, directamente no se puede incluir en la base vectorial.

Para poner este sistema a funcionar de verdad en el Puerto de Rosario, implementaría un flujo doble: que el sistema intente leer primero la patente con OCR y, si hay dudas o la foto es mala, use la búsqueda vectorial para confirmar de qué barco se trata. También agregaría controles en la carga de datos para bloquear de entrada los registros con fechas o velocidades erróneas, y pasaría la base vectorial a un servidor persistente para poder guardar fotos sin saturar la memoria.