Вопросы для интервью системного администратора Linux/DevOps
===========================================================

Коллекция вопросов для собеседования linux сисадмина/devops. Не стесняйтесь добавлять свои через pull request'ы, issues или сообщением по электронной почте.

## <a name='toc'>Содержание</a>

  1. [Общие вопросы](#general)
  1. [Простые вопросы о Linux](#simple)
  1. [Вопросы среднего уровня о Linux](#medium)
  1. [Сложные вопросы о Linux](#hard)
  1. [Вопросы экспертного уровня о Linux](#expert)
  1. [Вопросы по сетям](#network)
  1. [Вопросы о MySQL](#mysql)
  1. [Вопросы о DevOps практиках](#devop)
  1. [Забавные вопросы](#fun)
  1. [Время демо](#demo)
  1. [Другие ссылки](#references)


#### [[⬆]](#toc) <a name='general'>Общие вопросы:</a>

* Что вы узнали за вчера/эту неделю?
* Расскажите о предпочитаемом окружении разработчика/администратора. (OS, редактор, браузеры, инструменты и т.п.)
* Расскажите о последнем проекте на Linux, который вы закончили.
* Расскажите о самой большой неудаче, которую вы допустили [какой-то период времени] и как вы изменились на сегодняшний день. Что вы вынесли из этого опыта?
* Почему мы должны выбрать вас?
* Какую роль играет DNS в сети?
* Что такое HTTP?
* Что такое HTTP прокси и как он работает?
* Опишите кратко как работает HTTPS?
* Что такое SMTP? Расскажите кратко сценарий доставки сообщения через SMTP.
* Что такое RAID? Что такое RAID0, RAID1, RAID5, RAID10?
* Что такое резервная копия 0-го уровня? Что такое инкрементальная резервная копия?
* Опишите иерархию файловой системы в Linux.


#### [[⬆]](#toc) <a name='simple'>Простые вопросы о Linux:</a>

* Какое имя и UID администратора?
* Как посмотреть все файлы в каталоге, включая скрытые?
* Какая команда в Unix/Linux удаляет каталог со всем его содержимым?
* Какая команда в Unix/Linux показывает свободную/используемую память? Существует ли свободная память в Linux?
* Как найти строку "my konfu is the best" в файлах каталога рекурсивно?
* Как подключиться к удаленному серверу или что такое SSH?
* Как получить все переменные окружения и как их можно использовать?
* Я получил "command not found" при запуске ```ifconfig -a```. Что может быть не так?
* Что произойдет, если я нажму TAB-TAB?
* Какая команда показывает доступное свободное пространство на диске в Unix/Linux?
* Какие команды вы знаете, которые могут быть использованы для проверки DNS записей?
* Какая команда Unix/Linux используется для изменения владельца файла, прав доступа к файлу?
* Что делает команда ```chmod +x FILENAME```?
* Что означают права 0750 для файла?
* Что означают права 0750 для каталога?
* Как добавить пользователя без прав входа в систему?
* Как добавить/убрать пользователя в/из группы?
* Что такое bash алиас?
* Как установить email для пользователя root?
* Что делает Ctrl+c?
* Что содержится в файле /etc/services?
* Как перенаправить STDOUT и STDERR в bash?
* Какая разница между UNIX и Linux?
* В чем разница между Telnet и SSH?
* Объясните три усредненных значения load average и что они означают? Какой командой можно посмотреть load average?
* Можете назвать букву в нижнем регистре, которая не является валидной опцией для GNU ```ls```?
* Что такое модуль ядра Linux?
* Расскажите по шагам как загрузить систему в однопользовательском режиме для решения проблем.
* Расскажите по шагам как вы будете решать проблему с ошибкой 404 в веб-приложении, которое вы обслуживаете.


#### [[⬆]](#toc) <a name='medium'>Вопросы среднего уровня о Linux:</a>

* Что делают следующие команды и как вы из будете использовать?
 * ```tee```
 * ```awk```
 * ```tr```
 * ```cut```
 * ```tac```
 * ```curl```
 * ```wget```
 * ```watch```
 * ```head```
 * ```tail```
* Что делает ```&``` в конце команды?
* Что делает ```& disown``` в конце команды?
* Что такое пакетный фильтр и как он работает?
* Что такое виртуальная память?
* Что такое swap и для чего он используется?
* Что такое A-запись, NS-запись, PTR-запись, CNAME-запись, MX-запись?
* Знаете ли вы еще какие-либо RR-записи и для чего они используются?
* Что такое Split-Horizon DNS?
* Что такое sticky bit?
* Что делает установленный на файл immutable bit?
* Какая разница между символическими и жесткими ссылками? Что произойдет если удалить символическую/жесткую ссылку?
* Что такое inode и какая информация хранится в inode?
* Как принудительно запустить проверку файловой системы при следующей перезагрузке?
* Что такое SNMP и для чего он используется?
* Что такое уровень запуска и как узнать текущий?
* Что такое SSH port forwarding?
* Какая разница между локальным и удаленным пробросом портов SSH?
* Какие шаги надо предпринять, чтоб добавить пользователя в систему не используя утилиты useradd/adduser?
* Что такое MAJOR и MINOR нумерация спец. файлов?
* Опишите команду mknod и когда она используется?
* Опишите сценарий, когда вы можете получить ошибку "filesystem is full", но 'df' показывает наличие свободного места.
* Опишите сценарий, когда вы удаляете файл,но 'df' не показывает, что место освободилось.
* Опишите как работает 'ps'.
* Что случиться, если процесс-потомок умрет и не будет процесса-родителя, ожидающего его и что в этом плохого?
* Объясните кратко каждое из состояний процесса.
* Как узнать какой процесс слушает указанный порт?
* Что такое зомби-процесс и какова его причина возникновения?
* Вы запускаете bash скрипт и хотите видеть его вывод на экране и одновременно сохранить этот вывод в файл. Как это сделать?
* Объясните, что делает echo "1" > /proc/sys/net/ipv4/ip_forward.
* Кратко объясните, какие шаги надо предпринять, чтоб создать и установить сертификат для сайта https://foo.example.com.
* Можно ли создать несколько HTTPS виртуальных хостов, используя один IP?
* Что такое wildcard сертификат?
* Какие типы файловых систем в Linux вам известны?
* В чем разница между процессом и потоком? И родительским и потомком процессами после системного вызова fork?
* В чем разница между exec и fork?
* Для чего используется ```nohup```?
* В чем разница между этими двумя командами?
 * ```myvar=hello```
 * ```export myvar=hello```
* Как много NTP севреров настроено в вашем локальном ntp.conf?
* Что означает колонка 'reach' в выводе ```ntpq-p```?
* Вам необходимо обновить ядро на 100-1000 серверах, как вы будете это делать?
* Как можно получить Host, Channel, IS, LUN для SCSI диска?
* Как можно ограничить использование памяти для процесса?
* Что такое быстрый поиск и замена в bash (^x^y)?
* Какие вы знаете альтернативные оболочки? Какую вы используете?
* Что такое tarpipe (или, как вы будете копировать все, включая жесткие ссылки и специальные файлы, с одного сервера на другой)?
* Как можно проверить, что пакет httpd уже был установлен?
* Как посмотреть содержимое установочного пакета?
* Как вы определите какой пакет лучше: openssh-server-5.3p1-118.1.el6_8.x86_64 или openssh-server-6.6p1-1.el6.x86_64?
* Как вы можете объяснить мне разницу между хранилищем, основанным на блоках и объектах?


#### [[⬆]](#toc) <a name='hard'>Сложные вопросы о Linux:</a>

* Что такое туннель и как вы можете обойти http прокси?
* В чем разница между IDS и IPS?
* Какие горячие клавиши вы используете регулярно?
* Что такое Linux Standard Base?
* Что такое атомарная операция?
* Вы только что настроили http сервер, который не запустился после рестарта. Что вы будете делать?
* Какие ключи содержатся в ~/.ssh/authorized_keys и для чего нужен этот файл?
* Я добавил свой публичный ключ в authorized_keys, но до сих пор получаю запрос пароля. Что может быть не так?
* Вы когда-нибудь собирали RPM, DEB или solaris пакеты?
* Что сделает ```:(){ :|:& };:``` с вашей системой?
* Как можно перехватить Linux сигнал из скрипта?
* Можно ли перехватить SIGKILL?
* Что происходит, когда ядро Linux запускает OOM killer и как он выбирает какой процесс необходимо убить в первую очередь?
* Опишите процесс загрузки Linux с максимально возможным количеством деталей, начиная с момента включения компьютера и заканчивая получением приглашения командной строки.
* Что такое закрытие в chroot?
* При попытке отмонтировать каталог получаем ошибку занятости, как найти какой PID держит каталог?
* Что такое LD_PRELOAD и когда он используется?
* Вы запустили бинарник и ничего не произошло. Как вы будете искать проблему?
* Что такое cgroups? Можете ли вы указать сценарий, когда это может быть использовано?
* Как можно удалить файл, имя которого содержит непечатные символы?
* Как можно увеличить/уменьшить приоритет процесса в Linux?
* Что такое run-levels в Linux?


#### [[⬆]](#toc) <a name='expert'>Вопросы экспертного уровня о Linux:</a>

* Запущенный процесс получает ```EAGAIN: Resource temporarily unavailable``` при чтении сокета. Как можно закрыть этот плохой сокет/файловый дескриптор без убивания процесса?


#### [[⬆]](#toc) <a name='network'>Вопросы по сетям:</a>

* Что такое localhost и почему ```ping localhost``` может не работать?
* В чем сходство между "ping" и "traceroute"? Как traceroute находит промежуточные хосты?
* Какая команда можно использовать для поиска всех открытых портов и/или соединений с сокетами на машине?
* Валидный ли IP адрес 300.168.0.123?
* Какие IP диапазоны/подсети являются частными или не маршрутизируемыми (RFC 1918)?
* Что такое VLAN?
* Что такое ARP и для чего используется?
* В чем разница между TCP и UDP?
* Какова цель шлюза по умолчанию?
* Какая команда используется для просмотра таблицы маршрутизации в Linux?
* TCP-соединение в сети может быть однозначно определено четырьмя вещами. Что это за вещи?
* Когда клиент использует бразер для подключения к веб-серверу, какие порты источника и назначения будут у этого соединения?
* Как можно добавить IPv6 адрес для конкретного интерфейса?
* Вы добавили IPv4 и IPv6 адреса на eth0 интерфейс. Ping на v4 адрес работает, но ping на v6 адрес дает ответ ```sendmsg: operation not permitted```. Что может быть не так?
* Что такое SNAT и когда он должен быть использован?
* Объясните, как можно войти по ssh на Linux сервер, который сбрасывает (DROP) все новые входящие пакеты, используя SSH туннель.
* Как вы будете противодействовать DDoS атаке?
* Как можно посмотреть содержимое ip пакета?
* Что такое IPoAC (RFC 1149)?


#### [[⬆]](#toc) <a name='mysql'>Вопрос о MySQL:</a>

* Как создать пользователя?
* Как предоставить права пользователю?
* В чем разница между 'left' и 'right' join?
* Объясните кратко разницу между InnoDB и MyISAM.
* Зачем надо запускать "mysql_secure_installation" после установки MySQL?
* Как проверить какие задачи запущены?
* Как вы делаете бекап MySQL?


#### [[⬆]](#toc) <a name='devop'>Вопросы о DevOps:</a>

* Как вы можете описать ваш workflow при создании скрипта?
* Что такое GIT?
* Что такое динамически/статически слинкованные файлы?
* Что делает "./configure && make && make install"?
* Для чего используется puppet/chef/ansible?
* Для чего используется Nagios/Zenoss/NewRelic?
* Для чего используется Jenkins/TeamCity/GoCI?
* В чем разница между контейнеризацией и виртуализацией?
* Как создать нового postgres пользователя?
* Что такое виртуальный IP адрес? Что такое кластер?
* Как вывести все строки печатных символов, присутствующих в файле?
* Как найти зависимости для библиотеки?
* Что такое Automake и Autoconf?
* ./configure вывела ошибку, что libfoobar не найдена в система, как вы будете исправлять это? Что может быть не так?
* Какие преимущества/недостатки у скриптов против компилируемых программ?
* Какая связь между непрерывной доставкой (continuous delivery) и DevOps?
* Каковы важные аспекты системы непрерывной интеграции и развертывания?
* Как бы вы включили совместное использование сетевых файлов в AWS, которые позволили бы экземплярам EC2 в нескольких зонах доступности обмениваться данными?


#### [[⬆]](#toc) <a name='fun'>Забавные вопросы::</a>

* Небрежный сисадмин запустил команду ```chmod 444 /bin/chmod``` - как будете исправлять проблему?
* Я потерял пароль пользователя root. Что мне делать?
* Я перезагрузил удаленный сервер, но спустя 10 минут все еще не могу зайти по SSH. Что может быть не так?
* Если бы вы попали на пустынный остров с 5 утилитами коммандной строки, то какие утилиты это были бы?
* Вы сталкиваетесь с случайным компьютером и, похоже, это консоль к мирозданию. Что первое вы наберете?
* Расскажите о креативном использовании ssh в вашей практике?
* Вы случайно удалили запущенный скрипт, как вы будете его восстанавливать?
* Что случится 19 января 2038 года?
* Как перезагрузить сервер когда команда reboot не доступна?


#### [[⬆]](#toc) <a name='demo'>Время демо:</a>

* Распакуйте test.tar.gz без использования man и google.
* Удалите все "*.pyc" файлы рекурсивно из testdir.
* Найдите все "my konfu is the best" во всех *.py файлах.
* Замените все вхождения "my konfu is the best" на "I'm a linux jedi master" во всех *.txt файлах.
* Проверьте доступность 443 порта на машине с IP X.X.X.X.
* Получите страницу http://myinternal.webserver.local/test.html при помощи telnet.
* Как отправить email без почтового клиента, только с помощью командной строки?
* Напишите метод ```get_prim``` в python/perl/bash/pseudo.
* Найдите все файлы, доступ к которым был осуществлен за последние 30 дней.
* Объясните следующую команду ```(date ; ps -ef | awk '{print $1}' | sort | uniq | wc -l ) >> Activity.log```
* Напишите скрипт, показывающий разницу двух каталогов.
* Из лог файла, содержащего ```<TIME> : [MESSAGE] : [ERROR_NO] - Human readable text``` выведите сумму/количество указанной ошибки, которая повторяется каждый час, или указанный час.


#### [[⬆]](#toc) <a name='references'>Другие ссылки:</a>

Некоторые вопросы 'заимствованы' из других замечательных ссылок, например:

* https://github.com/darcyclarke/Front-end-Developer-Interview-Questions
* https://github.com/kylejohnson/linux-sysadmin-interview-questions/blob/master/test.md
* http://slideshare.net/kavyasri790693/linux-admin-interview-questions
