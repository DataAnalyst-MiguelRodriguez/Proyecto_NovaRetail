# 📊 NovaMarket: Análisis de Correlación de Actividad, Compras e Ingresos

Análisis exploratorio de datos (EDA) en Python sobre **1,500 usuarios** de un e-commerce, para identificar qué métricas de actividad se asocian con las compras y los ingresos mensuales, y traducir los resultados en recomendaciones de negocio.

![Python](https://img.shields.io/badge/Python-3.x-blue) ![Pandas](https://img.shields.io/badge/Pandas-EDA-150458) ![Seaborn](https://img.shields.io/badge/Seaborn-Visualización-4c72b0) ![SciPy](https://img.shields.io/badge/SciPy-Estadística-8caae6)

## 🎯 Objetivo
Identificar relaciones entre métricas de actividad (visitas, gasto publicitario, satisfacción, edad), compras e ingresos mensuales, para generar hipótesis accionables para el equipo de negocio. El análisis es **correlacional, no causal**.

## 🔍 Hallazgos clave
| # | Hallazgo | Evidencia | Implicación de negocio |
|---|----------|-----------|------------------------|
| 1 | Más visitas se asocian con más compras (relación débil-moderada) | Pearson 0.30 · Spearman 0.28 | Probar estrategias de engagement previas a la compra y validarlas con experimentos controlados (A/B) |
| 2 | La suscripción casi no se asocia con los ingresos | Punto-biserial 0.063 | No usar la suscripción como único criterio de segmentación; combinarla con otras métricas |
| 3 | Visitas y gasto publicitario van juntos | r = 0.59 (heatmap) | Revisar si el gasto publicitario está atrayendo tráfico o solo sigue al tráfico existente |
| 4 | Satisfacción y edad casi no muestran relación con compras o ingresos | \|r\| < 0.06 (heatmap) | No priorizar estas variables en segmentaciones iniciales |

> Las compras y los ingresos tienen una correlación de 0.96. Es esperable, ya que los ingresos provienen de las compras.

## 🧪 Metodología
1. **Limpieza:** exclusión de usuarios sin visitas en los últimos 30 días.
2. **Visualización:** heatmap de correlaciones, pairplot y scatterplots de pares clave.
3. **Coeficientes según el tipo de variable:**
   - **Pearson y Spearman:** numérica vs. numérica (relación lineal y monótona).
   - **Punto-biserial:** binaria vs. numérica (suscripción vs. ingresos).
   - **V de Cramér:** categórica vs. categórica (región vs. dispositivo).
4. **Interpretación orientada a negocio:** cada hallazgo incluye evidencia, qué se puede afirmar, qué *no* y qué hacer.

## 🛠️ Stack
`Python` · `Pandas` · `NumPy` · `Seaborn` · `Matplotlib` · `SciPy` · `Jupyter Notebook`

## ⚠️ Limitaciones
- Análisis correlacional: no permite afirmar causalidad.
- Variables no controladas: campañas, antigüedad del usuario, promociones.
- Efectos de segmentación aún no explorados.

## 🚀 Próximos pasos
- Análisis por cohortes.
- Segmentación por dispositivo y región.
- Diseño de experimentos A/B para validar las hipótesis.

## 📁 Estructura
```
├── 8_3_Reporte_de_análisis_de_correlación_NovaMarket.ipynb
├── nova_market_activity.csv
└── README.md
```

## ▶️ Cómo ejecutarlo
```bash
git clone https://github.com/TU_USUARIO/TU_REPO.git
cd TU_REPO
pip install pandas numpy seaborn matplotlib scipy jupyter
jupyter notebook
```

## 👤 Autor
**TU NOMBRE** · [LinkedIn]https://www.linkedin.com/in/miguel-rodriguez-dataanalyst/ · [Correo]mian.rove04@gmail.com
