# **ЧТО ТАКОЕ GIT?**

![тут лого git](gitlogo.jpeg)

  ## 1. **ОБЩЕЕ ОПИСАНИЕ**


Git – распределенная система контроля версиями, была создана  Линусом Торвальдсом, чтобы управлять разработкой ядра Линукс. На сегодняшний день многие проекты используют Git. Среди них PHP, jQuery, Wine, Android, Qt, Drupal и другие.

Система выпущена под лицензией GNU GPL и является, по сути, набором программ, очень удобных для разработки. Поддерживает нелинейную историю разработки проекта, фиксируя образ системы проекта на данный момент, т.е. то, как выглядят все файлы разработки в конкретный момент времени. Если какой-то файл не изменился с течением времени, он не дублируется, на него просто делается ссылка. Это позволяет повысить эффективность системы.

Устанавливать Git можно и на Linux,  и на Mac, и на Windows. Главная задача  - это правильная настройка системы. Git достаточно гибкая, что даёт возможность реализации практически любых клиентов с интерфейсом по желанию.

Перед началом командной разработки создается репозиторий с доступом к нему по сети. Когда разработчик посчитал, что нужный код готов и написан, он выгружает его в репозиторий. Код становится доступным остальным участникам команды, которые, обратившись к репозиторию, получают актуальную версию. Таким образом, Git хранит историю проекта: авторство и историю изменения вашей разработки с возможностью отката к предыдущей версии. Присутствует возможность контроля доступа к коду. Большим удобством является возможность работы с несколькими версиями разработки одновременно.

Большинство операций системы контроля версий Git производится в локальном репозитории. История проекта также хранится на локальном ПК и делает доступ к ней максимально быстрым. Постоянное соединение с сервером системе не требуется, поэтому вы можете работать независимо от наличия постоянного канала связи. Это актуально в случаях плохого интернет-коннекта. Весьма полезной функцией Git-a является отслеживание целостности файлов. Система постоянно следит за контрольными сумами, что даёт большую надежность и актуальность текущего проекта.

Несомненное удобство системы контроля версий – это ветвление: возможность параллельной разработки нескольких версий ПО.   На простом примере это можно сравнить с большим паззлом, например, на 3 тысячи кусков, который собирают 10 человек. Каждый участник сборки складывает свой кусок картинки и, когда он её сложит, этот кусок (ветку) ему необходимо прикрепить к общей картинке. Теперь представьте, что этот паззл с картинкой автомобиля. Пока вы собирали свой кусок, у автомобиля поменялся дизайн фары – так вот та ветка, которая отвечала за фару, имеет возможность быть выключенной и быть собранной по-другому и вставиться целиком. Что же такое Git - его смысл и заключается как раз в этом: есть центральная линия, на которой всё понятно и всё работает. В нашем случае это рабочая оттестированная версия программы, которую в любой момент можно показать заказчику или отдать пользователям, и есть боковые ветки, где производится доработка или изменения, которую, кроме самих разработчиков и лиц, имеющих доступ к коду, не видит никто.

Если в процессе работы с ветками случается конфликт при слиянии версий, то вы имеете возможность разобраться с его причиной, принять решение о слиянии или не слиянии того, что есть в главной ветке и тем, что наработали вы и дать конечные исправления.

Возникающие ошибки легко отследить и установить, где, когда, кем и почему они были сделаны. С изменениями также весьма удобно работать – в системе присутствует широкая возможность комментирования.

Многие пользователи почему-то испытывают боязнь в создании новых веток. Этого делать не нужно,  как раз наоборот: все изменения следует проводить сначала на отдельной ветке, потом выкладывать их в основную и только после этого уже принимать решение о внедрении в стабильную версию программы.

Существуют не только графические, но и консольные версии git-клиентов. Они в большинстве случаев удобны для использования на серверах. Консольная версия отличается только отсутствием графического интерфейса. Все остальные действия и команды – аналогичны.

В результате, используя Git, вы получаете удобную среду, как для командной работы, так и для одиночной, имея под рукой возможность сохранять несколько версий программы, держать отдельно главную ветвь, оттестированную и работоспособную и видеть всю историю написания проекта, с возможностью откатиться куда вам необходимо или изменить направление разработки с любой существующей точки.
gi

# 2. ПОЛЕЗНЫЕ ССЫЛКИ

* https://habr.com/ru/post/542616/ 

* https://gb.ru/posts/soveti-pro-git

* https://learngitbranching.js.org/?locale=ru_RU

# 3. УСТАНОВКА

Основой интерфейс для работы с Git-ом является консоль/терминал. Это не совсем удобно, тем более для новичков, поэтому предлагаю поставить дополнительную программу с графическим интерфейсом (кнопками, графиками и т.д.). О них я расскажу чуть позже.

Но для начала, все же установим сам Git.

Windows. Проходим по [этой ссылке](https://gitforwindows.org/), выбираем под вашу ОС (32 или 64 битную), скачиваем и устанавливаем.

Для Mac OS. Открываем терминал и пишем:

* Если установлен Homebrew
brew install git

* Если нет, то вводим эту команду. 
git --version

После этого появится окно, где предложит установить Command Line Tools (CLT).
Соглашаемся и ждем установки. Вместе с CLT установиться и git

Linux. Открываем терминал и вводим следующую команду.

* Debian или Ubuntu
sudo apt install git

* CentOS
sudo yum install git

# 4. НАСТРОЙКА

Вы установили себе Git и можете им пользоваться. Давайте теперь его настроим, чтобы когда вы создавали commit, указывался автор, кто его создал.

Открываем терминал (Linux и MacOS) или консоль (Windows) и вводим следующие команды.

* Установим имя для вашего пользователя
* Вместо <ваше_имя> можно ввести, например, Grisha_Popov
Кавычки оставляем

git config --global user.name "<ваше_имя>"

* Теперь установим email. Принцип тот же.
 git config --global user.email "<адрес_почты@email.com>"

# 5. СОВМЕСТНАЯ РАБОТА

Представим, что вы с друзьями придумали проект, с "блэкджеком" и ... Вы разделили обязанности. Кто-то будет делать авторизацию и регистрацию, а кто-то функционал вывода новостей. Для этого вам пригодится ветвление.


Ветка - это набор commit (кружок), которые идут друг за другом. У ветки есть название, основную ветку чаще всего называют master (на картинках будет называться main) . Если говорить простыми словами, то ветка master - это наш проект.

Другие ветки - это отдельное место для реализации нового функционала или исправление багов (ошибок) нашего проекта. То есть, с отдельной веткой вы делаете что угодно, а затем сливаете эти изменения в основную ветку master.

 Не рекомендую создавать commit напрямую в master . Лучше для этого заводить новую ветку и все изменения писать там.

Для того, чтобы создать новую ветку вводим:

git branch <название_ветки>

или вот так

git checkout -b <название_ветки>

Эти команды делают тоже самое, только второй вариант позволяет сразу переключиться в новую ветку. Вносить изменения в новую ветку можно сразу после ее создания.

При создании новой ветки, старайтесь называть ее кратким и ёмким именем. Чтобы сразу было понятно, что именно изменялось по проекту. Если вы используете, какую-нибудь систему для ведения задач, то можете в начале названия ветки указывать ID задачи, чтобы можно было легко найти, на основе какой задачи была создана ветка. Например вот так:

3424_fix_catalog_ajax

В каждом новом commit следует оставлять коммент и в нем описывать суть изменений.

Переключаться между ветками можно такой командой:

git checkout <название_ветки>
После того, как вы завершили работу над своей задачей, ветку можно слить в master . Для этого нужно переключиться в ветку master и выполнить следующую команду:

* Переключаемся в master

git checkout master

* Обновляем локальную ветку с сервера

git pull origin master

* Делаем merge вашей ветки, в ветку в которой вы находитесь
В данном примере это master

git merge <название_ветки>

❗️ Перед тем как сливать новый merge , стоит обновить локальную ветку master , во избежания дальнейших проблем.

Команда merge берет все изменения из ветки (например bugFix) и добавляет их в ветку master.

Для того чтобы посмотреть текущее состояние ветки, например, какие файлы добавлены или не добавлены для создания commit, можно выполнить команду:

git status

Другие пользователи не увидят вашу ветку, пока она не будет отправлена на удаленный репозиторий. Поэтому, после того как вы слили все изменения в master , нужно отправить их в GitHub. Для этого обязательно нужно находиться в ветке master :

git checkout master

* Отправляем наши изменения в GitHub

git push origin master

Теперь все ваши изменения, в ветке master улетели в GitHub. Таким же образом, можно отправить любую другую ветку:

git checkout <название_ветки>

git push origin <название_ветки>

Совет. Каждый коммит, лучше заливать сразу в удаленный репозиторий. Никто не застрахован, поломки собственного ПК. Поэтому чтобы не потерять все наработки, не забывайте сливать ваши изменения на GitHub.


Как же теперь другой человек получит все ваши изменения?
Для этого вам понадобиться GitHub или любой другой сервис для хранения кода. В прошлой статье я рассказывал как отправить код в GitHub. Сейчас я покажу, как его скопировать обратно себе на компьютер.

Если у вашего друга раньше не было проекта, то ему придется его "клонировать" себе:

git clone <адрес_репозитория>

 Адрес репозитория на GitHub можно получить, нажав на зеленую кнопку Code

После выполнения команды, в папке где появиться проект и ваш друг сможет с ним работать. Все ветки и их история также подтянуться.

Теперь самое главное
Перед тем, как создавать новый функционал и новую ветку, стоит обновить master на вашем устройстве. Для этого нужно находиться в этой ветке и выполнить следующую команду:

 Переключаемся в master
 
 git checkout master
  
Подтягиваем изменения из репозитория GitHub

git pull origin master

Таким же образом можно актуализировать любую другую ветку, заменив название ветки master на вашу.

Для обновления всех веток сразу, можно использовать такую, команду, но не рекомендую:

git pull

Теперь можно создавать новую ветку и кодить.