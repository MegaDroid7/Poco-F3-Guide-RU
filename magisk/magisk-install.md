---
description: Моя прелесть!
---

# 🎭 Установка Magisk

Если вы когда-то прошивали телефон в прошлом десятилетии, то вы слышали о SuperSU. Magisk - тот же SuperSU, только лучше.

{% hint style="info" %}
Magisk - модификация для ОС, которая позволяет получить полный доступ к системным файлам.
{% endhint %}

Данная модификация в основном нужна для того, чтобы устанавливать модули и предоставлять доступ к системе другим приложениям.

Самое интересное - это то, что модули работают бессистемным (systemless) образом, никак не затрагивая систему. То есть, если модуль вызвал ошибку в системе, то вы сможете просто удалить этот модуль любым удобным вам способом.

Есть 2 способа установки Magisk'а:

{% tabs %}
{% tab title="Через рекавери" %}
Рекавери TWRP от SKKK и OrangeFox изначально поставляются с возможностью установки Magisk из меню "Дополнительное" или "Дополнения Fox" в меню OrangeFox.

Но если у вас нету такого в вашем Рекавери, то:

1. Скачайте последний APK Magisk ([GitHub](https://github.com/topjohnwu/Magisk/releases))
2. Перезапуститесь в Рекавери
3. Установите скачанный файл (Да-да, выбирайте APK-файл)
4. Перезагрузите устройство

Magisk установлен!
{% endtab %}

{% tab title="Через патч boot-раздела (HentaiOS)" %}
{% hint style="danger" %}
Не перепутайте vendor\_boot с boot! Это может привести к окирпичиванию устройства!
{% endhint %}

Вы хотите установить Magisk на HentaiOS, а он не хочет запускать стороннее рекавери? Тогда:

1. Скачайте последний APK Magisk ([GitHub](https://github.com/topjohnwu/Magisk/releases))
2. Скачайте на устройство boot образ прошивки (поставляется вместе с прошивкой)
3. Установите Magisk на телефон (В виде приложения)
4. Выберите "Установка" справа от пункта Magisk
5. Выберите "Пропатчить boot образ"
6. Выберите заранее скачаный boot образ
7. Скачайте пропатченный образ на ПК
8. Перезагрузите телефон в режим Fastboot
9. Откройте ADB и прошейте образ:

```
fastboot flash boot_ab magisk-patched-boot.img
```

После этих действий загрузитесь в прошивку и установите приложение Magisk. Root-права должны появиться.
{% endtab %}
{% endtabs %}
