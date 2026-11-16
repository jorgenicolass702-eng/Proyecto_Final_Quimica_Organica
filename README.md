# Proyecto Final de Química Orgánica: Reacciones y obtenciones de hidrocarburos

Ingeniería Ambiental, FAMARENA, Universidad Distrital Francisco José de Caldas (QUIMORG 2026-III).

## Descripción
Base de datos de 200 reacciones (100 reacciones y 100 obtenciones) de 10 hidrocarburos
(pentano, isopentano, hexano, heptano, octano, pent-2-eno, 2-metilpent-2-eno, hex-1-eno,
ciclopropeno y ciclobuteno), consultadas en CAS SciFinder, con análisis gráfico en Python,
informe en LaTeX y presentación en Power BI.

## Estructura del repositorio
```
├── Analisis_Grafico_Reacciones/   # Cuaderno Colab/Jupyter con explicación en Markdown
├── Informe_Latex/                 # main.tex, references.bib, imagenes/
├── Datos/Datos_Reacciones.xlsx    # Tabla de datos recolectados
├── PowerBI/Presentacion_proyecto.pbix
└── README.md
```

## Variables
Catalizador, reactivo, solvente, temperatura, medio, productos, nombre y tipo de reacción;
peso molecular, punto de fusión, punto de ebullición, densidad, pKa, momento dipolar,
solubilidad en agua y presión de vapor.

## Integrantes
| Integrante | Código | Usuario GitHub | Responsabilidad |
|---|---|---|---|
| Jorge Nicolás Méndez Castellanos | 20241180048 | @USUARIO_JORGE | Análisis gráfico (Colab) e informe LaTeX |
| Laura Alejandra Parra | 20252180055 | @USUARIO_LAURA | Por definir |
| Gabriela Santamaría | 20252180048 | @USUARIO_GABRIELA | Por definir |

## Cómo reproducir el análisis
1. Abrir el cuaderno en `Analisis_Grafico_Reacciones/` en Google Colab.
2. Subir `Datos/Datos_Reacciones.xlsx` al entorno.
3. Ejecutar las celdas en orden (mapa de calor, V de Cramér, gráficas de tendencias).
