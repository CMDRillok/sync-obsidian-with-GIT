**recall** считает отношение правильно угаданных ко всем **реальным** единицам.

Например, назовем в задаче диагностики классом 1 — больных. Оценим эти метрики для модели, которая всех считает больными.

ecall покажет `(правильно предсказанные больные) / (общее число реальных больных) = 1 / 1 = 1`.
$$
precision = \frac{TP}{TP + FN}
$$
[[TP (True Positive)]] [[FN (False Negative)]] [[точность модели]]

```python
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score
```

```python
# вычисляем значения метрик
recall = recall_score(y_test, y_pred)

# выводим результат
print(f"Recall: {recall:.2f}")

# вывод:
# Recall: 0.90
```