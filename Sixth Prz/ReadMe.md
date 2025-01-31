# Практика 6: Атака по переносу (Transfer Attack) на модели ИИ


## Цель задания:

Изучить концепцию атаки по переносу, где противоречивые примеры, созданные для одной модели, используются для атаки на другую модель. Это задание требует создания нескольких моделей, генерации противоречивых примеров для одной модели и проверки их на другой модели.

## Задачи:

1. Загрузить несколько моделей, обученных на датасете MNIST.
2. Изучить теоретические основы атаки по переносу.
3. Реализовать атаку FGSM на одну модель и проверить, как противоречивые примеры влияют на другую модель.
4. Оценить точность обеих моделей


## Выполнение:

Выполнение работы было произведено в Google Colab - https://drive.google.com/file/d/1qyHnUhwB-lMBWLIqQi-HyIMWxSKFSvbw/view?usp=sharing

## Вывод:
В ходе выполнения данной практики удалось реализовать атаку по переносу на основе противоречивых примеров, сгенерированных с помощью метода FGSM. Результаты показали, что простая полносвязная модель (model1) продемонстрировала точность на противоречивых примерах на уровне 0.0735, а её точность на примерах, атакующих другую модель, составила 0.9426. Это подчеркивает ограниченную устойчивость данной модели к целевым атакам, но также показывает относительное снижение эффективности атак, направленных с другой модели.

Сверточная нейронная сеть (model2) показала гораздо более высокую устойчивость к атакам. Её точность на примерах, созданных для model1, достигла 0.9629, что свидетельствует о её лучшей способности справляться с переносимыми атаками. Тем не менее, противоречивые примеры, созданные для неё, смогли успешно атаковать model1 с точностью 0.9309, что доказывает наличие общих слабостей между архитектурами.

В результате анализа стало ясно, что атака по переносу работает эффективно, даже на моделях с разными архитектурами. Это подчеркивает важность разработки методов для повышения устойчивости моделей, таких как использование обучения с противоречивыми примерами или регуляризация. Эти результаты дают ценные сведения для анализа безопасности моделей и оценки их уязвимости.


## Автор

Брестер Андрей Николаевич, группа ББМО-02-23
