# Trabajo Practico Integrador: Port Log - Sprint 3

## Integrantes
- **Grupo:** 22
- **Alumno:** Tomás Ezequiel Martínez
- **Repositorio:** https://github.com/tomas-e-martinez/Port_Log-Grupo_22.git

---

## Objetivo
Estructurar la informacion del puerto en una base de datos relacional mediante SQLAlchemy y sumar un sistema de busqueda por similitud visual con ChromaDB para identificar buques a partir de sus fotos.

---

## Introduccion y Contexto del Problema
A medida que el puerto escala en volumen de operaciones, el procesamiento basado en archivos CSV resulta insuficiente y la identificacion de buques únicamente por OCR genera fallas ante fotos nocturnas, borrosas o fuera de foco.

Para resolver estas limitaciones y profesionalizar la plataforma, en este sprint se abordan tres ejes principales:

1. **Persistencia relacional:** Migrar la informacion a una base de datos estructurada con un ORM (SQLAlchemy) que vincule buques, radares, registros de ingreso y evidencias fotográficas.
2. **Versionado de datos:** Implementar trazabilidad sobre los archivos y datasets del proyecto para garantizar el control sobre los cambios en los datos.
3. **Busqueda por similitud visual:** Incorporar una base de datos vectorial con ChromaDB y OpenCLIP para identificar embarcaciones mediante sus caracteristicas visuales completas, sirviendo de respaldo cuando la lectura de la patente por OCR resulta ilegible.