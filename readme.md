## Настройка

Вы установили себе Git и можете им пользоваться. Давайте теперь его настроим, чтобы когда вы создавали commit, указывался автор, кто его создал.

Открываем терминал (Linux и MacOS) или консоль (Windows) и вводим следующие команды.

# 3. УСТАНОВКА

Основой интерфейс для работы с Git-ом является консоль/терминал. Это не совсем удобно, тем более для новичков, поэтому предлагаю поставить дополнительную программу с графическим интерфейсом (кнопками, графиками и т.д.). О них я расскажу чуть позже.

Но для начала, все же установим сам Git.

Windows. Проходим по [этой ссылке](https://gitforwindows.org/), выбираем под вашу ОС (32 или 64 битную), скачиваем и устанавливаем.

Для Mac OS. Открываем терминал и пишем:

#Если установлен Homebrew
brew install git

#Если нет, то вводим эту команду. 
git --version
#После этого появится окно, где предложит установить Command Line Tools (CLT).
#Соглашаемся и ждем установки. Вместе с CLT установиться и git
Linux. Открываем терминал и вводим следующую команду.

* Debian или Ubuntu
sudo apt install git

* CentOS
sudo yum install git
Настройка
Вы установили себе Git и можете им пользоваться. Давайте теперь его настроим, чтобы когда вы создавали commit, указывался автор, кто его создал.

Открываем терминал (Linux и MacOS) или консоль (Windows) и вводим следующие команды.

#Установим имя для вашего пользователя
#Вместо <ваше_имя> можно ввести, например, Grisha_Popov
#Кавычки оставляем
git config --global user.name "<ваше_имя>"

#Теперь установим email. Принцип тот же.
git config --global user.email "<адрес_почты@email.com>"

* Установим имя для вашего пользователя
Вместо <ваше_имя> можно ввести, например, Grisha_Popov
Кавычки оставляем
git config --global user.name "<ваше_имя>"

* Теперь установим email. Принцип тот же.
git config --global user.email "<адрес_почты@email.com>"

Новый текст новый текст новый текст

