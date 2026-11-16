# 🧪 Proyecto Final de Química Orgánica — Reacciones y Obtenciones de Hidrocarburos

> **Proyecto académico** | Química Orgánica (QUIMORG 2026-III)  
> Ingeniería Ambiental — FAMARENA  
> Universidad Distrital Francisco José de Caldas

---

## 📋 Descripción del proyecto

Este repositorio contiene el desarrollo del proyecto final de Química Orgánica, enfocado en el estudio sistemático de las **reacciones químicas y métodos de obtención de 10 hidrocarburos**, mediante la construcción de una base de datos de **200 registros**, distribuidos en 100 reacciones y 100 obtenciones.

La información experimental y fisicoquímica fue consultada en **CAS SciFinder**, con el propósito de identificar las condiciones de reacción, los reactivos, catalizadores, solventes, productos y propiedades características de los compuestos estudiados.

El proyecto integra tres componentes principales:

- **Base de datos:** recopilación y organización de 200 reacciones y obtenciones.
- **Análisis gráfico:** procesamiento estadístico y visualización de datos mediante Python en Google Colab/Jupyter Notebook.
- **Informe científico:** presentación de la metodología, resultados, análisis y conclusiones mediante LaTeX.
- **Visualización interactiva:** presentación de resultados mediante Power BI.

El objetivo es analizar las relaciones entre las condiciones experimentales, los tipos de reacción, los métodos de obtención y las propiedades fisicoquímicas de los hidrocarburos seleccionados.

---

## 🗂️ Estructura del repositorio

```text
proyecto-quimica-organica/
│
├── README.md
│
├── Analisis_Grafico_Reacciones/
│   └── analisis_reacciones.ipynb
│
├── Informe_Latex/
│   ├── main.tex
│   ├── references.bib
│   └── imagenes/
│
├── Datos/
│   └── Datos_Reacciones.xlsx
│
└── PowerBI/
    └── Presentacion_proyecto.pbix
```

---

## 🔬 Hidrocarburos estudiados

El proyecto comprende 10 hidrocarburos pertenecientes a tres grandes familias: alcanos, alquenos y cicloalquenos.

### 1. Alcanos

| Código | Compuesto | Fórmula molecular | Clasificación |
|---|---|---|---|
| H01 | Pentano | C₅H₁₂ | Alcano lineal |
| H02 | Isopentano (2-metilbutano) | C₅H₁₂ | Alcano ramificado |
| H03 | Hexano | C₆H₁₄ | Alcano lineal |
| H04 | Heptano | C₇H₁₆ | Alcano lineal |
| H05 | Octano | C₈H₁₈ | Alcano lineal |

### 2. Alquenos

| Código | Compuesto | Fórmula molecular | Clasificación |
|---|---|---|---|
| H06 | Pent-2-eno | C₅H₁₀ | Alqueno interno |
| H07 | 2-Metilpent-2-eno | C₆H₁₂ | Alqueno ramificado |
| H08 | Hex-1-eno | C₆H₁₂ | Alqueno terminal |

### 3. Cicloalquenos

| Código | Compuesto | Fórmula molecular | Clasificación |
|---|---|---|---|
| H09 | Ciclopropeno | C₃H₄ | Cicloalqueno |
| H10 | Ciclobuteno | C₄H₆ | Cicloalqueno |

**Distribución de los compuestos:**

- 5 alcanos.
- 3 alquenos.
- 2 cicloalquenos.
- 10 hidrocarburos en total.

---

## ⚗️ Base de datos de reacciones y obtenciones

La base de datos contiene **200 registros**, organizados en dos categorías:

| Categoría | Cantidad | Descripción |
|---|---:|---|
| Reacciones | 100 | Transformaciones químicas en las que participan los hidrocarburos estudiados. |
| Obtenciones | 100 | Métodos y rutas de síntesis para producir los hidrocarburos seleccionados. |
| **Total** | **200** | **Registros recopilados y organizados.** |

### Variables registradas

La información se organiza en variables experimentales, químicas y fisicoquímicas.

| Categoría | Variables |
|---|---|
| Identificación | Compuesto, nombre y tipo de reacción. |
| Condiciones experimentales | Reactivo, catalizador, solvente, temperatura y medio de reacción. |
| Productos | Nombre e identificación de los productos obtenidos. |
| Propiedades fisicoquímicas | Peso molecular, punto de fusión, punto de ebullición, densidad, pKa, momento dipolar, solubilidad en agua y presión de vapor. |

**Consideraciones sobre los datos:**

- Las propiedades deben conservar sus unidades correspondientes.
- Se debe mantener la trazabilidad de las fuentes consultadas.
- Los datos no disponibles deben identificarse como valores faltantes y no sustituirse por valores inventados.
- Las condiciones experimentales deben corresponder a la fuente bibliográfica consultada.
- Se debe diferenciar entre los métodos de obtención y las reacciones de transformación.

---

## 🗃️ Fuente de información

La fuente principal de consulta para la recopilación de información química es **CAS SciFinder**.

| Información | Fuente |
|---|---|
| Reacciones químicas | CAS SciFinder |
| Métodos de obtención | CAS SciFinder |
| Reactivos y catalizadores | CAS SciFinder |
| Solventes y medios de reacción | CAS SciFinder |
| Condiciones experimentales | CAS SciFinder |
| Propiedades fisicoquímicas | CAS SciFinder |

La información recopilada se utiliza para construir una base de datos organizada que permita realizar comparaciones y análisis estadísticos entre los hidrocarburos estudiados.

---

## 📓 Análisis gráfico en Python

**Directorio:** `Analisis_Grafico_Reacciones/`

El análisis se desarrolla mediante un cuaderno Jupyter Notebook, ejecutable en Google Colab o en un entorno local de Python.

### Librerías utilizadas

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

### Análisis y visualizaciones

| Análisis | Objetivo |
|---|---|
| Mapa de calor | Identificar patrones de asociación entre variables categóricas. |
| V de Cramér | Cuantificar la intensidad de asociación entre variables categóricas. |
| Gráficas de tendencias | Examinar relaciones entre propiedades fisicoquímicas. |
| Distribución de reacciones | Comparar la frecuencia de los tipos de reacción. |
| Comparación de hidrocarburos | Identificar diferencias entre las familias estudiadas. |

### Cómo ejecutar el análisis

**Opción A — Google Colab**

1. Abrir el cuaderno ubicado en `Analisis_Grafico_Reacciones/`.
2. Cargar el archivo `Datos/Datos_Reacciones.xlsx` al entorno.
3. Verificar la ruta de acceso al archivo.
4. Ejecutar las celdas en orden.
5. Revisar las visualizaciones y los resultados estadísticos.

**Opción B — Ejecución local**

Instalar las dependencias:

```bash
pip install pandas numpy matplotlib seaborn openpyxl scipy
```

Ejecutar Jupyter Notebook:

```bash
jupyter notebook
```

Abrir el cuaderno de análisis y ejecutar las celdas secuencialmente.

---

## 📄 Informe científico en LaTeX

**Directorio:** `Informe_Latex/`

El informe presenta el desarrollo metodológico y los resultados del proyecto, integrando la información recopilada en CAS SciFinder con los análisis estadísticos y gráficos.

### Archivos principales

| Archivo | Función |
|---|---|
| `main.tex` | Documento principal del informe. |
| `references.bib` | Base de referencias bibliográficas. |
| `imagenes/` | Gráficas, figuras y recursos visuales. |

### Contenido del informe

1. Introducción.
2. Objetivos generales y específicos.
3. Marco teórico.
4. Metodología de recopilación de datos.
5. Resultados y análisis de las 200 reacciones y obtenciones.
6. Análisis estadístico y gráfico.
7. Discusión de resultados.
8. Conclusiones.
9. Referencias bibliográficas.

---

## 📊 Visualización en Power BI

**Directorio:** `PowerBI/`

**Archivo principal:** `Presentacion_proyecto.pbix`

Se desarrolla una presentación interactiva para explorar y comparar los resultados de la base de datos.

El componente de Power BI permite organizar la información mediante indicadores, filtros y visualizaciones que facilitan la interpretación de los resultados obtenidos.

La presentación se alimenta de la base de datos consolidada en Excel.

---

## 👥 Integrantes y responsabilidades

| Integrante | Código | Usuario GitHub | Responsabilidad |
|---|---|---|---|
| Jorge Nicolás Méndez Castellanos | 20241180048 | jorgenicolass702-eng | Análisis gráfico en Python, Repositorio Git Hub e informe en LaTeX. |
| Laura Alejandra Parra | 20252180055 | @USUARIO_LAURA | Tabla reacciones y validación de datos |
| Gabriela Santamaría | 20252180048 | @USUARIO_GABRIELA | Power BI |

### Participación y colaboración en GitHub

Este repositorio tiene como finalidad documentar el trabajo colaborativo de los integrantes del equipo.

Cada integrante debe contribuir al desarrollo del proyecto mediante:

- Elaboración y actualización de archivos.
- Registro de avances mediante commits.
- Revisión y corrección de información.
- Participación en la documentación.
- Seguimiento de actividades y responsabilidades.

**La participación de todos los integrantes debe quedar reflejada en el historial de contribuciones del repositorio.** La finalidad de GitHub no es únicamente almacenar los archivos finales, sino también evidenciar el proceso de desarrollo colaborativo.

---

## ✅ Estado del proyecto

| Actividad | Estado |
|---|---|
| Selección de los 10 hidrocarburos | ✅ |
| Recopilación de 100 reacciones | ✅ |
| Recopilación de 100 obtenciones | ✅ |
| Consolidación de la base de datos Excel |✅ |
| Validación de información química |✅ |
| Desarrollo del análisis en Python |✅ |
| Elaboración del informe en LaTeX |✅|
| Construcción de la presentación en Power BI | En desarrollo |
| Revisión final y entrega | Pendiente |

---

## 🎯 Objetivo académico

Integrar los conocimientos de química orgánica, análisis de datos y herramientas computacionales para estudiar las rutas de reacción y obtención de diferentes hidrocarburos, identificando patrones en sus condiciones experimentales y propiedades fisicoquímicas.

El proyecto busca fortalecer tanto la interpretación química de los procesos como las competencias de investigación, procesamiento de información, análisis estadístico y trabajo colaborativo.

---

## 👤 Información del proyecto

**Asignatura:** Química Orgánica (QUIMORG 2026-III)  
**Programa:** Ingeniería Ambiental  
**Facultad:** Medio Ambiente y Recursos Naturales (FAMARENA)  
**Institución:** Universidad Distrital Francisco José de Caldas  
**Año:** 2026

---

*Última actualización: noviembre de 2026.*
