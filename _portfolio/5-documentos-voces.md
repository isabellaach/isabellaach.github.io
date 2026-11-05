---
title: "Voces y documentos peruanos: del archivo escaneado al texto buscable"
excerpt: "<img src='/images/documentos.jpg' alt='Comunicado oficial del MINSA usado como ejemplo de documento escaneado' style='width:100%;max-width:600px'><br/><b>Pregunta:</b> ¿se pueden convertir documentos escaneados y entrevistas en audio en un archivo de texto estructurado y buscable, solo con modelos abiertos?<br/><b>Resultado:</b> 25 documentos y 51 minutos de audio procesados; error por carácter de 0,10 en OCR (PaddleOCR-VL) y error por palabra de 0,24 en transcripción (Whisper turbo).<br/><a href='https://python-qlab-8pczqqvrjifzjm6vcpi2qh.streamlit.app/'>Dashboard</a> · <a href='https://github.com/isabellaach/python-qlab/tree/main/tarea_2'>Código</a>"
collection: portfolio
---

**Pregunta.** ¿Se pueden convertir documentos escaneados y entrevistas en audio en un archivo de texto estructurado y buscable, solo con modelos abiertos y locales?

**Qué hice.** Un pipeline que extrae texto de 25 documentos peruanos (impresos, fotos y manuscritos) con OCR, transcribe 28 clips de audio en español peruano (51 min) con detección de voz y diarización, reemplaza los nombres de personas privadas por seudónimos y extrae campos estructurados con un LLM.

**Resultados** (10 documentos y 10 clips transcritos a mano como referencia):
- **CER 0,10** en OCR con PaddleOCR-VL.
- **WER 0,24** en transcripción con Whisper turbo.
- El LLM coincidió con la revisión humana en 6 de 20 extracciones: sirve como borrador, no como fuente final.

[Dashboard interactivo](https://python-qlab-8pczqqvrjifzjm6vcpi2qh.streamlit.app/) · [Código y metodología](https://github.com/isabellaach/python-qlab/tree/main/tarea_2)

*Imagen: comunicado oficial del Ministerio de Salud del Perú, dominio público (Wikimedia Commons).*
