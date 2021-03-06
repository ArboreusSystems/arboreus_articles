# Почему Erlang?

![](https://raw.githubusercontent.com/ArboreusSystems/arboreus_articles/master/erlang/why_erlang/illustrations/why_erang_001.png)

Выбор любой технологии должен быть обусловлен задачей которую нужно решить. Данная статья описывает причины выбора Erlang для разработки приложений:

* платежных систем использующих или не использующих [blockchain](https://github.com/ArboreusSystems/arboreus_articles/tree/master/blockchain)
* отказоустойчивых систем хранения данных различного объема ([data storage, big-data storage, etc](https://github.com/ArboreusSystems/arboreus_articles/tree/master/data_storage))
* систем логирования событий ([envent driven systems](https://github.com/ArboreusSystems/arboreus_articles/tree/master/event))
* и т.д.

При необходимости данный список может быть бесконечным, но у всех этих задач есть общее - все эти задачи не могут быть решены при помощи только одного сервера. Логика этих приложений будет всегда обязывать разрабатывать механизм позволяющий реализовывать межсерверные сообщения. Эти приложения всегда будут распределенными (distributed).

Distributed - ключевой термин для выбора Erlang. Этот язык и виртуальная машина разрабатывались изначально для распределенных систем со сложной логикой взаимодействия. Механизм взаимодействия - с самого начала в архитектуре языка. На момент написания этой статьи никакой другой язык не может предоставить в готовом виде подобный механизм. Вы будете обязаны разрабатывать его, а это огромная часть системы которая потребует огромных вложений и времени.

Если коротко то объяснение причин выбора Erlang может звучать так: **язык который создан для разработки распределенных (distributed) приложений с самого начала**.

Помимо этого, Erlang позволяет использовать данный механизм для приложений написанных на С/С++ ([Erlang NIF](http://erlang.org/doc/tutorial/nif.html)). Вы можете разработать модули на С/С++ и  использовать Erlang для распределения по серверам, в кратчайшие сроки с минимальными затратами.

На основании опыта разработки распределенных приложений, самый лучший способ это разработка прототипов на Erlang используя механизм распределения и если недостаточно его (нужно повысить производительность, нужно повысить безопасность и т.д.) разрабатывать на C/C++. При необходимости, можно использовать компилированные модули на Java через обертку разработанную на С/С++, но это будет выглядеть как заклинивший ручной тормоз на гоночном автомобиле.

Следите за обновлениями автора в [**Linkedin**](https://www.linkedin.com/in/alexandr-kirilov-3365b992/).

Следите за AR|BO|RE|US обновлениями в [**Twitter**](https://twitter.com/ArboreusSystems) в [**Linkedin**](www.linkedin.com/company/arboreus-systems/).