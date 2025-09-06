Эта метрика считает, как часто мы правильно угадываем ответ — независимо от класса. Для задачи диагностики больных это не самая удачная метрика: она покажет 99% точности для модели, которая всех считает здоровыми.

Но для данных, где классы распределены равномерно, она очень удобная.
Формула метрики:
$$
accuracy = \frac{TP + TN}{TP + TN + FP + FN} 
$$
[[TP (True Positive)]] [[TN (True Negative)]] [[FP (False Positive)]] [[FN (False Negative)]] [[точность модели]]
```python
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score
```

```python


# вычисляем значения метрик
accuracy = accuracy_score(y_test, y_pred)


# выводим результат
print(f"Accuracy: {accuracy:.2f}")


# вывод:
# Accuracy: 0.95

```
