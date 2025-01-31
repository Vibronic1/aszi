# Практика 7: Создание и использование генеративных противоречивых примеров (GANbased Adversarial Examples)


## Цель задания:

Изучить использование генеративных моделей (GAN — Generative Adversarial Networks) для
создания противоречивых примеров. В этом задании мы создадим противоречивые примеры с
использованием GAN и проверим их влияние на модели классификации.

## Задачи:

1. Изучить концепцию генеративных противоречивых примеров.
2. Реализовать простую GAN для создания противоречивых изображений.
3. Оценить точность моделей классификации на противоречивых примерах, созданных спомощью GAN.
4. Сравнить атаку на обе модели (полносвязную и свёрточную сети).

## Выполнение:

Выполнение работы было произведено в Google Colab - https://drive.google.com/file/d/17I4mPUSksmNlESGPgI6vLO-fMWZldeas/view?usp=sharing

## Вывод:

Итогом выполнения практической работы стало создание генеративной состязательной сети (GAN) для генерации противоречивых примеров, которые использовались для оценки устойчивости двух различных моделей классификации. В процессе реализации были изучены основные концепции генеративных противоречивых примеров, создана простая архитектура GAN с генератором и дискриминатором, а также разработан процесс обучения сети для генерации сложных, реалистичных изображений. Это позволило эффективно изучить влияние противоречивых примеров на модели классификации.

На заключительном этапе были проверены две модели классификации: полносвязная и свёрточная нейронные сети. Обе модели продемонстрировали нулевую точность на сгенерированных примерах, что подтверждает высокую эффективность GAN в создании атак, способных вводить модели в заблуждение. Эти результаты совпадают с теоретическими ожиданиями, согласно которым GAN способны генерировать данные, визуально близкие к реальным, но одновременно трудные для корректной классификации.

Анализ итогов эксперимента подтвердил значимость использования GAN для исследования уязвимости нейронных сетей к противоречивым примерам. Нулевая точность обеих моделей на таких данных подчёркивает необходимость разработки более устойчивых архитектур, способных противостоять генеративным атакам. Эти выводы создают основу для дальнейшего изучения и совершенствования подходов к созданию более надёжных систем машинного обучения.

## Автор

Брестер Андрей Николаевич, группа ББМО-02-23
