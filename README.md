Explorando factores de comportamiento en NovaRetail+

NovaRetail+ es una plataforma de comercio electrónico en Latinoamérica. Este análisis busca responder:

¿Qué factores del comportamiento del cliente están más fuertemente asociados con el ingreso anual generado?

Principio rector del proyecto: correlación no implica causalidad.

Herramientas
Python (pandas): limpieza y exploración
Visualización: heatmaps y scatterplots
Coeficientes de asociación: Pearson, Spearman, punto biserial y V de Cramér
Metodología
Limpieza y exploración del dataset.
Visualización de relaciones con heatmaps y scatterplots.
Cálculo del coeficiente adecuado según el tipo de variable (numérica, categórica o binaria).
Interpretación cuidando no atribuir causalidad.
Hallazgos

1. Compras mensuales e ingreso anual. No se puede afirmar que incentivar las compras mensuales sea la causa única del aumento de ingresos, porque ambas variables podrían contar la misma historia. Hay que revisar la posible colinealidad.

2. Publicidad dirigida y visitas. No se puede afirmar que la publicidad dirigida se convierta eficientemente en ventas directas: su relación con las compras mensuales desciende drásticamente a cerca de 20%.

3. Satisfacción, edad e ingreso personal. Son independientes del desempeño comercial en este dataset. Esto no significa que no importen, sino que sus efectos no son detectables de forma directa o lineal aquí.

Siguientes pasos
Revisar la colinealidad entre compras mensuales e ingreso anual.
Probar modelos que capturen relaciones no lineales.
Estructura del repositorio
├── data/          # dataset
├── notebooks/     # análisis en Python
└── README.md
Autor

Miguel Angel Rodriguez Vega · LinkedIn
