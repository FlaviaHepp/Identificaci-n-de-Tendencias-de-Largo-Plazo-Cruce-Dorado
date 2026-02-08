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
