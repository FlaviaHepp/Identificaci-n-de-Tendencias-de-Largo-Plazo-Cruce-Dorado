# 📍Identificación de Tendencias de Largo Plazo – Cruce Dorado

## 📌Descripción del Proyecto

Este proyecto implementa un análisis clásico de tendencia de largo plazo utilizando medias móviles, conocido como Cruce Dorado (Golden Cross).
El objetivo es identificar acciones que presentan una estructura alcista sólida, donde la media móvil de corto/medio plazo supera a la de largo plazo.

Un Cruce Dorado es una de las señales técnicas más utilizadas para detectar tendencias alcistas sostenidas y suele ser empleada por inversores institucionales y estrategias de momentum.

## 🎯Objetivo del Análisis

Detectar acciones donde:
- La SMA de 50 días (sma_50) es mayor que la SMA de 200 días (sma_200)
- El precio de cierre confirma la estructura de tendencia
- La señal se presenta en la fecha más reciente disponible

## 🧠Insight Clave

- ¿Qué acciones muestran una tendencia alcista fuerte y estructural, validada por un Cruce Dorado?

Estas acciones tienden a:
- Tener mayor probabilidad de continuidad alcista
- Atraer flujos de capital de mediano y largo plazo
- Servir como base para estrategias de trend following o buy & hold táctico

## 🗂️Fuentes de Datos

El análisis se construye a partir de las siguientes tablas:
- indicadores_tecnicos
- sma_50
- sma_200
- precios_diarios
- close

Relación por:
- ticker_id
- fecha

## 🧮Lógica del Modelo

- Se cruzan los indicadores técnicos con los precios diarios por ticker y fecha.

Se filtran únicamente los registros donde:
- sma_50 > sma_200

Se clasifica el estado de la acción como:
- Tendencia Alcista Fuerte (Cruce Dorado)

## 💼Valor de Negocio

- Identificación rápida de activos líderes del mercado

Filtro inicial para:
- Estrategias de momentum
- Rotación sectorial
- Selección de acciones para carteras de largo plazo
- Reduce ruido al enfocarse solo en tendencias confirmadas

## ⚠️Consideraciones

- El Cruce Dorado no indica timing exacto de entrada, sino dirección de fondo

Se recomienda combinar con:
- Volumen
- RSI
- Análisis de riesgo (volatilidad, drawdown)

En mercados laterales puede generar señales falsas

## 🚀Posibles Extensiones

- Validación del cruce con volumen creciente
- Medición de rendimiento posterior a 30 / 90 días
- Análisis por sector o país
- Cruce Dorado + filtro de volatilidad baja

## 👤Autora
Flavia Hepp Proyecto de SQL aplicó un análisis de riesgo basado en eventos.

***
📈 **Cuando la tendencia deja de ser duda… y se vuelve estructura**

En análisis técnico, hay señales que marcan un antes y un después.
Una de las más conocidas (y seguidas) es el **“Cruce Dorado”**.

👉 Analicé las acciones donde la **SMA 50 supera a la SMA 200**, identificando tendencias alcistas de largo plazo.

💡 **Insight clave:**
Cuando la media de corto/mediano plazo (50 días) supera a la de largo plazo (200 días), no es solo momentum…
es una señal de **cambio estructural en la tendencia**.

---

📊 **¿Qué medí?**

* SMA 50 vs. SMA 200
* Precio de cierre actual
* Identificación de activos en **Golden Cross**

---

🧠 **¿Cómo interpretarlo?**

* SMA 50 > SMA 200 → tendencia alcista consolidada
* Confirma que el precio viene ganando fuerza de forma sostenida
* Suele atraer capital institucional y estrategias *trend-following*

---

⚡ **¿Por qué importa?**

Porque este tipo de señal:

* Filtra ruido de corto plazo
* Identifica tendencias más “robustas”
* Es base de muchas estrategias sistemáticas

---

📌 Pregunta para la comunidad:
¿Usan el Golden Cross como señal de entrada… o solo como confirmación de tendencia?

#QuantFinance #Trading #DataScience #StockMarket #TechnicalAnalysis #TrendFollowing #SQL #Analytics
