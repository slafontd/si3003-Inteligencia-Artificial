# Challenge 3 — Evaluación final e inferencia

- **Modelo campeón:** LogisticRegression
- **Accuracy CV:** 97.91%
- **Accuracy test:** 97.22%
- **F1 macro test:** 97.10%
- **Tamaño de test:** 36 registros

## Interpretación
El resultado de test es cercano al de validación cruzada. La matriz de confusión es:
[[12, 0, 0], [0, 14, 0], [0, 1, 9]]

Una observación de la clase 2 fue clasificada como clase 1. No hay evidencia clara de sobreajuste a partir de esta comparación aislada; el test es pequeño (36 observaciones), por lo que existe incertidumbre.

## Archivos generados
- `reports/test_metrics.json`
- `reports/batch_predictions.csv`
- `artifacts/champion_model.joblib`
