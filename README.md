# TFG — Técnicas de ensamblado para la estimación de la probabilidad de impago

Código del Trabajo de Fin de Grado *"Técnicas de ensamblado en aprendizaje
automático supervisado. Un análisis comparativo en la estimación de la
probabilidad de impago."*

**Autor:** Fernando Fernández Picón
**Tutor:** Carlos Enrique Carleos Artime
**Grado en Matemáticas — Universidad de Oviedo**

## Descripción

Este repositorio contiene el desarrollo experimental del trabajo, en el que se
comparan distintos modelos de clasificación binaria (regresión logística, k-NN
y árboles de decisión) frente a diversas técnicas de ensamblado (bagging,
Random Forest, AdaBoost, Gradient Boosting, voting y stacking) sobre un problema
de riesgo de crédito.

## Datos

Se utiliza el *Credit Risk Dataset*, disponible públicamente en Kaggle:
https://www.kaggle.com/datasets/laotse/credit-risk-dataset

El conjunto recoge 32.581 préstamos descritos por 11 variables predictoras y
una variable objetivo binaria (`loan_status`), que indica si el préstamo
terminó en impago.

## Contenido

- `Credit_Risk_Dataset.ipynb` — notebook con todo el flujo: preprocesamiento,
  ajuste de hiperparámetros por validación cruzada y comparativa de modelos.

## Requisitos

- Python 3.x
- numpy, pandas, matplotlib, scikit-learn

Instalación de dependencias:

    pip install numpy pandas matplotlib scikit-learn

## Cómo ejecutarlo

1. Descargar el conjunto de datos desde el enlace de Kaggle y colocarlo en la
   carpeta del proyecto.
2. Abrir `Credit_Risk_Dataset.ipynb` con Jupyter y ejecutar las celdas en orden.

> Los resultados son reproducibles gracias al uso de una semilla aleatoria fija
> en la partición y en la validación cruzada.
