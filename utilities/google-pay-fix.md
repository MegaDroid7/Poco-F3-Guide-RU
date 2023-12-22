---
description: Я хочу платить деньги, а телефон не даёт(
---

# 💳 Фикс платежных приложений (Google Pay, MIR Pay)

После разблокировки устройства вы можете заметить, что платежные приложения перестали работать. Как пофиксить эту проблему и начать платить с разблокированным телефоном?

{% hint style="info" %}
Во многих кастомных прошивках данная проблема исправлена по умолчанию. В описании таких прошивок обычно пишут: "safetynet pass by default".

Но после установки Magisk данная проблема появляется снова, и тогда уже нужно будет применить данный гайд.
{% endhint %}

Для обоих гайдов нужен Magisk. [Как его установить?](../magisk/magisk-install.md)

{% tabs %}
{% tab title="Гайд для Mir Pay" %}
1. Откройте Magisk
2. Откройте настройки
3. Активируйте Zygisk
4. Скройте приложение Magisk (Пункт: Скрытие приложения Magisk)
5. Установите модуль [PlayIntegrityFix](https://github.com/chiteroman/PlayIntegrityFix)
6. Установите [LSPosed](https://github.com/LSPosed/LSPosed)
7. Установите [mirpaysecurity](https://github.com/Xposed-Modules-Repo/ru.bluecat.mirpaysecurity)
8. Вернитесь в настройки
9. Активируйте DenyList
10. Откройте настройки DenyList
11. Найдите приложение Mir Pay и внесите его в список Deny List
12. Перезагрузите устройство
13. Зайдите в LSPosed (Появится уведомление после установки)
14. Активируйте mirpaysecurity
{% endtab %}

{% tab title="Гайд для Google Pay" %}
1. Скачайте модуль Play Integrity fix ([GitHub](https://github.com/chiteroman/PlayIntegrityFix))
2. Откройте Magisk
3. Установите модуль Play Integrity fix
4. Откройте настройки
5. Включите Zygisk
6. Активируйте DenyList
7. Откройте настройки DenyList
8. Нажмите на три точки и включите галочку "Системные приложения"
9. Напишите в поиске "Wallet", Выберите "Google Pay / Кошелёк"
10. Напишите в поиске "gms", Выберите "Сервисы Google Play"
11. Напишите в поиске "vending", Выберите "Play Маркет"
12. Перезагрузите телефон

Этих действий достаточно, чтобы Google Pay заработал на вашем устройстве с Magisk. Но если Google Pay так и не заработал после всех этих действий, то очистите кэш Сервисов Google Play, Play Маркета и Google Pay / Кошелька. После этого Google Pay должен заработать.
{% endtab %}
{% endtabs %}
