# Explicabilidad Forense de Tatuajes mediante Visión Artificial y Modelos Multimodales

Repositorio asociado al Trabajo Fin de Grado **"Explicabilidad Forense de Tatuajes mediante Visión Artificial y Modelos de Lenguaje (LLM)"**.

El proyecto estudia el uso combinado de técnicas de visión artificial, extracción de características explicables y modelos multimodales para el análisis automático de tatuajes en contextos relacionados con la identificación forense.

## Estructura del repositorio

```text
├── Codigo
│   ├── Fase1-InformesForensesTatuajes
│   │   ├── Extractor de Características
│   │   │   └── extractor_caracteristicas.ipynb
│   │   │
│   │   └── Informes con LLM
│   │       └── generador_informes_qwen.ipynb
│   │
│   └── Fase2-CompararLLM
│       └── comparacion_modelos_multimodales.ipynb
│
├── Resultados.zip
│   ├── features_merged
│   ├── forensic_reports_qwen_batches
│   └── LLM evaluation
│
├── Memoria.pdf
│
└── README.md
```

## Descripción de los componentes

### Fase 1 - Informes forenses de tatuajes

#### Extractor de Características

Notebook encargado de extraer automáticamente características explicables a partir de imágenes de tatuajes segmentados.

Entre las características obtenidas se incluyen:

* Información espacial y de localización.
* Características geométricas.
* Medidas relacionadas con la forma.
* Métricas de apariencia visual.
* Información utilizada posteriormente para la generación de informes.

Los resultados generados se almacenan en archivos CSV y JSON.

#### Informes con LLM

Notebook encargado de generar informes descriptivos utilizando:

* La imagen del tatuaje.
* Las características previamente extraídas.
* Un modelo multimodal basado en Qwen.

El objetivo es producir descripciones estructuradas apoyadas en información visual y características cuantitativas previamente calculadas.

---

### Fase 2 - Comparación de modelos multimodales

Notebook utilizado para evaluar distintos modelos visión-lenguaje sobre imágenes reales de tatuajes.

Las tareas realizadas incluyen:

* Generación de respuestas mediante distintos modelos multimodales.
* Comparación de precisión entre arquitecturas.
* Construcción de matrices de confusión.
* Cálculo de métricas de evaluación.
* Generación de gráficas y análisis de resultados.

Los modelos evaluados fueron:

* Moondream2
* LLaVA 1.5 7B
* Qwen2-VL 2B

## Resultados

El archivo `Resultados.zip` contiene los principales resultados obtenidos durante el desarrollo del proyecto:

### features_merged

Archivos CSV y JSON con las características extraídas de las imágenes procesadas.

### forensic_reports_qwen_batches

Informes descriptivos generados automáticamente por el modelo multimodal.

### LLM evaluation

Resultados de la evaluación multimodal, incluyendo:

* Predicciones generadas.
* Métricas de precisión.
* Matrices de confusión.
* Gráficas utilizadas en la memoria.

## Bases de datos

Las bases de datos utilizadas durante el proyecto **no se incluyen en este repositorio** debido a restricciones de distribución y permisos de uso.

Concretamente se emplearon:

* HDA-IWBF-2023
* Tattoo-YOLO

Por este motivo, los notebooks se proporcionan únicamente como referencia del proceso experimental desarrollado.

## Memoria

El documento `EII-GCID-2026-06BlancoDavila_V` contiene la descripción completa del trabajo realizado, incluyendo:

* Objetivos.
* Metodología.
* Desarrollo experimental.
* Resultados obtenidos.
* Conclusiones y trabajos futuros.

## Autor

Víctor Blanco Dávila

Grado en Ciencia e Ingeniería de Datos

Universidad de Las Palmas de Gran Canaria
