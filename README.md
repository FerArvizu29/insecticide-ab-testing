# Análisis Estadístico de la Efectividad de Insecticidas  
### Regresión Logística, Modelos Dosis–Respuesta y Pruebas A/B

## Descripción general
En este proyecto se analiza la efectividad de tres insecticidas variando la dosis aplicada en grupos homogéneos de insectos.  
La variable respuesta es binaria (éxito / fracaso), por lo que el análisis se realiza mediante modelos lineales generalizados (GLM), criterios de selección de modelos y pruebas de hipótesis.

El objetivo del análisis es:
- identificar el insecticida más efectivo,
- evaluar la relación dosis–respuesta,
- y estimar la dosis necesaria para alcanzar un nivel objetivo de efectividad.

---

## Descripción de los datos.
- Datos experimentales con respuestas binarias agrupadas.
- Tres insecticidas evaluados a distintos niveles de dosis.
- Los datos se encontraban originalmente agrupados y posteriormente se desagruparon para el ajuste de modelos.

Los datos pueden consultarse en el archivo _Datos_Insecticidas.csv_ del mismo repositorio.
---

## Metodología

### 1. Preparación de datos
- Desagrupación de los datos binarios para obtener observaciones individuales.
- Análisis exploratorio para identificar patrones en la relación dosis–respuesta.

### 2. Modelado estadístico
Se ajustaron distintos modelos lineales generalizados:

- Modelos con las covariables **Insecticida**, **Dosis** y su interacción.
- Modelos que incorporan **efectos no lineales de la dosis** (término cuadrático).
- Evaluación de diferentes funciones de enlace para datos binarios.

### 3. Selección de modelo
- Comparación de modelos mediante el **criterio de información de Akaike (AIC)**.
- Selección del modelo más verosímil.
- Verificación de supuestos y evaluación del ajuste del modelo.

### 4. Estimación e inferencia
- Estimación puntual de los parámetros del modelo.
- Obtención de curvas dosis–respuesta por insecticida.
- Cálculo de la **dosis requerida para alcanzar una efectividad del 72%** en cada tratamiento.

### 5. Pruebas de hipótesis
- Aplicación de pruebas estadísticas (ANOVA o enfoque de pruebas A/B) para:
  - identificar diferencias estadísticamente significativas entre insecticidas,
  - determinar el insecticida más efectivo,
  - evaluar si los insecticidas restantes presentan un desempeño similar.

---

## Resultados principales
- Se identificó un insecticida con **efectividad significativamente mayor**.
- Los insecticidas restantes mostraron un rendimiento **similar entre sí e inferior** al tratamiento más efectivo.
- La relación dosis–respuesta varía entre insecticidas, evidenciando efectos de interacción.


El reporte puede consultarse en el archivo _Reporte_Insecticidas.pdf_ del mismo repositorio.
---

## Herramientas y tecnologías
- **Métodos estadísticos:** Regresión logística, GLM, ANOVA, pruebas A/B  
- **Lenguajes:** R
- **Enfoque:** Diseño experimental, inferencia estadística, análisis de datos aplicados.

---

## Posibles aplicaciones
- Optimización de dosis en experimentos biológicos.
- Comparación estadística de tratamientos.
- Toma de decisiones basada en evidencia mediante análisis estadístico.

---

## Autor
Fernando Arvizu Vargas
