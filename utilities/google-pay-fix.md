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
3. Включите Zygisk
4. Активируйте DenyList
5. Откройте настройки DenyList
6. Найдите приложение Mir Pay и внесите его в список Deny List
7. Перезагрузите устройство
{% endtab %}

{% tab title="Гайд для Google Pay" %}
1. Скачайте модуль safetynet fix ([GitHub](https://github.com/kdrag0n/safetynet-fix/releases))
2. Откройте Magisk
3. Установите модуль safetynet fix
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