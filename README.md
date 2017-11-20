Провайдер: ER-Telecom/ Дом.ru


Текст отчета blockcheck:

[O] Тестируем IPv4 DNS
	Через системный DNS:	 ['5.178.68.100', '92.255.241.100', '92.255.241.100', '92.255.241.100', '92.255.241.100', '92.255.241.100']
	Через Google DNS:	 ['5.178.68.100', '92.255.241.100', '92.255.241.100', '92.255.241.100', '92.255.241.100', '92.255.241.100']
	Через Google API:	 ['104.20.134.45', '104.20.135.45', '104.24.10.70', '104.24.11.70', '184.173.136.161', '195.8.215.136', '195.82.146.214', '5.178.68.100']
	Через недоступный DNS:	 ['92.255.241.100']
[☠] DNS-записи подменяются
[☠] DNS перенаправляется

[O] Тестируем HTTP (по настоящим IP-адресам сайтов)
	Открываем  http://a.putinhuylo.com/
[☠] Сайт не открывается, пробуем через прокси
[☠] Получен неожиданный ответ, скорее всего, страница-заглушка провайдера. Считаем заблокированным.
	Проверяем доступность через isup.me
[⁇] Ошибка при соединении с isup.me
	Открываем  http://furry.booru.org/
[✓] Сайт открывается
	Открываем  http://furry.booru.org/index.php?page=post&s=view&id=111173
[☠] Получен неожиданный ответ, скорее всего, страница-заглушка провайдера. Пробуем через прокси.
[☠] Получен неожиданный ответ, скорее всего, страница-заглушка провайдера. Считаем заблокированным.
	Проверяем доступность через isup.me
[☠] Сайт доступен, проблемы только у нас
	Открываем  http://pbooru.com/
[✓] Сайт открывается
	Открываем  http://pbooru.com/index.php?page=post&s=view&id=303026
[☠] Получен неожиданный ответ, скорее всего, страница-заглушка провайдера. Пробуем через прокси.
[☠] Получен неожиданный ответ, скорее всего, страница-заглушка провайдера. Считаем заблокированным.
	Проверяем доступность через isup.me
[☠] Сайт доступен, проблемы только у нас
	Открываем  http://rutracker.org/forum/index.php
[☠] Сайт не открывается, пробуем через прокси
[☠] Получен неожиданный ответ, скорее всего, страница-заглушка провайдера. Считаем заблокированным.
	Проверяем доступность через isup.me
[☠] Сайт доступен, проблемы только у нас

[O] Тестируем HTTPS
	Открываем  https://e621.net/
[☠] Сайт не открывается
	Открываем  https://lolibooru.moe/
[☠] Сайт не открывается
	Открываем  https://rutracker.org/forum/index.php
[☠] Сайт не открывается
	Открываем  https://www.dailymotion.com/
[☠] Сайт не открывается

[O] Тестируем обход DPI
	Пробуем способ «дополнительный пробел после GET» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «заголовок hOSt вместо Host» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «заголовок hoSt вместо Host» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «значение Host БОЛЬШИМИ БУКВАМИ» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «необычный порядок заголовков» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «отсутствие пробела между двоеточием и значением заголовка Host» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «перенос строки в заголовках в UNIX-стиле» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «перенос строки перед GET» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «табуляция в конце домена» на pbooru.com
[☠] Сайт не открывается
	Пробуем способ «точка в конце домена» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «фрагментирование заголовка» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «фрагментирование заголовка, hoSt и отсутствие пробела одновременно» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «дополнительный пробел после GET» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «заголовок hOSt вместо Host» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «заголовок hoSt вместо Host» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «значение Host БОЛЬШИМИ БУКВАМИ» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «необычный порядок заголовков» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «отсутствие пробела между двоеточием и значением заголовка Host» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «перенос строки в заголовках в UNIX-стиле» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «перенос строки перед GET» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «табуляция в конце домена» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «точка в конце домена» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «фрагментирование заголовка» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «фрагментирование заголовка, hoSt и отсутствие пробела одновременно» на rutracker.org
[✓] Сайт открывается

[!] Результат:
[⚠] Ваш провайдер подменяет DNS-записи и перенаправляет сторонние IPv4 DNS-серверы на свой.
 Вам следует использовать шифрованный канал до DNS-серверов, например, через VPN, Tor, HTTPS/Socks прокси или DNSCrypt.
[⚠] Ваш провайдер полностью блокирует доступ к HTTPS-сайтам из реестра.
[⚠] У вашего провайдера "полный" DPI. Он отслеживает ссылки даже внутри прокси, поэтому вам следует использовать любое шифрованное соединение, например, VPN или Tor.

Скриншот LinkedIn:

![img](https://github.com/gib130/DPI/blob/master/link.png)

