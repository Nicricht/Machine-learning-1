# Machine Learning - Evaluaciones Parciales 1 y 2

Repositorio de MLY0100 Machine Learning. El proyecto utiliza Properati y la metodología CRISP-DM.

## Evaluación Parcial 1

- Enunciado y guía de EV1.
- `notebook/evaluacion_parcial_1.ipynb`: fases 1, 2 y 3 de CRISP-DM.
- `Evaluación Parcial 1 - Dataset.zip`: dataset original.
- Al ejecutar EV1 se genera `DS1-18-Datos-Properati-preparado.csv`.

## Evaluación Parcial 2

- `notebook/evaluacion_parcial_2.ipynb`: fases 4 y 5 de CRISP-DM.
- Regresión: `price`, con regresión lineal múltiple y KNN Regressor.
- Clasificación: `property_type` agrupada en Departamento, Casa, PH y Otros; se comparan Regresión Logística, KNN, SVM y Decision Tree.
- Evaluación: MAE, RMSE, R², accuracy, precision, recall, F1, ROC-AUC multiclase, matrices de confusión y validación cruzada.
- Balance: RandomOverSampler solo sobre entrenamiento.

## Evaluación Parcial 2: abrir o ejecutar en Google Colab

**Opción 1 (ver los resultados):** abrir el notebook desde [Google Colab](https://colab.research.google.com/github/Nicricht/Machine-learning-1/blob/evaluacion-parcial-2/notebook/evaluacion_parcial_2.ipynb). Las tablas, las métricas, los gráficos y las explicaciones están guardados en el archivo, por lo que pueden revisarse sin ejecutar el código.

**Opción 2 (ejecutar todo de nuevo):** en ese mismo notebook seleccionar **Entorno de ejecución → Ejecutar todas**. La primera celda de configuración comprueba las librerías necesarias y, cuando no está disponible localmente, descarga automáticamente el ZIP Properati desde este repositorio público. Luego EV2 reconstruye la limpieza final de EV1 y calcula de nuevo los resultados. **No hace falta importar manualmente el dataset** en un entorno Colab con acceso a internet.

El notebook usa una muestra de hasta 12.000 observaciones para regresión y 8.000 para clasificación, por lo que ejecutar los modelos puede requerir recursos de cómputo y varios minutos. Para ejecución local también se pueden instalar las dependencias con `pip install -r requirements.txt`. El workflow `validate-ev2.yml` comprueba la ejecución sin el ZIP precargado para cubrir el caso de un entorno nuevo.

EV2 utiliza muestras reproducibles de hasta 12.000 registros para regresión y 8.000 para clasificación por el costo computacional de KNN y SVM. La validación cruzada utiliza submuestras de entrenamiento. Los CSV generados son archivos de trabajo y no es necesario versionarlos.
