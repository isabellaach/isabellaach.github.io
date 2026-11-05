---
title: "¿A quién alcanzará el fuego? Alerta de evacuación por incendios en el Perú"
excerpt: "<img src='/images/incendios.jpg' alt='Mapa de corredores de viento de los incendios activos' style='width:100%;max-width:600px'><br/><b>Pregunta:</b> ¿qué poblaciones deberían prepararse para evacuar en las próximas 24–72 h, según hacia dónde empujará el viento a los incendios activos?<br/><b>Resultado:</b> de 161 incendios activos, solo 1 justificaba preparar una evacuación en 24 h (Juli, Puno: 3 372 personas en su corredor); el círculo fijo de 5 km sobreestima el riesgo en 142 de 150 incendios.<br/><a href='https://claude.ai/artifact/B6Xd7Qk5C5pGghCu1tjt68'>Dashboard</a> · <a href='https://github.com/isabellaach/python-qlab/tree/main/tarea_data_raster'>Código</a>"
collection: portfolio
---

**Pregunta.** ¿Qué poblaciones del Perú deberían prepararse para evacuar en las próximas 24–72 h, según hacia dónde empujará el viento a los incendios activos de hoy?

**Qué hice.** Crucé los focos de calor VIIRS de NASA FIRMS con el pronóstico horario de viento, humedad y lluvia de Open-Meteo y la población de WorldPop. En vez de un círculo fijo alrededor del fuego, el área de riesgo es un corredor que sigue al viento pronosticado. Medí el área quemada con el dNBR de Sentinel-2.

**Resultados (corte: 21 de octubre de 2026).**
- De 161 incendios activos, **solo 1 justificaba preparar una evacuación en 24 h**: Juli (Puno), con 3 372 personas en su corredor.
- La dirección del viento cambia a quién avisar: en Candarave (Tacna) el corredor tiene **1 641 personas frente a 201** en el círculo de 5 km.
- El dNBR mide **101 ha quemadas** en Tahuania (Ucayali), un 44 % más que la huella térmica del satélite.

[Dashboard interactivo](https://claude.ai/artifact/B6Xd7Qk5C5pGghCu1tjt68) · [Código y metodología](https://github.com/isabellaach/python-qlab/tree/main/tarea_data_raster)
