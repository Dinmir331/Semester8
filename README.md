#   Лабораторная работы №1 по дисциплине "Системы копьютерного зрения"
# Фильтрация изображений
##  Задания
&ensp; Применить методы обработки изображений:
1. Выполнить свертку изображения
2. Применить морфологические операции: эрозию и дилатацию
3. Применить 2 фильтра: фильтр Гаусса и медианный фильтр
4. Применить бинаризацию и корректировку освещенности к изображению


### Дополнительная информация
&ensp; В качестве среды выполнения был выбран сервис Colab, так как имеется опыт работы в данной системе. 

&ensp; В качестве тестового изображения был взят цветной мем размерностью 351x400 (длина; высота), файл носит название MEM_OPEN_CV.jpg .

&ensp; В файлах данного репрезитория можно найти файл с сервиса Colab, содержащий в себе весь проект (название LB_vizhen.ipynb).

&ensp; В папке Image хранятся изображения, используемые в данном файле README для демонстрации результатов работы фильтров.

##  Размерность итогового и начального изображения

##  Размерность итогового и начального изображения

  
  
## Общий алгоритм работы
  &ensp;В проекте каждый фильтр реализован в своём независимом блоке, что упрощает работу с проектом и позволяет независимо друг от друга надстраивать фильтры. Все этапы обработки изображения от его растягивания до конечной свёртки прописаны индивидуально в каждом блоке.

  &ensp;После загрузки изображения, происходит его разбивка на три цветовых канала (BRG), что позволяет получить три матрицы изображения в оттенках серого (однако, под серым подрузамевается цвет цветового канала).

  &ensp;Фильтр применяется к каждому каналу изображения, после чего информация с канналов суммируется и обратно превращается в системиу RGB, что позволяет востановить обычное цветное изображение

## Фильтры
### Эрозия


![alt text](Image/Эрозия.png)

### Диалотация


![alt text](Image/Дилатация.png)

### Медианный

![alt text](Image/Медианый.png)

### Гаусовый


![alt text](Image/Гаусовый.png)

### Корректировка освещения (коэффициент)


![alt text](Image/Коэффициент.png)

### Корректировка освещения (гамма)

![alt text](Image/Гамма.png)

### Бинаризация


![alt text](Image/Бинаризация.png)

##  Результаты работы

&ensp; В рамках данной работы были изучены теорретически и реализованы в коде фильтры изображений, согласно поставленной задачи. Были созданы материалы, показывающие этапы работы фильтров, а так же позволяюще сравнить начальное и обработанное изображение после применения каждого из фильтров.

&ensp; Все результаты работы были оформлены в проекте на платформе GitHub, при этом сам код фильтров был реализован на платформе Colab (файл с кодами содержится в репрезитории на GitHub).










