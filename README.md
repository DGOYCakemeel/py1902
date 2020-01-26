# py1902
I just love ""bold text""
Italicized text is the "cat's meow"
this text is __really important___


1.  Open the file containing the Linux mascot.
2.  Marvel at its beauty.

    ![Tux, the Linux mascot](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Python-logo-notext.svg/1200px-Python-logo-notext.svg.png)

3.  Close the file.


1.python /path/to/script.py
2./path/to/script.py
python /path/to/script.py работает, если файл является исполняемым или нет shebang ( #!/usr/bin/env python ) в #!/usr/bin/env python скрипта – хорошая практика, но не нужна /path/to/script.py работает, если скрипт исполняемый требуется shebang ( #!/usr/bin/env python ) script.py работает, если скрипт находится в $ PATH сценарий должен быть исполняемым имя файла должно иметь расширение требуется shebang ( #!/usr/bin/env python ) script работает, если скрипт находится в $ PATH сценарий должен быть исполняемым имя файла не должно иметь расширения требуется shebang ( #!/usr/bin/env python )

# Heading level 1

Просмотр и изменение файлов
cat. Когда команда используется с одним текстовым файлом (вот так: cat путь_к_файлу), она отображает его содержимое в окне терминала. Если указать два и больше файлов, cat путь_к_файлу_1 путь_к_файлу_2, она склеит их. Если ввести cat путь_к_файлу_1 > новый_файл, она объединит содержимое указанных файлов в новый файл.
chmod. Позволяет изменять права доступа к файлу. Может пригодиться, если вы хотите внести изменения в системный файл.
chown. Изменяет владельца файла. Следует выполнять с правами суперпользователя.
file. Выводит информацию об указанном файле.
nano. Открывает простой текстовый редактор. Можно создать новый текстовый файл или открыть существующий: nano путь_к_файлу.
rename. Переименовывает файл или несколько файлов. Команду можно использовать и для массового переименования файлов по маске.
touch. Изменяет дату последнего открытия или модификации указанного файла.
wget. Загружает файлы из интернета в терминальную папку.
zip. Распаковывает и сжимает архивы.
Создание и удаление файлов и папок
mkdir. Создаёт новую папку в текущей терминальной папке или в указанной папке: mkdir путь_к_папке.
rmdir. Удаляет указанную папку.
rm. Удаляет файлы. Может удалить как отдельный файл, так и группу, соответствующую определённым признакам.
Копирование и перемещение файлов
cp. Создаёт копию указанного файла в папке терминала: cp путь_к_файлу. Или вы можете указать назначение cp путь_к_файлу путь_для_копии.
mv. Перемещает файл из одной папки в другую. Вы можете указать имя для перемещаемого файла. Забавно, но в Linux эта команда может использоваться и для переименования файлов. Просто укажите ту же папку, где находится файл, и другое имя.
Поиск файлов
find. Поиск файлов по определённым критериям, таким как имя, тип, размер, владелец, дата создания и модификации.
grep. Поиск текстовых файлов, содержащих определённые строки. Критерии очень гибко настраиваются.
locate. Поиск файлов и папок, чьи названия подходят запросу, и отображение их путей в файловой системе.
Команды Linux для работы с разделами
lsblk. Эта команда демонстрирует, какие диски есть в вашей системе и на какие разделы они поделены. Также команда отображает имена ваших разделов и накопителей, в формате sda1, sda2 и так далее.
mount. Монтирует накопители, устройства или файловые системы Linux, чтобы вы могли с ними работать. Обычно устройства подключаются автоматически, как только вы щёлкнете по ним в файловом менеджере. Но иногда может понадобиться примонтировать что-то вручную. Вы можете подключать что угодно: диски, внешние накопители, разделы и даже ISO-образы. Эту команду нужно выполнять с правами суперпользователя. Чтобы примонтировать имеющийся диск или раздел, введите mount sdX.
umount. Демонтирует файловые системы. Команда umount sdX отключит файловую систему внешнего носителя, чтобы вы могли извлечь его.
dd. Эта команда копирует и преобразовывает файлы и разделы. У неё множество различных применений. Например, dd if=/dev/sda of=/dev/sdb сделает точную копию раздела sda на разделе sdb. dd if=/dev/zero of=/dev/sdX затрёт содержимое указанного носителя нулями, чтобы информацию было невозможно восстановить. А dd if=~/Downloads/ubuntu.iso of=/dev/sdX bs=4M сделает загрузочный носитель из скачанного вами образа с дистрибутивом.
Команды Linux для управления системой
df. Отображает объём вашего диска, и сколько на нём осталось свободного места.
free. Отображает объём доступной и занятой оперативной памяти.
uname. Отображает сведения о системе Если ввести uname, терминал сообщит только Linux. Но команда uname -a выводит сведения об имени компьютера и версии ядра.
uptime. Сообщает, как долго запущена ваша система.
whereis. Отображает расположение исполняемого файла нужной программы.
whoami. Называет имя пользователя.
Команды Linux для управления пользователями
useradd. Регистрирует нового пользователя. Введите useradd имя_пользователя, и пользователь будет создан.
userdel. Удаляет учётную запись и файлы пользователя.
usermod. Изменяет учётную запись пользователя. Может переместить домашнюю папку пользователя или назначить дату, когда учётная запись будет заблокирована.
passwd. Изменяет пароли учётных записей. Обычный пользователь может изменить пароль только своей учётной записи, суперпользователь может изменить пароль любой учётной записи.
Команды Linux для управления сетью
ip. Многофункциональная команда для работы с сетью. Команда ip address show выводит сведения о сетевых адресах, ip route управляет маршрутизацией и так далее. Давая команды ip link set ethX up, ip link set ethX down, можно включать и выключать соединения. У команды ip много применений, так что перед её использованием лучше ознакомиться с руководством или ввести ip --help
ping. Показывает, подключены ли вы к сети, и помогает определить качество связи.
И ещё кое-что
Напоследок — главные команды Linux. Они выводят на экран корову, которая может разговаривать с вами (не спрашивайте, что употребляют разработчики).

cowsay что_угодно. Корова произнесёт то, что вы ей скажете.
fortune | cowsay. Корова выдаст умную (или не очень) мысль или цитату.
cowsay -l. Выводит список всех животных, которые могут быть отображены в терминале. Если вы вдруг не любите коров.
fortune | cowsay -f животное_из_списка. Животное на ваш выбор начинает сыпать цитатами, иногда уместными.
sudo apt-get install fortunes fortune-mod fortunes-min fortunes-ru. Заставит весь зоопарк говорить по-русски. Без этого животные цитируют Твена и Уайльда в оригинале.
Это далеко не все команды Linux. Если вам нужно узнать в деталях параметры и способы применения команд Linux, вы можете воспользоваться встроенным руководством. Наберите man ваша_команда или ваша_команда --help.
![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Python-logo-notext.svg/1200px-Python-logo-notext.svg.png)
