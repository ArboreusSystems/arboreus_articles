# Понимание Blockchain.

То, что сейчас называется blockchain - является одним из воплощений фундаментального механизма, позволяющего оперировать каким-либо множеством элементов как одним целым. 

Одним из самых ярких примеров, иллюстрирующих этот механизм, может быть обычная стена. Стена в офисе, стена в квартире, или еще где-либо. Стена может состоять из кирпичей или каменных блоков соединенных раствором цемента с песком, может состоять из досок или бруса скрепленных между собой и т.д. Но когда необходимо  упоминание "стены", происходит упоминание "стены", а не 13267 кирпичей скрепленных 2-я тоннами раствора или 237 досок сколоченных 589-ю гвоздями. И в свою очередь когда нужно раскрыть свойства "стены" мы говорим об элементах составляющих "стену" - о кирпичах с раствором или досках с гвоздями.

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/understanding_blockchain/illustrations/arb_illustartions_blockchain_017_rus.png)

На данном изображении показана "стена" (blockchain), которая является множеством состоящим из элементов - "кирпичи" (elements), которые скреплены (blocked) между собой цементным раствором в определенном порядке. В контексте описанном термином "стена" - элементы "кирпичи" которые зафиксированы раствором в соответсвии с идеей (idea) "стена", но в контексте "дом" - элементами становятся "стены" которые скреплены идеей (idea) "дом", а в контексте "кирпич" - элементами становятся ингредиенты необходимые для производства кирпича закрепленного рецептурой производства кирпича на основании идеи "кирпич", и дальше в контексте каждого ингредиента существует химическая формула каждого ингредиента и т.д. С точки зрения информации это выглядит как связь родители-ребенок (parents-child) или спиральная модель развития описанная в статье ["Spiralnoyes"](https://github.com/alexandrkirilov/kirilov_articles/blob/master/unsorted/spiralnoyes/rus.spiralnoyes.md).

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/understanding_blockchain/illustrations/arb_illustartions_blockchain_018_rus.png)

Человек с самого детства сталкивается с этим механизмом не подозревая этого. Можно бесконечно описывать примеры этого механизма:
* Словообразование - когда из букв, складываются слова в контексте описываемого объекта, из слов складываются предложения в контексте ситуации, а из предложений складываются тексты описывающие идею.
* В химии это построение элементов
* Еще одним примером является английская народная сказка-песня ["Дом который построил Джек"](https://ru.wikipedia.org/wiki/Дом,_который_построил_Джек) (Перевел эту сказку-песню [Маршак С.](http://www.world-art.ru/lyric/lyric.php?id=4367))
* и т.д.

Основой для создания "целого" (blockchain) из "множества элементов" (blocked elements of the chain) является "идея" (idea), отражающая то, что мы хотим достичь или получить в итоге. Исходя из значения слова ["идея"](https://ru.wikipedia.org/wiki/Идея_(значения)), основой является вид или форма того что мы хотим получить в итоге. Руководствуясь идей мы выбираем компоненты которые будут составлять ту форму, которая будет соответствовать "идее", мы ищем способ реализации "идеи" из существующих компонентов, и если не хватает компонентов, мы должны спустится на уровень ниже, сформировать новую "идею" которая будет отражать необходимый компонент. И так далее по всем уровням. Если описывать это на базе примера изображенного выше, то вы никогда не создадите дом в городе, если у вас нет кислорода для смешивания его с водородом для получения воды (или нет готовой воды), которая нужна для производства кирпича при смешивании с глиной. Выглядит знакомо? В доме который построил Джек? 

Или в другом случае, если вы изменили свойства воды, то при перестроении зависимостей это может уничтожить весь дом или как минимум сделать необходимым перестроение всего дома.

Идея всегда определяет структуру организации элементов внутри целого. 

Если идея обязывает к построению статического объекта вы и будете описывать статический объект - для иллюстрации можно взять пример описанный в статье ["Blockchain пример для Desktop/Mobile приложения"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/blockchain/bc_example_desktop_mobile_application/rus.bce_desktop_mobile_application.md). В этом примере рассматривается статическое приложение, в котором нужно обеспечить неизменность приложения при установке его на стороне пользователя.

Если же идея обязывает к построению динамически изменяемого объекта, то нужно фиксировать формулу отражающую динамику изменения объекта, делая его тем самым статичным с точки зрения неизменности структуру позволяющей данному динамическому изменению существовать - для иллюстрации можно взять пример описанный в статье ["Blockchain пример для Event Flow"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/blockchain/bc_example_event_flow/rus.bce_events_flow.md). В этом примере описывается динамически изменяемых поток событий - event flow, события постоянно происходят и дополняют поток в определенном порядке. Этот порядок (block) и является статической структурой потока (chain of events), которая обеспечивает неизменность структуры потока (blocked chain) вне зависимости от событий и времени.

Если пытаться статически зафиксировать динамически изменяемый объект (то, что сейчас используется в blockchain решениях для финансового сектора, в классическом варианте это описано в [Wiki](https://en.wikipedia.org/wiki/Blockchain)), то это будет постоянно вызывать необходимость полной перестройки (перерасчета root hash) объекта в зависимости от новых параметров используемых при построении (transaction), что в свою очередь рано или поздно вызовет невозможность дальнейшего использования данного объекта по причине:

* высокой себестоимости
* отсутствия вычислительных мощностей
* и т.д.

Для того чтобы избежать тупика, в первую очередь нужно определять "идею", что является динамическим, а что является статическим. И статическое фиксировать как статическое, а в случае с динамическим фиксировать закономерность изменений, а не новое состояния объекта в результате произошедших изменений. Представьте на секунду, что в 3D моделировании и анимации используются не формулы описывающее движение, а список значений координат объекта. Представили? Понравилось?

Следите за обновлениями автора в [**Linkedin**](https://www.linkedin.com/in/alexandr-kirilov-3365b992/).

Следите за AR|BO|RE|US обновлениями в [**Twitter**](https://twitter.com/ArboreusSystems) в [**Linkedin**](www.linkedin.com/company/arboreus-systems/).