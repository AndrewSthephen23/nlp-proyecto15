# Proyecto 15: Implementación de HMM y Algoritmo de Viterbi con Ejemplo de POS-Tagging

## Objetivo

El objetivo de este proyecto es construir desde cero un **Hidden Markov Model (HMM)** de primer orden para el etiquetado de partes de habla (**POS-tagging**) y aplicar el **algoritmo de Viterbi** con **backpointers** para encontrar la secuencia más probable de etiquetas para un conjunto de palabras. El proyecto incluye un ejemplo práctico paso a paso utilizando el **Brown Corpus** para demostrar el funcionamiento del modelo y el algoritmo.

## Descripción del Proyecto

Este proyecto implementa un **Modelo Oculto de Markov (HMM)** de primer orden y el **algoritmo de Viterbi**, el cual es utilizado para resolver tareas de etiquetado de partes de habla (POS-tagging). La tarea consiste en predecir la etiqueta gramatical (sustantivo, verbo, adjetivo, etc.) de cada palabra en una oración.

La implementación incluye los siguientes componentes:

- **HMM**: El modelo se entrena utilizando secuencias de palabras etiquetadas, donde las probabilidades de transición entre etiquetas y las probabilidades de emisión (de palabra a etiqueta) son aprendidas.
- **Algoritmo de Viterbi**: Este algoritmo es utilizado para encontrar la secuencia más probable de etiquetas para una secuencia dada de palabras observadas.

## Estructura del Proyecto

```
nlp-proyecto15/
├── src/
├── notebooks/
│   ├── CorpusBrown.ipynb          # Ejemplo del uso del corpus Brown para entrenamiento y etiquetado de palabras
│   ├── PrimerProtipo.ipynb        # Prototipo de un HMM aprendiendo la teoria
│   └── PrototipoViterbi.ipynb     # Ejecución del algoritmo de Viterbi paso a paso 
├── results/                   
├── README.md                      # Documentación del proyecto
└── requirements.txt               # Librerías necesarias para ejecutar el proyecto (como numpy, nltk, etc.)

```

## Instalación

### Requisitos

Para ejecutar este proyecto, es necesario tener Python 3.x instalado, así como las siguientes librerías:

- `numpy`
- `nltk`

Puedes instalar las librerías necesarias ejecutando:

```bash
pip install -r requirements.txt
```

### Ejecución

1. **Preprocesamiento de datos**:
    
    En el archivo `CorpusBrown.ipynb`, puedes cargar el **Brown Corpus** de **NLTK** y visualizar las oraciones y etiquetas correspondientes comparando las etiquetas predichas con las reales.
    
2. **Entrenamiento del modelo**:
    
    El archivo `PrimerProtipo.ipynb` muestra cómo se implementa el HMM de primer orden y cómo se calculan las probabilidades de transición y emisión.
    
3. **Aplicación del algoritmo de Viterbi**:
    
    En `PrototipoViterbi.ipynb`, se ejecuta el algoritmo de Viterbi sobre el Primer Prototipo para etiquetar las palabras. 
    

---

## Créditos

Este proyecto es parte de la **práctica calificada 1 del curso CC0C2**.