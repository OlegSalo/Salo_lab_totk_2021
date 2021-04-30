# Звіт із лабораторної роботи №3
---
### із дисципліни Теоретичні основи телекомунікацій
## Тема: *Методи обходу та модифікації графів.*
---
## Мета роботи: *Навчитись застосовувати алгоритми обходу графів, побудови дерева шляхів та мінімального зв’язного дерева.*

### Виконав: студент групи *ТР-32* Сало О.I
### Прийняв: викладач Бугиль Б.А.
---

### Виконання роботи
#### 1.	За допомогою лабораторного макету побудувати випадковий неорієнтований граф G={8,12}:

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.1.png)

i.	Побудувати дерево за алгоритмом обходу в ширину (BFS); (для 2-х різних вершин)
* Для вершини 0 порядок обходу: 0 1 2 6 4 5 7 3

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.2.png)

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.3.png)

* Для вершини 5 порядок обходу: 5 2 4 0 6 7 3 1

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.4.png)

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.5.png)

ii.	Чи будуть однаковими топології дерев побудованих з різних кореневих вершин? Чому?
* Так, тому що на виході із вершини 0 і 5 корінь в обох має по дві вершини.

iii.	Побудувати дерево за алгоритмом обходу в глибину (DFS); (для 2-х різних вершин)
* Для вершини 7 порядок обходу: 7 2 0 1 6 3 4 5

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.6.png)

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.7.png)

* Для вершини 6 порядок обходу: 6 1 0 2 4 3 7 5

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.8.png)

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.9.png)

iv.	Чи будуть однаковими топології дерев побудованих з різних кореневих вершин? Чому?
* Ні, тому що у другому графі вершина 4 у своєму подальшому послідовному корені вершин 3-7 потрапила у глухий кут і їй довелось вернутись, так як ще одна вершина не була знайдена.

#### 2.	За допомогою лабораторного макету побудувати випадковий орієнтований граф G={6,10}:

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.10.png)

i.	Побудувати дерево за алгоритмом обходу в ширину (BFS);
* Порядок обходу:  0 1 5 2 3 4

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.11.png)

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.12.png)

ii.	Яка вершина (вершини) буде знайдена останньою?
* Вершина 4

iii.	Визначити чи існують цикли. Вказати послідовність ребер і їх довжину.
* Цикли: Немає циклів.

iv.	Визначити кількість хвиль, які пройдуть по ребрах доки буде виявлена остання вершина.
* Кількість хвиль становить 5.

v.	Побудувати дерево за алгоритмом обходу в глибину (DFS);
* Порядок обходу: 0 1 5 2 3 4

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.13.png)

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.14.png)

#### 3.	Побудувати дерево шляхів рангом r=4 для випадкового графа G={6,9}.

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.15.png)


![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.16.png)


#### 4.	Побудувати мінімальне зв’язне дерево для графа G. Вказати його вагу.

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.#4.1.png)


![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_3/3.17.png)

* Вага: 5+7+9+3+5=29
