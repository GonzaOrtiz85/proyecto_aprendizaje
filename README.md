# Proyecto de Aprendizaje Automático

## Alumno
**C. Gonzalo Ortiz**

## Materia
Aprendizaje Automático  
Tecnicatura en Datos e Inteligencia Artificial – Año 2025

---

## Propuesta del proyecto

### Descripción general del proyecto
El proyecto tiene como finalidad analizar y predecir la cantidad de espectadores de cine en Argentina a nivel provincial, utilizando datos históricos del período **2001–2023**.  
El dataset contiene la cantidad de espectadores por provincia o región del país para cada año, lo que permite estudiar la evolución del consumo cultural y su distribución territorial.

A partir de estos datos se aplicarán las etapas vistas en clase —preprocesamiento, análisis exploratorio y modelos supervisados de regresión— con el objetivo de **estimar tendencias futuras a partir de la información histórica disponible.**

Este análisis es relevante para la **planificación cultural**, la **gestión de salas de cine** y la **distribución audiovisual**, aportando una herramienta basada en datos para comprender la evolución del público en las distintas regiones del país.

---

### Objetivo general
Desarrollar un modelo de Aprendizaje Automático supervisado que permita analizar y estimar tendencias en la cantidad de espectadores de cine en Argentina, a partir de los datos históricos provinciales del período 2001–2023.

---

### Objetivos específicos
- Analizar la evolución temporal del público de cine en cada provincia entre 2001 y 2023.  
- Detectar patrones y diferencias regionales en la asistencia al cine.  
- Crear variables derivadas del tiempo (por ejemplo, cantidad de espectadores del año anterior y variación interanual).  
- Construir y comparar modelos de regresión (lineal y basados en árboles) aplicados a los datos históricos.  
- Evaluar el desempeño de los modelos mediante métricas de error apropiadas (MAE, MSE, R²).

---

### Tipo de problema
Se trata de un **problema de regresión supervisada**, en el que se busca predecir un valor numérico continuo —la cantidad de espectadores— utilizando información histórica temporal generada a partir del propio dataset.

---

### Modelos a utilizar
De acuerdo con el material de clase:
- **Regresión Lineal** (Clase 4)  
- **Árbol de Decisión Regressor** (Clase 5)  
- **Random Forest Regressor** (Clase 5)

Los modelos serán implementados con la librería **scikit-learn**, siguiendo las prácticas vistas en el curso.

---

## Reformulación de la Etapa 1

A partir de la observación del docente, se realizó una **reformulación metodológica** del proyecto.  
El objetivo no cambia, pero se aclara que el enfoque se basará en el **análisis de series temporales**, utilizando los propios datos históricos del dataset, en lugar de depender de variables externas.

El trabajo buscará estimar la cantidad de espectadores de cine en Argentina a partir de la **información de años anteriores**, generando variables derivadas del tiempo (por ejemplo, el valor del año previo o la variación anual).  
De esta forma, el modelo podrá reconocer patrones y tendencias sin necesidad de incorporar nuevas variables externas.

Este ajuste no modifica la temática general del proyecto, sino que aclara su planteo técnico y lo alinea con los contenidos trabajados en clase, especialmente con los modelos de **regresión supervisada** vistos durante el curso.

---

## Etapa 2 – Descripción del dataset

### Fuente y acceso
- **Dataset:** `data/raw/a04-espectadores-cine-nivel-provincial.csv`  
- **Origen:** datos públicos del ámbito cultural argentino, publicados por el **Ministerio de Cultura** en el portal **datos.gob.ar**.  
- **Fecha de adquisición:** octubre 2024.  
- **Licencia:** datos de dominio público para uso académico.  
- **Procesamiento previo:** ninguno (se utiliza el archivo original sin modificaciones).

---

### Estructura y contenido
- **Instancias (filas):** 23  
- **Características (columnas):** 25  
  - 24 columnas con conteos de espectadores por provincia (códigos INDEC).  
  - 1 índice implícito que representa los años del 2001 al 2023.

Las columnas siguen el patrón `espect_cine_XX`, donde `XX` es el código de la jurisdicción según INDEC (por ejemplo: 2 = CABA, 6 = Buenos Aires, 94 = Tierra del Fuego).

Todos los valores corresponden a **cantidades enteras de espectadores**.

---

### Observaciones
- Cada fila representa un año del período **2001–2023**.  
- Es esperable una caída abrupta en los años **2020–2021** por el impacto de la pandemia (COVID-19).  
- El dataset se usará para el análisis exploratorio (EDA) y, en etapas posteriores, para construir los modelos de regresión supervisada.

---

## Estructura del repositorio
