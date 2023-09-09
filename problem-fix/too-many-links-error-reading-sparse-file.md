---
description: AMD moment.
---

# Too many links / Error reading sparse file

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F5H3iTS7MbzmtXt2O6afq%2Fuploads%2FREKftOCMvxUhODE9XG0r%2Fimage.png?alt=media&#x26;token=7dc89d4e-5921-4fa3-9b8a-12eae9d88a66" alt=""><figcaption><p>Ошибка too many links</p></figcaption></figure>

Ошибка Too many links может возникать так же, как и ошибка Error reading sparse file (Если процесс был остановлен на Sending 'super'). Проблема заключается в процессоре AMD. Для решения данной ошибки, вам нужно открыть отдельное окно adb и дошить ручками оставшиеся файлы, главное не забыть перезапустить телефон в режим fastboot.

Или же мы поступим "элегантным" способом:

1. Создадим новый файл любоеназвание.bat (Пример: windows-befote-cust.bat)
2. Скопируем всё содержимое из файла windows\_fastboot\_first\_install\_with\_data\_format.bat в наш новый файл
3. Убираем всё лишнее до того момента, где программа застопорилась (в моём случае всё, что выделил синим - под удаление) ​![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F5H3iTS7MbzmtXt2O6afq%2Fuploads%2FpLdFzQUC7nyje6rvvfQo%2Fimage.png?alt=media\&token=ed0c4d7e-ffb4-4357-87fc-99b72fbd20e2)​
4. Сохраняем файл
5. Перезапускаем устройство в fastboot (даже если он уже в fastboot его нужно снова перезапустить)
6. Запускаем его
7. ... Profit!

Если же ваш телефон не обнаруживается в системе, то попробуйте выполнить данные пункты:

1. Установите [драйвера](https://disk.yandex.ru/d/Afu9It6tdCybAw) (QDLoader и ADB Driver Lite)
2. Замените провод или используйте оригинальный
3. Подключите телефон к материнской плате компьютера
4. Подключите телефон к USB-хабу (помогает в 99% случаев)
5. Установите [фикс](https://disk.yandex.ru/d/W4JlOBPyfh4HBQ) для AMD процессоров ([источник](https://forum.xda-developers.com/t/fix-fastboot-issues-on-ryzen-based-pcs.4186321/))
