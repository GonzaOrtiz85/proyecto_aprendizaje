# Proyecto de Aprendizaje Automático

## Alumno
**C. Gonzalo Ortiz**

## Materia
Aprendizaje Automático  
Tecnicatura en Datos e Inteligencia Artificial – Año 2025

---

## Descripción general del proyecto
El proyecto tiene como finalidad analizar y predecir la cantidad de espectadores de cine en Argentina a nivel provincial, utilizando datos históricos del período **2001–2023**.  
El dataset contiene la cantidad de espectadores por provincia o región del país para cada año, lo que permite estudiar la evolución del consumo cultural y su distribución territorial.

A partir de estos datos se aplicarán las etapas vistas en clase —preprocesamiento, análisis exploratorio y modelos supervisados de regresión— con el objetivo de **estimar tendencias futuras a partir de la información histórica disponible.**

Este análisis es relevante para la **planificación cultural**, la **gestión de salas de cine** y la **distribución audiovisual**, aportando una herramienta basada en datos para comprender la evolución del público en las distintas regiones del país.

---

## Objetivo general
Desarrollar un modelo de Aprendizaje Automático supervisado que permita analizar y estimar tendencias en la cantidad de espectadores de cine en Argentina, a partir de los datos históricos provinciales del período 2001–2023.

---

## Objetivos específicos
- Analizar la evolución temporal del público de cine en cada provincia entre 2001 y 2023.  
- Detectar patrones y diferencias regionales en la asistencia al cine.  
- Crear variables derivadas del tiempo (por ejemplo, cantidad de espectadores del año anterior y variación interanual).  
- Construir y comparar modelos de regresión (lineal y basados en árboles) aplicados a los datos históricos.  
- Evaluar el desempeño de los modelos mediante métricas de error apropiadas (MAE, MSE, R²).

---

## Tipo de problema
Se trata de un **problema de regresión supervisada**, en el que se busca predecir un valor numérico continuo —la cantidad de espectadores— utilizando información histórica temporal generada a partir del propio dataset.

---

## Modelos a utilizar
De acuerdo con el material de clase:
- **Regresión Lineal** (Clase 4)  
- **Árbol de Decisión Regressor** (Clase 5)  
- **Random Forest Regressor** (Clase 5)

Los modelos serán implementados con la librería **scikit-learn**, siguiendo las prácticas vistas en el curso.

---

## Estructura del repositorio
