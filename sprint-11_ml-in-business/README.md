## Определение наиболее выгодного региона нефтедобычи

### Задача проекта
На основе данных геологи разведки выбрать район добычи нефти

### Описание проекта
Вам предоставлены пробы нефти в трёх регионах. Характеристики для каждой скважины в регионе уже известны. Постройте модель для определения региона, где добыча принесёт наибольшую прибыль.

### Ключевые слова проекта
регрессия, разработка бизнес-модели, бутстреп

### Выводы
Как несложно заметить - в каждом из датасетов существуют дубликаты "уникальных" идентификаторов скважин. Но данные дубликаты несколько необычны в том смысле, что целевой признак у них не идентичен (как и все остальное). Можно предположить, что это ошибки именно в задублированном id. В любом случае - подобных строк немного и реальное влияние на конечный результат будет несущественнен вне зависимости от того, как поступить с данной аномалией. В данном конкретном случае - дубликаты в датасете были оставлены (так как id не будет учавствовать при обучении модели).

Единственный регион вообще показавший прибыльность у нижнего рубежа 95% доверительного интервала, высочайшую среднюю прибыль, а также минимальный уровень риска - регион №1. Таким образом, этот регион и является рекомендацией для разработки месторождений.