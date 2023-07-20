Привет! 
Меня зовут Андрей
я начинающий аналитик данных, с большим пратичесикм опытом работы в финансовом и реальном секторе экономики. 

Окончил НОУ "Московский экономико-финансовый институт"
Обучаюсь по направлению Аналитик данных в Skypro

Вы можите связаться со мной по адресу: Электронная почта: andreyshatalov1@gmail.com

В этом репозитории вы можете найти некоторые из моих проектов, выполненных во время обучения.

НАВЫКИ И ТЕХНОЛОГИИ
Инструменты анализа данных: SQL, Excel:
Языки программирования и библиотеки: Python
Системы управления базами данных: PostgreSQL

ПРОЕКТЫ

ПРОЕКТ 1: Калькулятор юнит-экономики онлайн-кинотеатра

Что нужно было сделать:
Задача №1 необходимо было посчитать юнит-экономику продукта предложить сценарий по настройке параметров для выхода на 25-процентную маржинальность 
Задача №2 предложить сценарий по настройке параметров для выхода на 25-процентную маржинальность
Задача №3 собрать наглядную визуализацию, где будет показано, кто, где и в каком объеме смотрит фильмы на платформе

Ссылка на проект:
финальные расчеты: https://disk.yandex.ru/i/kOmopY0ASdJviw 
Итоговый калькулятор: https://disk.yandex.ru/i/lsCEHUqiaCIt0Q

ИТОГИ:
1. много не популярных фильмов
2. Приток новых клиентов снижается
3. Снижается пользовательский ретеншен

ПРОЕКТ 2: Калькулятор юнит-экономики онлайн-школы

Что нужно было сделать:
Задача №1 учесть в калькуляторе корректировку планов маркетинга
Задача №2 пересчитать план найма преподавателей

Как решал:
Задача №1:
1. Добавил в список параметров нашего калькулятора показатель "Поправочный коэф-т на привлечение"
Установил значение этого показателя по умолчанию как 100% и добавил возможность изменять этот показатель для расчётного периода 05.21-04.22 по аналогии с другими - через столбец "Изменение"
2. Настроил динамический расчёт количества новых студентов за период 05.21-04.22 с поправкой на этот коэффициент.
3. Просчитал сценарий, при котором планы маркетинга будут увеличены на 12% (настройки остальных показателей не меняются)
4. Настроить связь с листом План Маркетинга через ВПР
   
ИТОГ: Новый калькулятор

Задача №2:
1.Добавить в калькулятор Найма преподавателей возможность изменять входных параметры: Пропускную способность П и Retention П - с помощью дополнительного столбца с процентными изменениями, как это сделано на Главном листе с основным калькулятором Юнит-экономики
2. Сделал поправку в расчёте общей пропускной способности - изменил формулу так, чтобы отразить, что новые преподаватели в первый месяц своей работы могут проводить только половину уроков от средней пропускной способности преподавателя, задаваемой параметром
3. Обновил прогнозное количество уроков, добавив новые значения из Задачи 1 (полученные после поправки на планы маркетинга)
4. Просчитал сценарий, при котором Пропускная способность П увеличится на 15 процентов, а Retention П упадёт на 2 процента
5. С помощью Поиска решений составил новый план найма с ограничением: за месяц нельзя нанять более 70 преподавателей

ИТОГ: Обновлённый план по найму

Ссылка на проект: https://docs.google.com/spreadsheets/d/16YFiaPBIf8Wo1S87X9Gkz73bCF3GHQdJ/edit?pli=1#gid=1785325717

ПРОЕКТ 3: Когортный анализ онлайн-кинотеатра

Что нужно было сделать:
Задача №1 Постройте сводную таблицу с абсолютными доходимостями клиентов по месячным когортам.
Задача №2 Постройте таблицу с клиентским Retention
Задача №3 На основании Retention рассчитайте лайфтайм с помощью метода усредненных прямоугольников для каждой когорты
Задача №4 Рассчитайте LTR для каждой когорты с помощью ARPU.
Задача №5 Рассчитайте LTV с помощью усредненных костов для каждой когорты
Задача №6 Сделайте выводы относительно хороших и плохих когорт с точки зрения LTV

Как решал:
На основани "флагов" рассчитал ретеншены каждой кагорыт наложив в последующем постояныеи пременные косты

ИТОГИ:
Выделил показатели которые показывают наиболее высокие и низкие значения:
Когорту, которая показывает высокий LTV за счет высокого лайфтайма.
Когорту, которая показывает высокий LTV за счет низких костов.
Когорту, которая показывает низкий LTV за счет низкого лайфтайма.
Когорту, которая показывает низкий LTV за счет высоких костов

Ссылка на проект: https://docs.google.com/spreadsheets/d/1mE_jZpdvhZEBFIunYYIrYbGOjzdaGilk/edit#gid=1761452865

ПРОЕКТ 4: Моделирование изменений балансов студентов в SQL 

Что нужно было сделать:
1. Посмотреть на изменения балансов студентов собранных из СТЕ
2. Собрать визуализацию итогового результата

Как решал:
1. Узнаем, когда была пкрвая транзакция для каждого студента
2. Собираем таблицу с датами за каждый календарный день 2016 года
3. Создан CTE, где хранятся все сроки его жизни после того, как произошла первая транзакция студента
4. Находим все изменения балансов, связанных с самыми разнообразными транзакциями
5. Находим изменения балансов из-за прохождения уроков
6. Создаем CTE «балансы» с вычисленными балансами каждого студента
7. Посмотрим, как менялось общее количество уроков на балансах студентов

ИТОГИ:
1. вопрос к датаинженерам: Отрицательный баланс, который периодически появляется - это крайне странно + много нулевых значений 
2. Баланс студентов растет, то есть студенты покупают больше уроков чем расходуют.На первый взгляд кажется что график "classes" убывает, но это требует дополнительных исследований.

ВЫВОД:
В итоговой таблице можно увидеть, что к концу 2016 года накопительный итог по урокам был: 4534, студентам было начислено больше уроков, чем было пройдено. Если было установлено прохождение уроков по месяцам, то можно увидеть, что в начале 2016 года приход был небольшим, по сравнению с концом года. Можно сделать вывод, что к концу года учащиеся получают ответы на вопросы по урокам, поэтому ситуация намного выше. Появляются из выводов выше, что студенты бросают обучение медленно или последовательно, провоцируют тем самые исключения "хвостов", которые идут на следующий год.

Ссылка на проект: 
решение по шаговое : https://metabase.sky.pro/question/75306
Итоговые графики: https://metabase.sky.pro/question/75190
