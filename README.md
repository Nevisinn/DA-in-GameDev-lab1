# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #3 выполнил(а):
- Шубин Игорь Васильевич
- РИ210941
Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | # | 20 |

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
- Выводы.
- ✨Magic ✨

## Цель работы
Познакомиться с программными средствами для создания системы машинного обучения и ее интеграции в Unit

## Задание 1
### Реализовать систему машинного обучения в связке Python - Google-Sheets – Unity.
Проверка работы модели:

![ML - SampleScene - Windows, Mac, Linux - Unity 2021 3 10f1 Personal _DX11_ 2022-10-27 14-56-16(1)](https://user-images.githubusercontent.com/38161044/198255355-4b217afb-2404-4647-bbb8-02fefeaa4126.gif)


## Задание 2
### Подробно опишите каждую строку файла конфигурации нейронной сети, доступного в папке с файлами проекта по ссылке. Самостоятельно найдите информацию о компонентах Decision Requester, Behavior Parameters, добавленных сфере.
```c#
behaviors: 'Поведение'
  RollerBall:'В нашем случае шара'
    trainer_type: ppo 'Алгоритм обучения PPO'
    hyperparameters: 'гиперпараметры'
      batch_size: 10 'Количество опытов на каждой итерации градиентного спуска.)
      buffer_size: 100 'Количество опытов, которые необходимо собрать перед обновлением модели политики. Соответствует тому, сколько опытов должно быть собрано, прежде чем мы будем изучать или обновлять модель.)
      learning_rate: 3.0e-4 'Начальная скорость обучения для градиентного спуска. Соответствует силе каждого шага обновления градиентного спуска.)
      beta: 5.0e-4 'Сила энтропийной регуляризации, которая делает политику «более случайной». Это гарантирует, что агенты правильно исследуют пространство действий во время обучения. '
      epsilon: 0.2 'Влияет на то, насколько быстро политика может развиваться во время обучения. Соответствует допустимому порогу расхождения между старой и новой политикой при обновлении градиентного спуска.'
      lambd: 0.99 'Параметр регуляризации (лямбда), используемый при расчете обобщенной оценки преимущества (GAE). Это можно рассматривать как то, насколько агент полагается на свою текущую оценку стоимости при вычислении обновленной оценки стоимости. '
      num_epoch: 3
      learning_rate_schedule: linear'Определяет, как скорость обучения изменяется с течением времени.'
    network_settings:'сетевые настройки'
      normalize: false 'Применяется ли нормализация к входным данным векторного наблюдения. Эта нормализация основана на скользящем среднем и дисперсии векторного наблюдения. '
      hidden_units: 128 'Количество блоков в скрытых слоях нейронной сети. Соответствуют количеству единиц в каждом полносвязном слое нейронной сети'
      num_layers: 2 'Количество скрытых слоев в нейронной сети. Для простых задач меньше слоев, скорее всего, будут обучать быстрее и эффективнее.'
    reward_signals:'Раздел reward_signals позволяет вам устанавливать настройки как для внешних (т.е. основанных на окружающей среде), так и для внутренних сигналов вознаграждения (например, curiosity и GAIL). Каждый сигнал вознаграждения должен определять по крайней мере два параметра, силу и гамму, в дополнение к любым гиперпараметрам, специфичным для определенного класса.'
      extrinsic:Включите эти настройки, чтобы убедиться, что ваш тренировочный прогон включает в себя сигнал вознаграждения, основанный на окружающей среде.'
        gamma: 0.99 'Фактор дисконта для будущих вознаграждений, поступающих из окружающей среды. Это можно рассматривать как то, как далеко в будущем агент должен заботиться о возможных вознаграждениях.'
        strength: 1.0 'Фактор, на который умножается вознаграждение, данное средой. Типичные диапазоны будут варьироваться в зависимости от сигнала вознаграждения.)	
    max_steps: 500000 (Общее количество шагов (т. е. собранных наблюдений и предпринятых действий), которые необходимо выполнить в среде (или во всех средах при параллельном использовании нескольких) перед завершением процесса обучения.'
    time_horizon: 64 'Сколько шагов опыта необходимо собрать для каждого агента перед добавлением его в буфер опыта. Когда этот предел достигается до конца эпизода, оценка значения используется для прогнозирования общего ожидаемого вознаграждения из текущего состояния агента.'
    summary_freq: 10000 'Количество опытов, которое необходимо собрать перед созданием и отображением статистики обучения.'
```
DecisionRequester: Компонент DecisionRequester через регулярные промежутки времени автоматически запрашивает решения для экземпляра агента.
BehaviorParameters: Компонент для настройки поведения экземпляра агента и его свойств.


## Выводы

Ознакомился с основными операторами зыка Python на примере реализации линейной регрессии и написал программы Hello World на Python и Unity.
