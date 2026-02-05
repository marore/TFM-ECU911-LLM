# TFM: Clasificación y generación inteligente de respuestas en diálogos de emergencias ECU911

Trabajo Fin de Máster en Análisis y Visualización de Datos Masivos  
**Autor:** Marcos Orellana Cordero  
**Universidad:** Universidad Internacional de La Rioja (UNIR)  
**Fecha:** Febrero 2026

## Resumen

El presente estudio propone una metodología integral para optimizar la gestión conversacional en centros de comando y control de emergencias, utilizando como caso de estudio el sistema ECU911. Mediante un proceso secuencial que combina técnicas avanzadas de Procesamiento del Lenguaje Natural y Large Language Models, se abordan cuatro etapas principales: preprocesamiento exhaustivo del corpus de diálogos con etiquetado manual de actores y actos conversacionales, extracción de entidades nombradas (NER), etiquetado morfosintáctico (POS) y representación TF-IDF; inferencia eficiente con vLLM para generar resúmenes por turno, palabras clave y clasificación de subactos, seguida de anonimización y limpieza; reducción semántica de las intervenciones del operador mediante prompting estructurado con LLM, generando preguntas canónicas y eliminando redundancias contextuales; y, finalmente, ajuste fino de un modelo BERT para la clasificación supervisada de actos de diálogo y niveles de severidad, complementado con estrategias de retrieval aumentado. Los resultados evidencian mejoras sustanciales en precisión, eficiencia y capacidad de captura de dependencias conversacionales complejas en entornos de alta presión temporal y emocional, reduciendo significativamente la carga cognitiva del operador humano y acelerando la toma de decisiones críticas. Esta contribución avanza en la analítica conversacional aplicada a emergencias, ofreciendo un framework reproducible, escalable y orientado a la mejora operativa de sistemas de atención ciudadana 911, cuyo código fuente, datasets anonimizados de muestra y documentación detallada se ponen a disposición en el presente repositorio para facilitar su reproducción, validación y extensión en contextos similares.

## Estructura del repositorio

- `notebooks/` → Etapas del pipeline (preprocesamiento, inferencia, fine-tuning)
- `data/` → Datasets anonimizados de muestra

## Requisitos

```bash
pip install -r requirements.txt
