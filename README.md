# ProyectoDSII-AugustoParajon
Análisis climático de San Miguel de Tucumán para anticipar picos de frío y calor, optimizar stock de climatizadores y mejorar campañas de venta usando EDA, PCA, clustering y visualizaciones en Python.


**Primera Entrega – Data Science II**  
**Autor:** Augusto Parajón  
**Fecha:** 5 de agosto de 2025  

---

## 📖 Descripción del Proyecto

En este trabajo se analiza el comportamiento climático de San Miguel de Tucumán entre el 1 de enero de 2005 y el 31 de julio de 2025, con el objetivo de anticipar picos de frío y calor y así optimizar la gestión de inventarios y el diseño de campañas de venta de productos de climatización (ventiladores, aires acondicionados, estufas) en Oscar Barbieri S.A.

### Abre este notebook en Colab

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1u7T-wuqFlMpkKDSMlAX30vlGpaBs0WkL#scrollTo=iNzoYcpZGN6h)



---

## 🎯 Objetivos

- **Detectar patrones estacionales** de temperatura y demanda.  
- **Cuantificar el impacto** de eventos extremos (olas de frío y calor) sobre las ventas.  
- **Explorar la relación** entre amplitud térmica y comportamiento de compra.  
- **Validar la estabilidad** de los ciclos climáticos a lo largo de los años.  

---

## 🗃️ Resumen de los Datos

- **Periodo de análisis:** 1 Ene 2005 – 31 Jul 2025  
- **Origen:** API Open-Meteo (datos diarios)  
- **Variables clave:**  
  - Temperatura (mín., máx., media)  
  - Precipitación diaria  
  - Humedad, presión al nivel del mar  
  - Velocidad de viento, radiación solar  
  - Variables derivadas: amplitud térmica, estación del año, día de la semana  

---

## 📊 Metodología

1. **Adquisición y limpieza**  
   - Descarga diaria de registros climáticos  
   - Imputación de valores faltantes y detección de outliers  

2. **Análisis exploratorio (EDA)**  
   - Distribuciones univariadas (histogramas, boxplots)  
   - Correlaciones y scatter plots bivariados  
   - Descomposición de series temporales y gráficas de tendencia  

3. **Análisis multivariado**  
   - PCA para reducir dimensionalidad  
   - Clustering para identificar perfiles climáticos recurrentes  

4. **Visualizaciones ejecutivas**  
   - Series temporales superpuestas (temperatura vs. demanda)  
   - Mapas de calor de correlación  
   - Gráficos de boxplot por estación  

---

## 🔍 Hallazgos Clave

- Se confirma un **patrón estacional** muy marcado, con temperaturas máximas en enero–febrero y mínimas en junio–julio.  
- Los **picos extremos** de calor (> 30 °C) coinciden con un aumento promedio del **30 %** en la demanda de climatizadores.  
- La **amplitud térmica moderada** se asocia a ventas más **estables**, mientras que variaciones extremas generan picos de pedidos.  
- El análisis de PCA revela que dos componentes (intensidad térmica y radiación/presión) explican más del **80 %** de la varianza, y el clustering repite cuatro perfiles climáticos cada año.

---

## 🚀 Recomendaciones

1. **Inventario Dinámico**  
   - Ajustar pedidos de productos de climatización según el perfil climático anticipado.  

2. **Promociones Temporales**  
   - Programar ofertas previas a eventos de calor y frío extremos para maximizar el engagement.  

3. **Modelo Predictivo**  
   - Desarrollar alertas automáticas basadas en PCA y clustering para planificar con 7 días de antelación.  

4. **Monitoreo Continuo**  
   - Integrar dashboards operativos que muestren el estado climático diario y su impacto en ventas.  

---

