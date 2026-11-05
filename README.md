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

## Ejecución

Instalar las dependencias indicadas en `requirements.txt`, abrir el notebook correspondiente en Jupyter o Colab y ejecutar todas las celdas en orden. Mantener el ZIP Properati en la raíz del repositorio. EV2 busca primero el CSV preparado de EV1; si no existe, reconstruye la limpieza final desde el ZIP.

EV2 utiliza muestras reproducibles de hasta 12.000 registros para regresión y 8.000 para clasificación por el costo computacional de KNN y SVM. La validación cruzada utiliza submuestras de entrenamiento. Los CSV generados son archivos de trabajo y no es necesario versionarlos.
