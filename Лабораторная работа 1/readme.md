# **Лабораторная работа №1**
*Цель работы:*
- Разработать функцию сортировки списка вставками
- Провести эксперимент - как растёт время сортировки при росте количества элементов n
- В своём репозитории с помощью разметки markdown создать краткое описание вашей функции сортировки
- В описание добавить таблицу с данными роста времени исполнения с помощью специальной разметки markdown
-—
## **Сортировка вставкой**
Сортировка вставками (англ. Insertion sort) — алгоритм сортировки, в котором элементы входной последовательности просматриваются по одному, и каждый новый поступивший элемент размещается в подходящее место среди ранее упорядоченных элементов[1]. Вычислительная сложность — O ( n 2 ) O(n^{2}).
### **Фрагмент алгоритма**
```py
def sort():
for i in range(len(lst) - 1, -1, -1):
n = lst[i] # берем элемент из списка
g = i+1
while g<=len(lst) - 1 and n<lst[g]:
lst[g-1] = lst[g]
print(lst)
g += 1 # передвигаем элемент для следующего сравнения
lst[g-1] = n # убирает
print(lst)
```
### **Проведение опыта**
После разработки и проверки алгоритма были получены следующие результаты:
|Количество элементов (ед.) |Время выполнения программы (с.)|
|----------|-----------|
|100 |0.001 |
|1000 |0.216 |
|2500 |0.742 |
|5000 |6.972 |
|10000 |29.078 |
-—
***
---
