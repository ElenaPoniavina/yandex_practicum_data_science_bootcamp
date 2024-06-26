# Исследование популярности консольных игр и игровых платформ

## Описание проекта
Имеется интернет-магазин «Стримчик», который продаёт по всему миру компьютерные игры. Из открытых источников доступны исторические данные о продажах игр, оценки пользователей и экспертов, жанры и платформы (например, Xbox или PlayStation). Выявим определяющие успешность игры закономерности. Это позволит сделать ставку на потенциально популярный продукт и спланировать рекламные кампании на следующий год.
Также проверим две гипотезы:
- Средние пользовательские рейтинги платформ Xbox One и PC одинаковые
- Средние пользовательские рейтинги жанров Action и Sports разные

## Этапы проекта
1. Загрузим и проведем предобработку данных: исправим типы данных, проанализируем пропуски и дубликаты, создадим новые столбцы.
2. Проведем исследовательский анализ:
  - Оценим количество выпускаемых игр в разные года.
  - Оценим продажи по платформам.
  - Изучим суммарные продажи по играм.
  - Изучим влияние отзывов на продажи.
  - Изучим распределение игр по жанрам.
4. Составим портрет игрока каждого региона
5. Проверим гипотезы
6. Сформулируем общие выводы
   
## Результат
На этапе исследовательского анализа было проанализировано:
1. Количество выпускаемых игр в разные года
Количество выпускаемых игр стремительно росло примерно до 2008-2010 года, а затем снизилось примерно до уровня 2000-го года. Возможно, объясняется это тем, что мобильные телефоны достигли достаточного уровня развития и пользователи переключились на мобильные игры (соответственно, игр на платформах в связи с уменьшившимся спросом тоже стало выпускаться меньше).
2. Продажи по различным платформам
  - Наиболее полпулярные платформы всех лет: PS2,X360, PS3,Wii,DS,PS.
  - Наименее популярная платформа - PCFX.
  - некоторые платформы постепенно заменяли друг друга (например, PS->PS2->PS3).
  - платформа, выпустившая игру первой - DS, впервые выпустившая игру в 1985году (но, похоже, продаж от нее так и не получившая), однако затем она не выпускала игр вплоть до 2004года. Так что первым сильным лидером можно назвать платформу PS, которая имела хорошие продажи примерно c 1994 до 2004года, а затем была заменена более современной версией PS2
  - платформы, получавшие максимальные годовые продажи - PS2(2000-2005годы) и Wii(2009год).
  - за последние 5 лет (2010-2015годы) выделяются два лидера - X360 и PS3, продажи которых находились примерно на одном уровне.
по всем платформам в последние годы в основном наблюдается спад продаж
<br>Если смотреть данные за последние 3 года:
  - В последние 3 года игры выпускают только 3 платформы: PS3, X360 и Wii и на текущий момент их продажи находятся практически на одном уровне. Однако PS3, X360 (в отличие от Wii) в последние 3 года имели продажи гораздо выше (до 80-110 млн. копий игр) и затем постепенно снизили продажи практически до 1,5-3,5млн.копий, в то время как Wii постепенно сдала позиции уже в 2011-2013годах году и к 2016году продает не более 200тыс.копий игр.
<br>Таким образом, последние три года потенциально прибыльными платформами игр явяются PS3 и X360, причем, несмотря на то, что падение продаж PS3 происходит быстрее, на конец 2016года PS3 продает почти вдвое больше игр, чем X360 - 3,6млн.копий против 1,5млн копий у X360.
3. Суммарные продажи составляют в основном от 60тыс до 470тыс. копий. При этом есть выбросы и одна из игр была продана более чем 82,5млн раз - WiiSports.
<br>Большинство выпускаемых игр даже близко не могут приблизиться к успеху игр, которые мы видим в top-10. По общей описательной статистике , 75% квартиль по суммарным продажам не превышает полумиллиона проданных копий.
<br>За всю историю в целом превысили планку продаж хотя бы в 1млн.копий только 2тыс.игр.
<br>Наибольшее число популярных игр за всю историю было у платформ платформ Wii, DS и PS. Однако, как видим, платформа DS перестала выпускать игры в 2014году, а также PSиPS2 обновились до PS3 и шестерка лидеров превратилась в тройку.
<br>По данным за последние 3 года, можно проследить стратегию каждой компании из тройки за последние 3 года:
  - у платформы PS3 больше всего игр-самородков, приносящих свервысокие продажи (максимально высокие выбросы), однако при этом и самый низкий 75% квартиль, что означает, что компания также выпускает много непопулярных игр. То есть, компания работает на количество: чем больше количество разнообразных игр, тем более вероятно, что какие-то из них станут мегапопулярными. При этом неудачные релизы снижают общую статистику по продажам.
  - у компании Wii противоположный подход: меньше всего выбросов, но самый высокий 75% квартиль, что говорит о том, что каждая выпущенная игра стабильно хорошо продается, но при этом мегапопулярной (как некоторые игры PS3) скорее всего не станет (мы видим только 1 выброс и он втрое ниже, чем максимальный выброс по PS3).
  - у компании X360 средний подход: есть и стабильно продаваемые игры, и при этом достаточное количество высоких выбросов.
4. Зависимость продаж от рейтинга критиков и пользователей На примере платформы PS3 Были проанализированы зависимости.
  - игры с высокой оценкой критиков могут как быть очень популярными, так и непопулярными. Однако, игры с низкой оценкой критиков не бывают сверхпопулярными - до оценки 70 нет даже единичных выбросов. Верхняя граница области разброса довольно четкая.
по оценкам пользователей зависмость менее однозначная: есть непопулярные игры с высокой оценкой и сверхпопулярные игры со средней или даже низкой оценкой. Это логично, у разных пользователей разные вкусы и предпочтения и разное субъективное восприятие игр, поэтому оценки могут отличаться от оценок экспертов, которые могут оценивать только объективно по заданным критериям. Но так как продажи формируются именно пользователями (а не критиками), то и даже при высокой оценке критиков игра может стать как популярнй, так и наоборот.

Почему есть случаи низкой оценки пользователей и высокого уровны продаж? Тут скорее всего играют роль несколько факторов:
  - мы не знаем в какое время проставлялись оценки. Возможно, игра вышла например в начале 2000х годов, получила высокие оценки критиков и изначально хорошо продавалась, но со временем игра устаревала, а пользователи продолжали ее устанавливать и проставлять оценки, но из-за того, что игра уже не соответствует времени, итоговая оценка снижалась.
  - либо игра могла быть очень популярна в одном регионе и там формировать основной доход, но при этом вызвала негативные отклики в другом регионе, что вызвало ухудшение общей оценки. Такои случаи можно отдельно проанализировать.
  - также фактор, который может повлиять: не все пользователи, которые покупают ту или иную игру, могут проставлять оценки по ней. Скорее всего, есть большое количество людей, которые просто играют (и формируют продажи), но не оставляют ни оценок, ни отзывов.

Коэффицицент корреляции продаж от оценки критиков по платформе PS3 равен 0,4 (средняя корреляция), в то время как корреляция от оценки пользователей равна 0,27 (слабая). Также прослеживается средняя корреляция оценки пользователей от оценки критиков на уровне 0,4, но это скорее говорит о частых случаях, когда мнения критиков и пользователей об игре совпадают, нежели о реальной зависимости оценки пользователей от критиков или наоборот.
<br>Если смотреть в целом по всем платформам, то коэффициенты корреляции становятся еще меньше: 0,23 для оценки экспертов и 0,2 для оценки пользователей. Возможно тут влияет тот факт, что среди наших платформ есть старые и новые поколения одной и той же платформы (PS, PS2, PS3). Также возможно, играет роль, что система оценок могла меняться со временем (мы не ограничивали игры по году выпуска), либо могло меняться общее количество пользовательских оценок (пользователей в 1990году скорее всего было меньше чем в 2014г), а значит и выборка была разного объема.

4. Распределение игр по жанрам Выделяются наиболее популярные жанры в порядке убывания популярности: Action, Sports, Shooter, Role-Playing, Platform.
<br>При этом, количество игр в каждой категории не всегда коррелирует с количеством установок. Например, шутеров больше, чем стратегий примерно в 2 раза, а количество их установок больше в 6 раз. Аналогично: платформенных игр вдвое меньше, чем игр категории "Misc"(разное), а установок они приносят вдвое больше, то есть эффективность платформенных игр с точки зрения продаж выше в 4 раза.
<br>Однако, конечно, стоит не забывать, что это общая статистика, включающая игры-самородки, где кол-во установок одной только игры может достигать 80млн, поэтому и вся категория может быть в топе только из-за одной или нескольких сверхпопулярных игр.
<br>В качестве непопулярных жанров можно выделить стратегии, приключения и пазлы.

Портрет пользователя каждого региона:
<br>На данном этапа был сформирован портрет наиболее вероятного пользователя в каждом регионе:
  - Северная Америка: подросток или взрослый, играющий в игру жанра Action/Sport/Shooter на платформе X360, либо PS2.
  - Европа: подросток или взрослый, играющий в игру жанра Action/Sport/Shooter на платформе PS2, либо PS3.
  - Япония: скорее подросток, играющий в игру Role-Playing на платформе DS или PS.

Этап проверки гипотез:
1. Средние пользовательские рейтинги платформ Xbox One и PC одинаковые
<br>Нулевая гипотеза: средние рейтинги скорее всего одинаковые
<br>Альтернативная гипотеза: средние рейтинги не одинаковые.
<br>Вывод:
  - Средний пользовательский рейтинг X360: 4.88
  - Средний пользовательский рейтинг PS: 0.2
  - p-значение: 2.7378867563341513e-220
<br>Отвергаем нулевую гипотезу о равенстве средних. Средние пользовательские рейтинги не одинаковые, рейтинг X360 составляет 4,88 против рейтинга PS - 0.2.
2. Средние пользовательские рейтинги жанров Action и Sports разные
<br>Нулевая гипотеза: средние рейтинги скорее всего одинаковые
<br>Альтернативная гипотеза: средние рейтинги не одинаковые.
<br>Вывод:
  - Средний пользовательский рейтинг жанра Action: 3.37
  - Средний пользовательский рейтинг жанра Sports: 2.74
  - p-значение: 1.2025568367391132e-08
<br>Отвергаем нулевую гипотезу о равенстве средних. В данном случае можно сказать, что рейтинги действительно разные.
<br> Полный итоговый вывод содержится в файле проекта.

## Технические параметры среды
Библиотеки: pandas, numpy, skipy, math, matplotlib, seaborn
<br>Версия Python: 3.9.5

