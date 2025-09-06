**F1-score** находит баланс между [[precision и recall]]. Вычисляется она так:
$$
F1 = \frac{2 * precision * recall}{precision + recall}
$$
[[precision]] [[recall]] [[точность модели]]

```python
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score
```

```python
# вычисляем значения метрик
f1 = f1_score(y_test, y_pred)

# выводим результат
print(f"F1: {f1:.2f}")

# вывод:
# F1: 0.95
```