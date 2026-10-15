# Informe — Challenge 1: datos y análisis exploratorio

## Calidad de datos
- Dimensiones: 178 filas y 14 columnas.
- Variables predictoras: 13; variable objetivo: `target`.
- Valores nulos: 0 en todas las columnas.
- Filas duplicadas exactas: 0.
- Clases del target: 0 (59), 1 (71), 2 (48).

## Preparación
- Split estratificado: 80 % entrenamiento (142 filas) y 20 % prueba (36 filas).
- Semilla: `random_state=42`.
- El conjunto de prueba se reserva para evaluación final; el EDA se hace únicamente con entrenamiento.

## Hallazgos del EDA sobre entrenamiento
1. Distribución de clases: clase 0 = 47 (33,1 %), clase 1 = 57 (40,1 %), clase 2 = 38 (26,8 %).
2. Promedio de `flavanoids` por clase: 0 = 2,93; 1 = 2,01; 2 = 0,78. Promedio de `color_intensity`: 0 = 5,48; 1 = 2,98; 2 = 7,39.
3. `total_phenols` y `flavanoids` tienen correlación positiva aproximada de 0,86; `flavanoids` y `od280/od315_of_diluted_wines`, aproximadamente 0,79.

## Archivos de salida
- `data/processed/train.csv`
- `data/processed/test.csv`
- `artifacts/data_contract.json`

Los hallazgos son descriptivos y no implican causalidad.
