# Analisis-ConnectaTel
Análisis exploratorio y limpieza de datos de una empresa de telecomunicaciones en México y Colombia, con segmentación de usuarios por edad, plan y nivel de uso para identificar patrones de consumo, outliers y oportunidades comerciales.
## Descripción
Este proyecto analiza datos de una empresa de telecomunicaciones con operaciones en México y Colombia. El objetivo es entender el comportamiento de los usuarios en llamadas y mensajes, revisar la calidad de los datos, detectar valores atípicos y generar recomendaciones comerciales.

## Datasets utilizados
- `plans.csv`: información de los planes.
- `users_latam.csv`: información de usuarios.
- `usage.csv`: registros de llamadas y mensajes.

## Herramientas utilizadas
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Proceso de análisis
1. Carga y exploración de datos.
2. Revisión de valores faltantes.
3. Detección de valores inválidos.
4. Estandarización de fechas.
5. Limpieza de datos.
6. Análisis exploratorio.
7. Detección de outliers.
8. Segmentación de clientes.
9. Conclusiones y recomendaciones.

## Principales hallazgos
- La columna `age` contenía valores inválidos como `-999`.
- La columna `city` tenía valores nulos y el valor `"?"`.
- La columna `churn_date` tenía muchos valores nulos, pero estos representan usuarios activos.
- En `reg_date` aparecieron 40 fechas del año 2026, fuera del rango esperado.
- En `usage`, la mayoría de los registros corresponde a 2024, pero había 50 registros sin fecha.
- Existen más mensajes que llamadas.
- Las columnas `duration` y `length` deben analizarse según el tipo de registro.
- Se detectaron posibles valores atípicos en duración de llamadas y longitud de mensajes.

## Conclusión
El dataset es útil para analizar el comportamiento de los usuarios de ConnectaTel, pero requiere limpieza previa. Después de corregir valores inválidos, fechas fuera de rango y valores faltantes, es posible construir segmentaciones útiles para mejorar la oferta comercial y la experiencia del cliente
