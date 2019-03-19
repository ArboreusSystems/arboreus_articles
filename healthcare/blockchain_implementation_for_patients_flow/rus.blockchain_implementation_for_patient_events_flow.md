# Разработка blockchain-решения для хранения данных о пациенте в event-driven системе.

Данная статья основана на других материалах представленных в данном репозитории:

* ["Event driven"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/event/event_driven/eng.event_driven.md)
* ["Event Driven for Healthcare"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/healthcare/event_driven_for_healthcare/eng.event_driven_for_healthcare.md)
* ["Blockchain"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/blockchain/rus.blockchain.md)

Для понимания принципов разработки blockchain-решения для хранения данных о пациенте в event-driven системе лучше ознакомиться с данными статьями. Данные статьи описывают фундамент на основании которого разрабатывается данная система.

Первое с чего нужно начать - с понимания на сколько сильно вам нужно именно blockchain-решение и можно ли без него обойтись так-как любое blockchain-решение всегда занимает больше времени на запись одной единицы хранения и сложнее и дороже в обслуживании. Что является той проблемой которую вы хотите решить при помощи blockchain-решения?

В случае с медицинскими учреждениями есть некий поток событий относительно пациента. Это могут быть осмотры состояния пациента, назначения лечения, результаты обследований и т.д. Основная проблема которую может решить blockchain - это исключить возможность фальсификации событий при длительном хранени данных это event-flow.

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/blockchain/bc_example_event_flow/illustrations/blockchain_007.png)

Пример технического решения данной проблемы детально описан в статье ["Blockchain пример для Event Flow"](https://github.com/ArboreusSystems/arboreus_articles/blob/master/blockchain/bc_example_event_flow/rus.bce_events_flow.md). Данное техническое решение может быть реализовано как на SQL-based базах данных так и на noSQL. Авторы статьи разрабатывали данное решение на Erlang/C. Выбор данной технологии позволяет обслуживать хранилища events огромного размера из-за масштабируемости Erlang.

При необходимости данное техническое решение может быть дополнено разделенным хранением логических и проверочных индексов что позволит очень сильно увеличить уровень безопасности хранения данных.

Следите за обновлениями автора в [**Linkedin**](https://www.linkedin.com/in/alexandr-kirilov-3365b992/).

Следите за AR|BO|RE|US обновлениями в [**Twitter**](https://twitter.com/ArboreusSystems) в [**Linkedin**](www.linkedin.com/company/arboreus-systems/).