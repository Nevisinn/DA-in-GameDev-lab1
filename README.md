# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #1 выполнил(а):
- Шубин Игорь Васильевич
- РИ210941
Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | * | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Структура отчета

- Данные о работе: название работы, фио, группа, выполненные задания.
- Цель работы.
- Задание 1.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 2.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 3.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Выводы.
- ✨Magic ✨

## Цель работы
Ознакомиться с основными операторами зыка Python на примере реализации линейной регрессии.

## Задание 1
Написать программы Hello World на Python и Unity
На Python
![изображение](https://user-images.githubusercontent.com/38161044/192271126-baebc0ae-4b4a-4bd6-bc38-8a7bc5a09b95.png)
![изображение](https://user-images.githubusercontent.com/38161044/192271171-a92ef185-f62b-40e1-91a5-ddd0e2bee8cf.png)
На Unity
![изображение](https://user-images.githubusercontent.com/38161044/192271209-e6cd037e-6731-42b5-882b-54b2e193d952.png)

## Задание 2
### Пошагово выполнить каждый пункт раздела "ход работы" с описанием и примерами реализации задач
Ход работы:
- Произвести подготовку данных для работы с алгоритмом линейной регрессии. 10 видов данных были установлены случайным образом, и данные находились в линейной зависимости. Данные преобразуются в формат массива, чтобы их можно было вычислить напрямую при использовании умножения и сложения.

```py

In [ ]:
#Import the required modules, numpy for calculation, and Matplotlib for drawing
import numpy as np
import matplotlib.pyplot as plt
#This code is for jupyter Notebook only
%matplotlib inline

# define data, and change list to array
x = [3,21,22,34,54,34,55,67,89,99]
x = np.array(x)
y = [2,22,24,65,79,82,55,130,150,199]
y = np.array(y)

#Show the effect of a scatter plot
plt.scatter(x,y)

```

- Определите связанные функции. Функция модели: определяет модель линейной регрессии wx+b. Функция потерь: функция потерь среднеквадратичной ошибки. Функция оптимизации: метод градиентного спуска для нахождения частных производных w и b.
	
![изображение](https://user-images.githubusercontent.com/38161044/192272666-1b36dff0-8ebd-4e97-8e52-f1ac782f2892.png)
3. Начать итерацию 
Шаг 1. Инициализация и модель итеративной оптимизации
![изображение](https://user-images.githubusercontent.com/38161044/192272892-6818c367-809a-4bf9-a6ec-9db7b6b19a56.png)
Шаг 2. На второй итерации отображаются значения параметров, значения потерь и эффекты визуализации после итерации
![изображение](https://user-images.githubusercontent.com/38161044/192272921-59138a52-2d70-4892-8833-75bc3fe90098.png)
Шаг 3 Третья итерация показывает значения параметров, значения потерь и эффекты визуализации после итерации
![изображение](https://user-images.githubusercontent.com/38161044/192272946-2493d5f3-c46b-4b06-b243-6357602e7427.png)
Шаг 4 Четвертая итерация показывает значения параметров, значения потерь и эффекты визуализации после итерации
![изображение](https://user-images.githubusercontent.com/38161044/192272968-3622fe5b-cc0c-4070-96df-188ce1e1fcb1.png)
Шаг 5. Пятая итерация показывает значения параметров, значения потерь и эффекты визуализации после итерации
![изображение](https://user-images.githubusercontent.com/38161044/192275432-402bffca-4f54-4e13-9d4f-60d2f3d463db.png)
Шаг 6. 10000-ая итерация, показывающая значения параметров, потери и визуализацию посел итерации

## Задание 3
### Должна ли величина loss стремиться к нулю при изменении исходных данных? Ответьте на вопрос, приведите пример выполнения кода, который подтверждает ваш ответ.
Величина loss должна стремиться к нулю.

![изображение](https://user-images.githubusercontent.com/38161044/192311299-d4ee0cee-002b-44b0-b19a-c2c38e0c98e4.png)
![изображение](https://user-images.githubusercontent.com/38161044/192311315-60af2c98-1d51-4e18-8028-572a3d86b8d8.png)
![изображение](https://user-images.githubusercontent.com/38161044/192312955-868ea81c-cf24-48c5-82a4-7007b08ffa4d.png)
![изображение](https://user-images.githubusercontent.com/38161044/192312998-b3602ea1-517a-4914-86c0-2a0e88515548.png)
![изображение](https://user-images.githubusercontent.com/38161044/192313767-0457c613-a3f3-4dff-b5ab-ccce2c21275f.png)
![изображение](https://user-images.githubusercontent.com/38161044/192313807-8d879751-91fd-4de4-9f6c-b7ec02a031e0.png)

### Какова роль параметра Lr? Ответьте на вопрос, приведите пример выполнения кода, который подтверждает ваш ответ. В качестве эксперимента можете изменить значение параметра.

Lr - угловой коэффициент прямой. 
Lr = 0.00009

![изображение](https://user-images.githubusercontent.com/38161044/192316045-cc7a2fc7-cf83-49f0-8d42-14d4a5ddb816.png)

Lr = 0.000027

![изображение](https://user-images.githubusercontent.com/38161044/192316192-cadea826-f0d8-46c9-9e42-24f31d295476.png)

## Выводы

Ознакомился с основными операторами зыка Python на примере реализации линейной регрессии и написал программы Hello World на Python и Unity.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
