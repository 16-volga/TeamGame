# TeamGame
Analysis of smart meter data in London

# Анализ данных интеллектуальных счетчиков Лондона
Чтобы лучше следить за потреблением энергии, правительство Великобритании хочет, чтобы поставщики энергии устанавливали интеллектуальные счетчики в каждом доме в Англии, Уэльсе и Шотландии. В перспективе для поставщиков энергии есть 26 миллионов домов,  и в планах  к 2020 году каждый дом должен иметь умный счетчик.

Вашему вниманию представлено исследование, основанное на данных, содержащих показания, снятые с интеллектуальных счетчиков, по энергопотреблению для 5567 лондонских домохозяйств, которые приняли участие в проекте Low Carbon London, возглавляемом британскими энергосистемами, в период с ноября 2011 года по февраль 2014 года.

*В проекте приняли участие:*

*Project lider:*

- Фурман Юрий Анатольевич, yuri063@yandex.ru

*Разработчики:*

- Шапилов Александр Викторович, sankas@lenta.ru
- Яров Евгений Андреевич, chatobec@yandex.ru
- Зинович Эдуард Владимирович, bozon5@yandex.ru

*Technical writer:*

- Боткин Александр Сергеевич, spratlist@yandex.ru

***Конкретные числовые  значения измеренных величин в таблицах, в комментариях и на графиках в пояснительной записке могут отличаться от тех же величин в notebook с кодом, т.к. при расчетах выборка на всем массиве данных берется каждый раз случайным образом. Тем не менее эта разница не влияет на полученный результат и сделанные в работе выводы, т.к. является, всего лишь, статистической погрешностью измерений***


Данное исследование проведено в соответствии с представленным ниже планом:
### 1. Первичный анализ имеющихся данных:

1.1. Выборка основных наборов данных для дальнейшего рассмотрения: 
-	informations_households.csv;
-	acorn_details.csv;
-	daily_dataset.csv;
-	uk_bank_holidays.csv;
-	weather_daily_darksky.csv;
-	weather_hourly_darksky.csv;
-	halfhourly_dataset;
-	hhblock_dataset/block_xxx.
### 2. Подготовка и анализ данных для исследования:

2.1. Анализ распределения домохозяйств по группам;

2.2. Анализ полноты представленных данных об энергопотреблении;

2.3. Финальное редактирование полученных данных;

### 3. Анализ энергопотребления:

#### 3.1.  Произведем анализ зависимости суммарного потребления энергии от среднесуточной температуры. Найдем средний прирост потребления энергии при изменении температуры:

3.1.1. Построим график зависимости суммарного потребления энергии и среднесуточной температуры от времени.

3.1.2.	Рассчитаем средний прирост потребления энергии при изменении среднедневной температуры на 1 градус Цельсия.

#### 3.2. Сделаем сравнение потребления энергии в выходные/праздничные и рабочие дни.

#### 3.3. Для каждой из пяти групп потребителей проведение анализа суточного энергопотребления в течение 2013 года:

3.3.1. Сравнение ночного, дневного и суммарного энергопотребления

3.3.2. Сравнение энергопотребления по периодам Т1, Т2 и Т3

#### 3.4. Для каждой из пяти групп потребителей построение графиков зависимости суточного потребления энергии от длины светового дня:

3.4.1. Построение графиков зависимости суточного потребления энергии от длины светового дня, и от среднесуточной температуры

3.4.2. Расчёт среднего прироста потребления энергии при изменении среднедневной температуры комфорта и длительности светового дня

#### 3.5. Исследование зависимости суммарного потребления энергии в течение года от времени суток; от дня недели и месяца года:

3.5.1. Тепловая карта потребления электроэнергии - время года/время суток

3.5.2. Тепловая карта потребления электроэнергии - дни недели/недели года

#### 3.6. Подробное исследование зависимости потребления энергии от среднесуточных температур в течение года:

3.6.1. Построение регрессионной модели зависимости энергопотребления от температуры наружного воздуха

3.6.2. Нахождение оценки R-квадрат (коэффициент детерминации; в Python - r2_score)

3.6.3. Нахождение доли домовладений, предположительно использующих электроэнергию для отопления.

### 4. Выводы.
