# Automatización y predicción de presupuestos en la industria de automoción mediante Machine Learning
Repositorio del Trabajo de Fin de Máster (TFM) centrado en el desarrollo de un sistema de presupuestación técnica de piezas plásticas por inyección, que combina la automatización de cálculos técnicos con modelos de predicción de precios basados en técnicas de Machine Learning.

Autor: Ana Rodríguez Rubio

## Estructura de los ficheros

notebooks

- `01_calculo_precios.ipynb`: Automatiza el cálculo del coste y precio final de cada pieza a partir de sus datos técnicos y económicos.
- `02_generar_historico.ipynb`: Genera un histórico de piezas con precios calculados para entrenar modelos predictivos.
- `03_prediccion_nuevas_piezas.ipynb`: Aplica un modelo de regresión entrenado para estimar el precio de nuevas piezas usando únicamente variables técnicas.
- `04_comparacion_precios.ipynb`: Compara los precios estimados por el modelo con los precios calculados mediante el sistema técnico.


data

- `datos_piezas.csv`: Fichero con las características técnicas de las piezas.
- `tarifas_costes.xlsx`: Fichero con las tarifas de materiales, máquinas y parámetros generales.
- `nuevas_piezas.csv`: Fichero con las características técnicas de nuevas piezas para realizar predicciones.

otros

- `requirements.txt`: Fichero con los paquetes (y versiones) necesarios para ejecutar el código.


## Requisitos

Instalar mediante:

pip install -r requirements.txt



## Pasos a seguir

1. Ejecutar `01_calculo_precios.ipynb` para calcular automáticamente los precios técnicos con las tarifas conocidas.
2. Ejecutar 02_generar_historico.ipynb para crear un dataset histórico que sirva como base para entrenar modelos predictivos.
3. Entrenar y aplicar el modelo con 03_prediccion_nuevas_piezas.ipynb, utilizando únicamente los datos técnicos de las nuevas piezas.
4. Comparar los resultados del modelo con el cálculo técnico exacto mediante 04_comparacion_precios.ipynb.

