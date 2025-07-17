# 📊 Dataset Benchmark: SportsMOT vs DeepSportRadar

Este repositorio contiene un análisis comparativo entre dos datasets de visión por computador centrados en deportes:

- [`SportsMOT`](https://github.com/MCG-NJU/SportsMOT)
- [`DeepSportRadar`](https://github.com/DeepSportradar)

El objetivo es evaluar la calidad, aplicabilidad y desempeño de ambos datasets bajo tareas como:
- Re-identificación de jugadores
- Seguimiento (tracking) multiobjeto
- Segmentación de instancias

---

## 📁 Estructura del Repositorio

---

---

## 📦 Datasets Comparados

### 🔹 [SportsMOT](https://github.com/MCG-NJU/SportsMOT)
- Tipo: Multi-Object Tracking (MOT)
- Tamaño: 139 secuencias de video (≈273K anotaciones)
- Modalidades: Visión monocular RGB
- Etiquetas: PlayerID, balón, poses, orientación
- Licencia: Uso no comercial
- Enfoque: Precisión en entornos multijugador y desafíos con oclusiones

### 🔹 [DeepSportRadar](https://github.com/DeepSportradar/)
- Submódulos:
  - **Re-identificación**: Tareas de seguimiento entre cámaras
  - **Segmentación**: Anotaciones precisas a nivel de píxel
- Modalidades: Multicámara, RGB, segmentación y bounding boxes
- Licencia: Uso académico / con restricciones (consultar repositorio)
- Enfoque: Datos enriquecidos y escenarios reales de competición

---

## 🔬 Criterios de Comparación

Los datasets serán evaluados usando los siguientes factores:

| Factor                        | Descripción                                                                 |
|------------------------------|-----------------------------------------------------------------------------|
| Tamaño y variedad            | Número de videos, frames y diversidad de escenarios                         |
| Calidad de anotaciones       | Precisión de bounding boxes, segmentación y etiquetas                       |
| Escenarios cubiertos         | Baloncesto indoor/outdoor, oclusiones, multijugador                         |
| Formato y accesibilidad      | Facilidad de uso, estándares, licencias                                     |
| Métricas de evaluación       | Aplicación de mAP, MOTA, MOTP, IDF1, etc.                                   |
| Compatibilidad con modelos   | Facilidad para usar con YOLO, DeepSORT, Detectron2, etc.                    |

---

## 🛠️ Dependencias Recomendadas

- Python 3.10+
- OpenCV
- Pandas
- Matplotlib / Seaborn
- Jupyter (opcional)

---

## 🚀 Cómo empezar

```bash
# Clona el repositorio con los submódulos
git clone --recurse-submodules https://github.com/tu_usuario/Dataset-Benchmark.git

# Entra al directorio
cd Dataset-Benchmark

# Instala las dependencias necesarias
pip install -r requirements.txt
