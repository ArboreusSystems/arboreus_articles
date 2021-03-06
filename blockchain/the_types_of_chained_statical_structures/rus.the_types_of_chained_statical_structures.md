# Blockchain. Типы статических структур.

Для определения основного типа статической структуры, для использования при разработке blockchain-приложений нужно понимать, что не существует (скорей всего только на момент написания статьи) универсального способа которой позволит реализовать одно программное решения для всех возможных случаев использования этой технологии. На данный момент каждую структуру и главное то, как она будет использоваться или применяться в реальном мире нужно рассматривать отдельно.

При создании слишком сложной структуры blockchain можно убить возможность использовать эту структуру, т.к. доступ к этой структуре будет или сильно ограничен или замедлен, что сделает из этой технологии "ручной тормоз" вместо "двигателя прогресса". 
Нужно соизмеряйть необходимость использования данной технологии с требованиями использования и применения структуры в реальном мире. Любая структура создана "потому что и для чего-то" и если использование структуру стало невозможным - зачем такая структура нужна? Далеко не всегда нужно использовать эту технологию, иногда достаточно примитивных, но не менее значимых и давно используемых способов.

Что такое статическая структура? Это та структура которая не меняет свою структуру с течением времени. Она существует в одном состоянии которое было сформировано в момент создания.

Теперь о типах структур. В данной статье описаны только некоторые принципиальные схемы, наиболее значимые для применения при разработке blockchain-приложений. В природе их может существовать огромное количество т.к. они являются отражением идеи (idea).

**1) Root-oriented или Tree-like (Merkle tree)**

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/the_types_of_chained_statical_structures/illustrations/blockchain_002.png)

Если по русски то - древовидная. Как правило хороша в использовании для описания статических структур или относительно медленно развивающихся структур (Mobile/Desktop приложения, структуры компании, кластера серверов и т.д.). Своего рода способ описания чего-то монолитного состоящего из каких-либо частей. Используется в классической модели построения [blockchain](https://en.wikipedia.org/wiki/Blockchain). При добавлении узла обязывает произвести перерасчет всей структуры.

**2) Linear или vector**

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/the_types_of_chained_statical_structures/illustrations/blockchain_003.png)

Если по русски то - линейная. Линейной структурой называют структуру в которой элемент может иметь связь с не более чем двумя другими элементами. Для примера, может быть применена для:

* описания событий (event) привязанных ко времени события, где значение времени является связью в структуре - больше или меньше относительно текущего или заданного;
* описания маршрута следования, где элементы (для примера адреса следования) могут быть либо впереди либо сзади и очередность прохождения адресов есть block для элементов chain (цепи);

Частные случаи от неё:

* Циклическая - когда последний элемент цепи связан с первым
* Путь от root до последнего элемента ветки древовидной структуры.

**3) Matrix**

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/the_types_of_chained_statical_structures/illustrations/blockchain_004.png)

Если по русски - матричная. Одна из наиболее сложных в разработке структур. Если говорить просто - то это некая связь определенная какой-то формулой между элементами структуры или нескольких структур. Для примера можно рассмотреть создание периодических отчетов филиалов некой компании, где есть первичная структура - расписание подачи отчетов (для примера каждые 10 минут, в обслуживании серверов - cron с определенным временем для выполнения какого-то действия) и есть потоки событий для каждого подразделения копании, и с частотой 1 раз в 10 минут система "открывает глаза", смотрит на происходящее и фиксирует состояние отделов компании. Элементом матричной структуры может являться запись в базе данных, где для примера первое поле таблицы - значение времени из начальной структуры, а остальные поля значение состояний филиалов компании в момент когда "глаза открыты".

При разработке матричных структур можно привести бесконечное множество таких примеров.

**4) Organic**

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/the_types_of_chained_statical_structures/illustrations/blockchain_005.png)

Органический тип. Название позаимствовано из "Химии", на основании раздела "Органическая химия" как одного из наиболее ярких примеров данного рода структур. Данный тип не является отдельным, скорее это свойство которое может быть добавлено к любой другой структуре, с одной разницей - все рассмотренные ранее структуры представляли из себя одноранговые объекты с одноранговыми связями. В "Химии" элементы структуры (молекулы) могут иметь валентность, что определяет возможность связи с другими элементами и характер связи как-таковой.

Данный пример можно привести не только для "Химии", такие же структуры окружают нас везде:

* автодороги, где ширина дороги и качество покрытия определяют скорость движения и максимально возможную плотность потока
* электрические сети, где максимальное значение напряжения и силы тока для кабеля определяют емкость сети а структура трансформаторного узла определяет возможности для объединения сегментов сети с основным кабелем
* тот же самый интернет 
* и т.д.

Основной задачей данной статьи было - показать несколько возможных типов структур (chain) для фиксации (block). Информацию о том как при помощи технологии blockchain защищать структуры от одного или нескольких видов опасности можно получить из статей ["Arboreus articles: blockchain"](https://github.com/ArboreusSystems/arboreus_articles/tree/master/blockchain).

Следите за обновлениями автора в [**Linkedin**](https://www.linkedin.com/in/alexandr-kirilov-3365b992/).

Следите за AR|BO|RE|US обновлениями в [**Twitter**](https://twitter.com/ArboreusSystems) в [**Linkedin**](www.linkedin.com/company/arboreus-systems/).