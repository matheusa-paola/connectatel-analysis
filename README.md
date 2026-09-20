# Análisis ConnectaTel

## Objetivo del proyecto

Como analista de datos, el objetivo de este proyecto es evaluar el comportamiento de los clientes de ConnectaTel, una empresa de telecomunicaciones en Latinoamérica, utilizando  información registrada hasta el año 2024. El análisis busca identificar patrones de consumo, detectar comportamientos atípicos, construir segmentos de clientes y generar recomendaciones  accionables para mejorar la oferta de planes y las estrategias de retención.

## Datasets utilizados
- **plans.csv**: información de los planes actuales (precio, minutos incluidos, GB incluidos, costo por extra).
- **users_latam.csv**: información de los clientes (edad, ciudad, fecha de registro, plan, fecha de baja/churn).
- **usage.csv**: detalle del uso real de los servicios (llamadas y mensajes por usuario).

## Etapas del análisis
1. **Carga y exploración**: revisión de estructura, tipos de datos y dimensiones de los 3 datasets.
2. **Identificación de problemas de calidad de datos**: detección de valores nulos, sentinels (`-999`, `"?"`) y fechas fuera de rango.
3. **Limpieza de datos**: corrección de sentinels, fechas imposibles y evaluación de nulos como MAR (Missing At Random).
4. **Agregación por usuario**: construcción de métricas de uso (mensajes, llamadas, minutos) combinadas con el perfil del cliente.
5. **Visualización y detección de outliers**: histogramas y boxplots para analizar distribuciones, con cálculo de límites vía método IQR.
6. **Segmentación de clientes**: clasificación por nivel de uso (Bajo/Medio/Alto) y por grupo de edad (Joven/Adulto/Adulto Mayor).
7. **Insight ejecutivo**: conclusiones y recomendaciones de negocio basadas en los hallazgos.
