# Descripción del dataset – Proyecto de Aprendisaje Automático

**Nombre del dataset:** Espectadores de cine en Argentina por provincia (2001–2023)  
**Archivo:** `data/raw/a04-espectadores-cine-nivel-provincial.csv`

## Origen y acceso
- **Fuente:** datos públicos del ámbito cultural argentino (series históricas de publico de cine por jurisdicción).  
  Referencia institucional: Ministerio de Cultura / sistema de estadísticas culturales publicados en **datos.gob.ar**.  
- **Fecha de adquisición:** octubre 2024.  
- **Licencia/uso:** datos de **dominio público** para fines academicos.  
- **Procesamiento previo realizado para esta entrega:** **ninguno** (se publica el archivo tal cual fue descargado; cualquier transformación se va a documentar en las etapas posteriores).

## Cobertura y alcance
- **Unidad de analisis:** cantidad anual de espectadores de cine por **provincia / jurisdicción**.  
- **Cobertura temporal:** **2001–2023** (23 años).  
- **Cobertura geografica:** 24 jurisdicciones + CABA (segun codigos INDEC).

> Nota: el archivo original no incluye una columna explicita de “año”; cada **fila** corresponde secuencialmente a un año del periodo **2001–2023**.

## Estructura del archivo
- **Instancias (filas):** 23  
- **Características (columnas):** 25  
  - 24 columnas con conteos de espectadores por jurisdicción (una por provincia/codigo INDEC).  
  - 1 columna índice implicita por fila (no esta en el archivo; el orden de filas representa los años).

## Nombres de columnas (ejemplos)
Las columnas siguen el patrón `espect_cine_XX`, donde `XX` es el **código INDEC** de la jurisdicción.  
Listado completo de códigos y nombres:

| Código | Columna           | Jurisdicción            |
|-------:|-------------------|-------------------------|
| 2      | espect_cine_2     | CABA                    |
| 6      | espect_cine_6     | Buenos Aires            |
| 10     | espect_cine_10    | Catamarca               |
| 14     | espect_cine_14    | Córdoba                 |
| 18     | espect_cine_18    | Corrientes              |
| 22     | espect_cine_22    | Chaco                   |
| 26     | espect_cine_26    | Chubut                  |
| 30     | espect_cine_30    | Entre Ríos              |
| 34     | espect_cine_34    | Formosa                 |
| 38     | espect_cine_38    | Jujuy                   |
| 42     | espect_cine_42    | La Pampa                |
| 46     | espect_cine_46    | La Rioja                |
| 50     | espect_cine_50    | Mendoza                 |
| 54     | espect_cine_54    | Misiones                |
| 58     | espect_cine_58    | Neuquén                 |
| 62     | espect_cine_62    | Río Negro               |
| 66     | espect_cine_66    | Salta                   |
| 70     | espect_cine_70    | San Juan                |
| 74     | espect_cine_74    | San Luis                |
| 78     | espect_cine_78    | Santa Cruz              |
| 82     | espect_cine_82    | Santa Fe                |
| 86     | espect_cine_86    | Santiago del Estero     |
| 90     | espect_cine_90    | Tucumán                 |
| 94     | espect_cine_94    | Tierra del Fuego        |

## Tipos de datos
- Todas las columnas `espect_cine_XX`: **entero** (conteo de espectadores por año y provincia).  
  En caso de encontrarse valores con separadores de miles en versiones alternativas del archivo, se aclarará su normalización mas adelante. En esta entrega se mantiene el archivo original sin cambios.

## Observaciones relevantes
- **Series con shock 2020–2021:** se espera una caida abrupta por pandemia (COVID-19).  
- **Interpretación temporal:** el orden de filas representa los años 2001→2023 (23 registros).  
- **Uso previsto:** el dataset se va a emplear para análisis exploratorio y, en etapas siguientes, para construir modelos supervisados de **regresión** que estimen tendencias a partir de la información histórica disponible (de acuerdo al material de las clases 1 a 5).
