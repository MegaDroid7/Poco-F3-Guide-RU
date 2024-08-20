---
description: >-
  Одна из стабильных прошивок на Чпоко. Советуется для повседневного
  использования.
---

# 🪿 PixelOS

Как вы уже прочитали выше, эта прошивка полностью стабильна, ~~зуб даю.~~ Она полностью повторяет ту операционную систему, которая поставляется вместе с устройствами Google Pixel. Поэтому она и называется - PixelOS.

Помимо этого, вместе с прошивкой поставляется камера MIUI, что позволяет использовать все функции основной камеры, как на стоке.

### Установка

{% hint style="warning" %}
В угловых скобках указан тип файла, который нужно будет указать, а не то, что вам нужно вводить. Если вы видите \<vendor\_boot>.img, а ваш файл называется vendor\_boot-alioth-20240528.img, то ваша команда будет следующей, при условии, что файл находится в той же директории, что и adb:

fastboot flash vendor\_boot vendor\_boot-alioth-20240528.img
{% endhint %}

1. Скачайте последнюю сборку PixelOS [здесь](https://pixelos.net/download/alioth) (нажать на кнопку Download под Latest Build)
2. Скачайте последние boot и vendor\_boot [здесь](https://sourceforge.net/projects/pixelos-releases/files/fourteen/alioth/recovery/) (тупо первые 2 файла)
3. Перезапустите телефон в режим Fastboot
4.  Установите vendor\_boot командой:

    ```
    fastboot flash vendor_boot <vendor_boot>.img
    ```
5.  Установите boot в рабочий раздел командой:

    ```
    fastboot flash boot <boot>.img
    ```
6.  Перезагрузитесь в рекавери:

    ```
    fastboot reboot recovery
    ```
7. Сделайте Wipe данных следуя данной последовательности: Factory reset > Format data/factory reset > Format data > Back to Main menu > Advanced > Reboot to Recovery
8. Включите ADB Sideload следуя данной инструкции: Apply update > Apply from ADB
9.  Установите прошивку:

    ```
    adb sideload <PixelOS_alioth>.zip
    ```
10. Установите последний доступный [Firmware](../beginning/firmware.md) региона MI:

    ```
    adb sideload <fw_alioth>.zip
    ```
11. Перезагрузите телефон.

### Ядро

Мейнтейнер категорически советует использовать ядра Nexus (оно и дело понятно, ядро от самого мейнтейнера). С другими ядрами (N0, MagicTime) могут быть проблемы.
