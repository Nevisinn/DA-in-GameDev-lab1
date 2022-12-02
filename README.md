# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #4 выполнил(а):
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
- Задание 3.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Выводы.
- ✨Magic ✨

## Цель работы
Интеграция экономической системы в проект Unity и обучение ML-Agent

## Задание 1
В проект Unity интегрировать экономическую систему,обучить ML-Agent, установить tensorflow и построить графики.
Обучение Ml-Agent
![Обучаем нейросеть](https://user-images.githubusercontent.com/38161044/205340948-778fd33c-e17e-4be9-b6f8-368b3182ff09.PNG)
Получаем такие графики
![получил такие графики](https://user-images.githubusercontent.com/38161044/205340991-1acb7e1b-909e-4c62-9463-945e37a66ef6.PNG)

## Задание 2
Измените параметры файла. yaml-агента и определить какие параметры и как влияют на обучение модели.

Уменьншил learning_rate до 0.5e-4 - коэффициент скорости обучения и получил такие графики. Модель стала обучаться дольше.
![изображение](https://user-images.githubusercontent.com/38161044/205341708-eb990b63-4046-4f9d-a4c4-af745a649e65.png)
![изображение](https://user-images.githubusercontent.com/38161044/205341915-75bd0942-84c8-4513-9d3d-93b812e40656.png)
![изображение](https://user-images.githubusercontent.com/38161044/205341947-b0e629c8-ca46-40b2-9e03-f2ebb1b18561.png)
![изображение](https://user-images.githubusercontent.com/38161044/205341964-716b43bb-55df-4f1b-901f-47bf98e1e390.png)

Увеличил epsilon до 0,3. Он влияет на то, насколько быстро политика может развиваться во время обучения. Соответствует допустимому порогу расхождения между старой и новой политикой при обновлении градиентного спуска. По итогу обучение происходит быстрее, но стабильность падает.
![изображение](https://user-images.githubusercontent.com/38161044/205342394-be8e0c11-7402-4ef1-b3ce-4060e98a0a1d.png)
![изображение](https://user-images.githubusercontent.com/38161044/205342408-fa3761bd-3ae5-4fa1-ab01-0066b2e3c3a2.png)
![изображение](https://user-images.githubusercontent.com/38161044/205342419-28c92e5a-6d49-4310-946c-f07fda8aa52b.png)
![изображение](https://user-images.githubusercontent.com/38161044/205342428-084ff04c-9852-4dbb-a05b-ee90e8a9554d.png)
![изображение](https://user-images.githubusercontent.com/38161044/205342450-f23a7ca8-b44c-4584-9d21-63839ea3b768.png)
![изображение](https://user-images.githubusercontent.com/38161044/205342466-6feca4d5-51f3-4177-b2ab-c79d43cb7ee2.png)
![изображение](https://user-images.githubusercontent.com/38161044/205342476-36dc196c-ed42-4d29-874d-72eac6165424.png)
![изображение](https://user-images.githubusercontent.com/38161044/205342488-f39ff9fd-4297-4abf-8328-c1760a05c05c.png)
![изображение](https://user-images.githubusercontent.com/38161044/205342513-7651a921-8502-40f0-8cbe-292906ad11ad.png)
![изображение](https://user-images.githubusercontent.com/38161044/205342545-845c068a-72fc-4088-87f5-fa51cd9aec75.png)

Увеличил num_epoch до 10 - количество эпох обучения. Чем больше значение, тем график становится все более нестабильным. 
![изображение](https://user-images.githubusercontent.com/38161044/205343040-3b01a5d4-16ec-4a36-b918-788d85ec7714.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343050-a6b49070-d596-4503-9edc-2f31c6debe50.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343059-6183a11e-ffd0-4c3e-ad84-4e4249f8d432.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343072-c7a1a2ad-3455-4a85-afb6-379bdb77ac4b.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343083-08528df7-250a-4242-97e7-2463e94d51a0.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343101-bdffb3c4-bfe5-4eb4-8656-76e970533a63.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343112-d6f83c64-3fd3-4188-bc6d-28cef5339858.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343123-ad2eb31d-e866-4f02-98bd-755bfc61ffb4.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343131-5c8a22dc-5536-4d22-bb6d-f0cf90209d31.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343140-5d07f974-e256-4a4a-ab11-43232582d20f.png)

Уменишил beta до 1.0e-4 - Сила энтропийной регуляризации, которая делает политику «более случайной». Чем меньше параметр, тем меньше действий совершают агенты.
![изображение](https://user-images.githubusercontent.com/38161044/205343641-e2f77b6a-38e6-418f-ad60-035c3e2dc5f2.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343649-e8bec0b9-d84e-4b2b-86a4-771ebcaa8e13.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343659-f5a04650-7453-4bef-b1d9-756166e7ad8d.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343669-56436773-eb5c-4af5-8c61-45586ead5b5d.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343681-1e33d2e0-2103-4379-bda4-14a8947b4b6c.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343713-112ab192-7c0c-4774-ad6a-9082d448a93b.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343722-9ff0f39f-6aa5-4a7c-9998-1d297e8bc5a7.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343736-564b5e34-16b8-4a77-a5be-b43544a9287e.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343744-9086e5c9-701a-4754-8638-bfb877611617.png)
![изображение](https://user-images.githubusercontent.com/38161044/205343751-333101b2-adc3-4271-bbca-df5ff766302d.png)

Уменьшил Labmd до 0.7 - Параметр регуляризации (лямбда), используемый при расчете обобщенной оценки преимущества. Чем выше значение, тем меньше полагается на себя.
В моем случае привело к уменьшению эффективности.
![изображение](https://user-images.githubusercontent.com/38161044/205344089-b071a774-ad1d-4578-8813-fb363267f86b.png)
![изображение](https://user-images.githubusercontent.com/38161044/205344096-c50dfe7e-b1f5-44fa-9340-902d953c028d.png)
![изображение](https://user-images.githubusercontent.com/38161044/205344107-289cc378-a970-4268-a7f2-69917b08bc47.png)
![изображение](https://user-images.githubusercontent.com/38161044/205344117-4b3485b6-a8ba-4c9d-b50b-b60782c95ebe.png)
![изображение](https://user-images.githubusercontent.com/38161044/205344127-36856a71-e9b8-4cba-911a-af32630af691.png)
![изображение](https://user-images.githubusercontent.com/38161044/205344132-cc61ac8b-2cec-46b9-bab5-c972d49173f8.png)
![изображение](https://user-images.githubusercontent.com/38161044/205344145-e43b6a44-63a3-4f60-af57-256af79998c6.png)
![изображение](https://user-images.githubusercontent.com/38161044/205344154-122aa4a1-3eda-457f-8306-033d703bd842.png)
![изображение](https://user-images.githubusercontent.com/38161044/205344158-38456957-b078-48f5-9543-2c0e72e1bc9f.png)
![изображение](https://user-images.githubusercontent.com/38161044/205344170-6c590fec-1f16-41e9-91bf-48d7491e9004.png)

## Задание 3
Опишите результаты, выведенные в TensorBoard.

Cumulative Reward - Среднее совокупное вознаграждение за эпизод по всем агентам. Должно увеличиваться во время успешной тренировки.
Episode Length - Средняя продолжительность каждого эпизода в окружающей среде для всех агентов.
Policy Loss - Средняя величина функции потерь. Соотносится с тем, насколько сильно меняется политика (процесс принятия решений). Величина этого должна уменьшаться во время успешной тренировки.
Value Loss - Средняя потеря обновления функции значения. Коррелирует с тем, насколько хорошо модель способна предсказать значение каждого состояния. Это должно увеличиваться, пока агент обучается, а затем уменьшаться, когда вознаграждение стабилизируется.
Beta - график, показывающий изменение силы энтропийной регуляризации
Entropy - Насколько случайны решения модели. Должна медленно уменьшаться во время успешного тренировочного процесса.
Epsilon - Соответствует допустимому порогу расхождения между старой и новой политикой при обновлении градиентного спуска.
Extrinsic Reward - Это соответствует среднему совокупному вознаграждению, полученному от окружающей среды за эпизод.
Extrinsic Value Estimate - Оценка агентом стоимости вознаграждения 
Learning Rate - Насколько большой шаг делает обучающий алгоритм при поиске оптимальной политики. Должно уменьшаться со временем.

## Выводы
В результате данной лабораторной работы я интегрировал экономическую систему в проект Unity и обучил Ml Agent. Познакомился с TensorBoard, построил графики для оценки результатов обучения. 
