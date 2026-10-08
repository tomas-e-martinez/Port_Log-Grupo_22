# Trabajo Practico Integrador: Port Log - Sprint 2

## Integrantes
- **Grupo:** 22
- **Alumno:** Tomás Ezequiel Martínez
- **Repositorio:** https://github.com/tomas-e-martinez/Port_Log-Grupo_22.git

---

## Objetivo del Sprint 2
Aplicar tecnicas de procesamiento de imagenes y reconocimiento de texto sobre las fotos de los buques para verificar que infracciones de velocidad tienen evidencia visual valida.

---

## Contexto del Problema
Los radares del puerto sacan fotos de la proa de los barcos cuando ingresan con exceso de velocidad para registrar su matricula. Las imagenes se dividen entre las que tienen solo el recorte de la patente y las que muestran el buque completo.

El trabajo de este sprint consiste en detectar el texto de las matriculas a partir de las imagenes y cruzarlo contra la tabla de movimientos del Sprint 1 para identificar que infracciones quedaron respaldadas con una foto valida y analizar el rendimiento de las capturas.

- **Dataset tabular:** `port_log/data/interim/port_movements.csv`
- **Dataset de imagenes:** [port_log_images.zip](https://github.com/HAD141/datasets/raw/refs/heads/main/TrabajosPracticos/port_log/port_log_images.zip)