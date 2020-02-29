# my-progs
chat Telegram bot on python to receive information about transactions in quick

1. Нужно создать чат бот в Телеграмме.
    В строку поиска ввести BotFather, открыть его, нажать на Старт или символ слэш "/"
    в меню выбрать /newbot create new bot и придумать название,
    после того как бот будет создан, на экране появится информация с текстом, где будет указан токен в виде -
    "1234567890: AAggddjdjdjdgu33333iTBFFddd"
    нажмите на него, он автоматически скопируется в буфер обмена, сохраните его, он понадобится далее.
    
2. Получить свой ID (идентификационный номер в Телеграмме). Найти бота наподобие @getmyid_bot, присоединиться к нему,
   нажать Старт,  и бот пришет ID. Это номер в виде "123456789". Его тоже надо сохранить. 

3. Установить Python 3.7 или старше (младше не тестировал) на компьютер, где работает Quik, при установке отметить галочку PATH, 
   чтобы скрипты Питона могли запускаться из любого каталога.

4. Установить библиотеку Telebot для Python для работы с Телеграмм. 
   Запустить командную строку Windows (Пуск-->Выполнить-->ввести команду cmd и нажать Enter.  
   Далее, в командной строке выполнить команду pip install pytelegrambotapi
   
5. В каталог с программой Quik скопировать нужные файлы -
   скрипты LUA - "socket_server.lua" и "socket.lua", создав и разместив их в папке "lua" 
   файл библиотеки Socket - "core.dll" , создав и разместив его в папке  "socket"

6. Запустить IDLE Python, из меню открыть файл "soket_quik_telegram.py", и отредактировать его, 
   вставив в соответствующие места (написано в комментариях  к коду) токен своего бота и свой ID,
   затем запустить на выполнение.
   Потом можно запускать кликнув на файл два раза (он запустится в командной строке без использования IDLE).

7. в программе Quik в меню "Сервисы" открыть подменю "Lua скрипты", там добавить и запустить файл "socket_server.lua"

Ньюансы.

Скрипт Python при попытке отправить сообщение в Телеграмм может завершаться с ошибкой из за проблем с блокировкой Телеграмм.
В этом случае нужно в коде скрипта раскомментировать строки, относящиеся к подключению через прокси сервер.
Возможно потребуется поменять прокси сервер, если он перестанет работать.



   
