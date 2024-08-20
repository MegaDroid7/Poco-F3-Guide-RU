---
description: >-
  Самая популярная прошивка на основе MIUI China ROM, которая содержит все фишки
  китайской прошивки + русскую локализацию.
---

# 🇨🇳 xiaomi.eu

Если вы хотели попробовать чистый MIUI, то вы по адресу. xiaomi.eu считается хорошей MIUI прошивкой. Вы получите не только MIUI лаунчер и звонилку с записью вызовов, но ещё и китайское приложение "Темы" с возможностью импорта кастомной темы.

{% hint style="success" %}
Последние сборки MIUI 14/HyperOS от команды xiaomi.eu начали поставляться с гибридными способами установки. Выбирайте любой удобный вам представленный ниже способ установки прошивки.
{% endhint %}

{% tabs %}
{% tab title="Fastboot" %}
### Установка:

1. Скачайте последнюю прошивку ([Ссылка на форум](https://xiaomi.eu/community/threads/hyperos-1-0-stable-release.71170/))
2. Распакуйте архив
3. Перезапустите телефон в режиме Fastboot [button-combinations.md](../beginning/button-combinations.md "mention")
4. Подключите телефон к компьютеру
5. Запустите скрипт установки прошивки в соответствии с вашей ОС (Для Windows это: windows\_fastboot\_first\_install\_with\_data\_format.bat)
6. Согласитесь на установку прошивки и на то, что все данные будут утеряны.
7. Ожидайте конца прошивки.



### Обновление:

1. Скачайте последнюю прошивку ([Ссылка на форум](https://xiaomi.eu/community/threads/hyperos-1-0-stable-release.71170/))
2. Распакуйте архив
3. Перезапустите телефон в режиме Fastboot [button-combinations.md](../beginning/button-combinations.md "mention")
4. Подключите телефон к компьютеру
5. Запустите скрипт обновления прошивки в соответствии с вашей ОС (Для Windows это: windows\_fastboot\_update.bat)
6. Ожидайте конца обновления
{% endtab %}

{% tab title="Recovery" %}
### Установка:

1. Скачайте прошивку ([Ссылка на форум](https://xiaomi.eu/community/threads/hyperos-1-0-stable-release.71170/))
2. Скачайте рекавери для вашего телефона [#ssylki-dlya-skachivaniya-recovery](../beginning/recovery-install.md#ssylki-dlya-skachivaniya-recovery "mention")
3. Перезапустите телефон в режиме Fastboot
4. Подключите телефон к компьютеру
5.  В окне ADB выполните команду:

    ```
    fastboot boot <recovery_filename>.img
    ```
6. Расшифруйте пользователя, используя пароль от телефона, если вы используйте блокировку устройства.
7. Загрузите прошивку в память телефона.
8. Установите прошивку.
9. Перезапустите телефон в рекавери.
10. Выполните Format Data через 'yes'
11. Перезагрузитесь в систему.



### Обновление:

1. Скачайте прошивку ([Ссылка на форум](https://xiaomi.eu/community/threads/hyperos-1-0-stable-release.71170/))
2. Скачайте рекавери для вашего телефона [#ssylki-dlya-skachivaniya-recovery](../beginning/recovery-install.md#ssylki-dlya-skachivaniya-recovery "mention")
3. Перезапустите телефон в режиме Fastboot [button-combinations.md](../beginning/button-combinations.md "mention")
4. Подключите телефон к компьютеру
5.  В окне ADB выполните команду:

    ```
    fastboot boot <recovery_filename>.img
    ```
6. Расшифруйте пользователя, используя пароль от телефона, если вы используйте блокировку устройства.
7. Установите прошивку.
8. Перезагрузитесь в систему.
{% endtab %}
{% endtabs %}
