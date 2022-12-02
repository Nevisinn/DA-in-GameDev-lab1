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
![изображение](https://user-images.githubusercontent.com/38161044/205350178-1c3d88e7-587d-45b8-bf27-5290056092e4.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350221-1f859eb5-b400-48ae-8a81-af936ded5891.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350279-95ac1484-1b9f-43ec-a701-eb4c680872fa.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350308-2520cccd-15c9-435e-bf4b-0912886b0135.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350337-b1a0f5f1-1058-4d1b-a755-f2afaee61f07.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350393-c2edf5a9-2221-4391-97bd-de67a7d71d83.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350413-4347c1cd-f8ac-423a-88cc-97d2dcba09e7.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350451-efb04ebe-66b2-4a7b-9c93-f9ef88f20281.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350481-966df41d-1210-4ede-bdad-2cc6479e16a1.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350495-8cd48c0a-cb88-4aa9-9947-890ab8d918fd.png)


Увеличил epsilon до 0,3. Он влияет на то, насколько быстро политика может развиваться во время обучения. Соответствует допустимому порогу расхождения между старой и новой политикой при обновлении градиентного спуска. По итогу обучение происходит быстрее, но стабильность падает.

![изображение](https://user-images.githubusercontent.com/38161044/205350551-78fa76aa-bf34-4c1f-b646-aa9eb9ed39fb.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350581-f60da170-7306-4a19-bb3a-ea72b9b57eba.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350597-d4eb554f-c786-489b-9830-acafb1cdb118.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350632-b5a4ccf2-5f7b-445b-ad16-04cbd5dea78e.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350686-dcdc07ff-1eda-46ca-a680-d1247edb0615.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350714-a75080d1-fd34-43de-89e1-b5b9b8e2af5e.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350751-62bbbd70-5b87-457a-806b-1083f716dae0.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350834-1f7bb465-9aca-499a-a527-956af1098e1f.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350854-91765728-c509-4048-b722-e3b9cce9bd0e.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350874-1a71f7db-a965-4ac3-b895-28e2fafcfe57.png)


Увеличил num_epoch до 10 - количество эпох обучения. Чем больше значение, тем график становится все более нестабильным. 

![изображение](https://user-images.githubusercontent.com/38161044/205350944-137de63d-6e5c-4d33-bd0b-ebf3d784eb66.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350963-c5e29e60-ede7-4bc7-9c7a-9f5a14cf3d9d.png)
![изображение](https://user-images.githubusercontent.com/38161044/205350998-ce9bbb79-4bfa-4fde-a9a1-d25de6e5da59.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351018-ebc6217e-3754-4a5f-84b1-ea7b2e0aae07.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351053-6e23fa55-cbbb-4e1a-ba4a-fa5bec9b6faf.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351067-e40b9eef-63ad-4dac-8908-c5b65661eb79.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351087-5bfe702c-7448-4716-bc18-846acd3c4a83.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351122-af6876eb-cd76-42a7-b62a-633ba9c3e8c8.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351153-569e976e-fc51-4ed8-a820-603538e51fc5.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351170-1674746f-3e28-4f17-bee1-6038fc1cd317.png)


Уменишил beta до 1.0e-4 - Сила энтропийной регуляризации, которая делает политику «более случайной». Чем меньше параметр, тем меньше действий совершают агенты.

![изображение](https://user-images.githubusercontent.com/38161044/205351222-a148c36c-b928-4a83-9350-c2e6167688dc.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351246-2be425a8-a922-4737-8121-c53ba8e2f1f0.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351282-47632879-eb16-49cc-af34-1d56ffe51dea.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351304-54472bb4-eb3e-4b9b-a013-0325aea29f7a.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351325-81cea668-9ab8-425a-baef-864a0c1f18ec.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351343-8b748b95-b89c-498c-8528-145681d60a67.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351364-e93c6da3-e0fd-4ecd-999d-2bc75f65ebf4.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351389-27093357-8b66-45bb-86ac-281f77f1749d.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351408-8465869c-5877-4c6f-857d-d7ca6f1f1316.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351425-814bdd02-e0c7-45ab-b431-ef999c08b041.png)

Уменьшил Labmd до 0.7 - Параметр регуляризации (лямбда), используемый при расчете обобщенной оценки преимущества. Чем выше значение, тем меньше полагается на себя.
В моем случае привело к уменьшению эффективности.

![изображение](https://user-images.githubusercontent.com/38161044/205351475-e61fbdc8-b5db-47ef-95c1-8cde937608cc.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351492-6b4de559-b7b6-4582-a6ae-02d5bc169688.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351517-41336786-7df5-4a80-97d8-4bde60e6c623.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351537-f3254234-dd84-42ff-a041-6be6d658687a.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351581-d29d135e-8346-4279-8f18-03a345330622.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351599-49ee3bf4-429f-4070-bce7-9c2e932c5695.png)
![изображение](https://user-images.githubusercontent.com/38161044/205351613-c67f1e1e-95e9-4cc8-9cfe-f525014cebd8.png)


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
