# 🌬️ Análisis Factorial de Contaminantes en Monterrey

Este proyecto fue desarrollado como parte del curso **Aplicación de Métodos Multivariados en Ciencia de Datos** en el Tecnológico de Monterrey. El objetivo fue aplicar un análisis factorial exploratorio para entender la estacionalidad y las causas principales de los contaminantes atmosféricos en la zona centro de Monterrey, a lo largo del año.

## 🎯 Objetivo

Identificar los factores latentes que explican la variabilidad en los niveles de contaminantes atmosféricos mediante análisis factorial exploratorio (AFE), aplicando técnicas estadísticas multivariadas a series temporales de estaciones de monitoreo ambiental.

---

## 📌 Metodología

1. **Selección y limpieza de datos**
   - Datos provenientes del SIMA (Sistema Integral de Monitoreo Ambiental).
   - Se filtraron 5 zonas con <5% de datos nulos.
   - Relleno de valores faltantes con promedio móvil.
   - Eliminación de valores extremos (outliers).

2. **Reducción de dimensiones**
   - De 240 columnas originales → 42 variables finales relacionadas con contaminantes.
   - Agrupación de datos por estaciones del año: primavera, verano, otoño, invierno.

3. **Validaciones estadísticas**
   - Prueba de Kaiser-Meyer-Olkin (KMO) para evaluar adecuación del AFE:
     - Primavera: 0.61
     - Verano: 0.66
     - Otoño: 0.76
     - Invierno: 0.76

4. **Análisis factorial**
   - Método: Máxima verosimilitud
   - Rotación: Ortogonal (Quartimax)
   - Número de factores: 4 (determinado por Scree Plot)

---

## 📊 Resultados clave

Se identificaron **5 factores principales** que agrupan las causas más comunes de contaminación:

| Factor | Descripción |
|--------|-------------|
| 🔥 Combustión energética | Relacionado con CO y SO₂ |
| 🏗️ Construcción/polvo
