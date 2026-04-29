# 🌿 PlantVillage Classifier

> Clasificación automática de enfermedades en hojas de cultivos mediante redes neuronales convolucionales: un estudio comparativo.

**Proyecto final — Aprendizaje Máquina**

## 📖 Descripción

Este proyecto desarrolla un sistema de clasificación de imágenes capaz de identificar **38 enfermedades distintas en 14 cultivos** a partir de fotografías de hojas. La motivación nace del impacto económico que tienen las enfermedades vegetales en la agricultura mexicana, donde un diagnóstico temprano puede reducir significativamente las pérdidas.

## 🎯 Objetivo

Comparar el desempeño de cuatro arquitecturas de redes neuronales convolucionales (CNN básica, MobileNetV2, ResNet50, EfficientNetB0) sobre el dataset PlantVillage, evaluando precisión, eficiencia computacional e interpretabilidad mediante Grad-CAM.

## 🗂️ Dataset

- **Fuente:** [PlantVillage Dataset (Kaggle)](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset)
- **Tamaño:** ~54,000 imágenes
- **Clases:** 38 (combinaciones de planta + enfermedad o estado sano)
- **Plantas incluidas:** Manzano, arándano, cereza, maíz, uva, naranja, durazno, pimiento, papa, frambuesa, soya, calabaza, fresa y tomate.

## 🛠️ Tecnologías

- Python 3.10
- PyTorch / Torchvision
- Scikit-learn
- Matplotlib / Seaborn
- Gradio (demo)
- Google Colab (entrenamiento)

## 📁 Estructura del Repositorio

plantvillage-classifier/
├── notebooks/
│   ├── 01_EDA.ipynb              # Análisis exploratorio
│   ├── 02_preprocessing.ipynb    # Preprocesamiento y augmentation
│   ├── 03_baseline_cnn.ipynb     # CNN desde cero
│   ├── 04_transfer_learning.ipynb # MobileNet, ResNet, EfficientNet
│   └── 05_evaluation_gradcam.ipynb # Métricas y Grad-CAM
├── app/
│   └── gradio_app.py             # Demo interactiva
├── docs/
│   └── informe_tecnico.pdf       # Reporte completo
├── figuras/                      # Gráficas y resultados
├── requirements.txt
└── README.md

## 🚀 Cómo reproducir

1. Clonar el repositorio:
```bash
   git clone https://github.com/PMEXDOWNY/plantvillage-classifier.git
```
2. Abrir los notebooks en Google Colab (botón "Open in Colab" o subiendo el `.ipynb`).
3. Ejecutar en orden: `01_EDA → 02_preprocessing → 03_baseline_cnn → 04_transfer_learning → 05_evaluation_gradcam`.
4. Para probar la demo: visitar [HuggingFace Space — *próximamente*].

## 📊 Resultados (en construcción)

| Modelo | Accuracy | F1-Score | Tiempo de entrenamiento |
|---|---|---|---|
| CNN Baseline | TBD | TBD | TBD |
| MobileNetV2 | TBD | TBD | TBD |
| ResNet50 | TBD | TBD | TBD |
| EfficientNetB0 | TBD | TBD | TBD |

## 👥 Equipo

Grupo X — Materia de Aprendizaje Máquina

## 📜 Licencia

MIT License — ver archivo [LICENSE](LICENSE).
