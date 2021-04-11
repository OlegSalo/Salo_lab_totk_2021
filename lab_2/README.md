# Звіт із лабораторної роботи №2
---
### із дисципліни Теоретичні основи телекомунікацій
## Тема: *Представлення телекомунікаційних мереж у термінах теорії графів.*
---
## Мета роботи: *Навчитись представляти телекомунікаційні мережі за допомогою матриць суміжності, інцедентності та списку ребер, і оволодіти основними поняттями теорії графів.*

### Виконав: 
### Прийняв: 
---

### Виконання роботи
#### 1. Записати (придумати) матрицю суміжності орієнтованого графа G={7,12}. Ввести її у лабораторний макет та побудувати візуальне представлення графа.
![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_2/1.1.png)

0, 0, 1, 0, 1, 1, 0,
1, 0, 1, 0, 1, 0, 0,
1, 0, 0, 0, 1, 0, 0,
0, 1, 0, 0, 0, 1, 0,
1, 0, 1, 0, 0, 0, 0,
0, 0, 0, 1, 0, 0, 1,
1, 0, 0, 0, 1, 0, 0,

i. Чи є у побудованому графі ізольовані вершини або незв’язні компоненти? Tак - назвіть їх; Hі - які ребра потрібно видалити щоб вони утворились?
* Ні, щоб утворилась ізольована вершина потрібно: ребро, яке з’днює вершини 3 і 5, та ребро, яке іде від вершини 3 до вершини 1. Тоді вершина 3 буде ізольованою.

ii.	Чи є у графі вершини типу глухий кут? Так - то змінивши напрямок ребер чи можна це усунути; Hі - вкажіть цикл обходу всіх вершин;
* Ні. Цикл обходу вершин: 0=>2=>4=>6=>5=>3=>1

iii.	Чи існує в графі цикл обходу вершин (цикл Гамільтона)? Так - вкажіть послідовність вершин, що входять до даного циклу; Hі - що потрібно змінити в графі щоб даний цикл існував;
* Так: 0⇒5⇒3⇒1⇒2⇒6⇒4⇒0

iv.	Чи існує в графі цикл обходу ребер (цикл Єйлера); Так - вкажіть послідовність ребер, що входять до даного циклу; Hі - що потрібно змінити в графі щоб даний цикл існував;
* Ні. Для цього потрібно видаляти ребра до тих пір, поки не залишуться вершини, які зєднані не більше як із 2 ребрами, щоб ланцюг проходив кожне ребро рівно один раз.

v.	Побудувати доповнення (обернений) графа G.
* ![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_2/1.2.png)

0, 1, 0, 0, 1, 0, 1,
0, 0, 0, 1, 0, 0, 1,
0, 1, 0, 1, 0, 1, 0,
0, 0, 1, 0, 1, 0, 0,
0, 0, 0, 1, 0, 1, 1,
1, 1, 1, 0, 1, 0, 0,
0, 1, 0, 0, 0, 1, 0,

  
#### 2.	За допомогою лабораторного макету побудувати випадковий неорієнтований граф G={7,15} та записати його матрицю суміжності.

0, 1, 0, 1, 1, 1, 1,
1, 0, 1, 1, 1, 0, 0,
0, 1, 0, 1, 0, 1, 1,
1, 1, 1, 0, 1, 0, 1,
1, 1, 0, 1, 0, 1, 0,
1, 0, 1, 0, 1, 0, 1,
1, 0, 1, 1, 0, 1, 0,


i.	Як зміниться топологія графа (структурні зв’язки), якщо циклічно зсунуту вправо 2 стовпці у матриці суміжностей?
* Граф буде частково орієнтованим і змінить розташування вершин

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_2/2.3.png)

ii.	Як зміниться топологія графа (структурні зв’язки), а) Якщо всі елементи над діагоналлю перетворити в 1? б) Якщо всі елементи під діагоналлю перетворити в 0?
* а) граф орієнтується, стрілки вказують від меншої до більшої вершини
* б)граф орієнтується, стрілки вказують від більшої до меншої вершини

#### 3.	За допомогою лабораторного макету побудувати випадковий орієнтований граф G={5,10} та записати його матрицю відповідностей (інцедентності).

![image](https://github.com/OlegSalo/Salo_lab_totk_2021/blob/main/lab_2/3.1.png)

1, 1, 0, -1, 0, 0, 0, -1, 0
-1, 0, 0, 0, 1, 0, 0, 0, -1
0, 0, 0, 0, 0, -1, 1, 1, 1
0, 0, -1, 1, 0, 0, -1, 0, 0
0, -1, 1, 0, -1, 1, 0, 0, 0


i.	Як з матриці відповідностей можна визначити ступінь кожної вершини?
* Ступінь вершини визначається кількістю одиничок у рядку матриці.

#### 4.	Задано граф G та M.
G={(5,1), (6,1), (2,3), (3,4), (2,6), (3,6), (5,6), (1,7), (2,7), (3,7), (4,7), (6,7)}
M={(2,1), (5,1), (1,2), (4,2), (5,2), (6,2), (2,4), (5,4), (6,4), (1,5), (2,5), (4,5), (6,5), (2,6), (4,6), (5,6)}
Визначте для кожного з графів:
ii.	Графи орієнтовані чи неорієнтовані?
* G - орієнтований, а M - не орієнтований.

iii.	Яка кількість вершин V та ребер E?
* У G - Вершин 7, ребер 12. У М - 6 вершин та 8 ребер.

iv.	Яка з вершин має найбільшу ступінь? Скільки?
* У G - Вершина 2 і вершина 3 мають по 3 ступені. У М - вершина 2 та 5 мають ступені 4.

v.	Визначте ексцентриситети вершин для графа G та M.
* У G - 2. У M - 2

vi.	Який радіус кожного з графів?
* У G - Радуис граф: 1 (1⇒7). У M - Граф не є звязним.

vii.	Який діаметр кожного з графів?
* У G - Диаметр граф: 2 (2⇒6⇒1). У M - Граф не є звязним.

viii.	Чи містять графи петлі (елементарні цикли)? Вкажіть послідовність ребер.
* У G - Ні. У M - Ні

ix.	Чи містять графи ізольовані вершини?
* У G - Ні. У M - Так, вершина 3.

x.	При транспонування G та M чи змінюється графічне представлення графа? Як?
* Орієнтація змінюється в протилежному напрямку