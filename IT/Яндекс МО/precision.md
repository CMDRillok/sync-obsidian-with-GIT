**precision** считает отношение правильно угаданных единиц ко всем **предсказанным** единицам

Например, назовем в задаче диагностики классом 1 — больных. Оценим эти метрики для модели, которая всех считает больными.

Precision покажет `(правильно предсказанные больные) / (общее число предсказанных больных) = 1 / 100 = 0.01`.
$$ 
precision = \frac{TP}{TP + TF}
$$
[[TP (True Positive)]] [[FP (False Positive)]] [[точность модели]]

```python
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score
```

```python
# вычисляем значения метрик
precision = precision_score(y_test, y_pred)

# выводим результат
print(f"Precision: {precision:.2f}")

# вывод:
# Precision: 1.00
```