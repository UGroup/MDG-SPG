Одностраничный генератор проекта
========
Для запуска необходимо:
* создать каталог c:\temp - в него будут генерироваться все проекты. 
** Папки с префиксом __DB/ - база данных
** Папки с префиксом __WEB/ - веб часть
* переписать в каталог c:\temp папку с библиотекам templ
* импортировать файл spg19082014.xml в любую область, например spg. В этой области:
** создать веб приложение ссылающееся на папку app, например /spg
** создать веб приложение /brokerspg вызывающее брокер WEB.Broker
* открыть в браузере http://localhost:57772/spg/index.html
* 
На странице
* Заполните название проекта
* Заполните название пакета в котором будут созданы классы
* Создайте произвольное количество классов нажимая на + указав лишь их имена
** в каждом классе создайте произвольное количество свойств

По завершении - нажмите кнопку создать. Если всё удовлетворяет правилам синтаксиса (пока проверок нет), то будут созданы:
* База данных
* Область к которой будет монтирована БД
* Веб приложение для файлов
* Веб приложение для брокера
* Классы и свойства в них
* Методы CRUD в каждом классе
* Соответствующий брокер, обслуживающий классы в пакете
* Веб часть с использованием bootstrap и angularjs
** CRUD методы в контроллере и фабриках
** роутинг
** меню классов
** формы просмотра,  создания и обновления свойств класса

на текущий момент все свойства типа %String
