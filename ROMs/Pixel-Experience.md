---
description: Не менее популярная прошивка с не менее популярными плюсами.
---

# 🥒 Pixel Experience

Ностальгия пробирает тело, когда я вспоминаю 2016 год, ставил root права на Nexus 7 и устанавливал CyanogenMod на Android 4.4.4, тогда ещё даже не существовало Android 6. Потом Cyanogen стал Lineage, а сейчас все поголовно ставят Pixel Experience.

Ещё мне нравится xdroid - форк Pixel Experience с направлением на минимализм. Очень плавная и стабильная прошивка. Но об этом в следующий раз. Сейчас у нас гайд по установке Pixel Experience.

{% hint style="warning" %}
Перед установкой Pixel Experience убедитесь, что на прошлой прошивке работали все функции. При возникновении проблем установите Firmware вашей прошлой прошивки.
{% endhint %}

{% hint style="danger" %}
Не продолжайте установку если что-то пошло не так!
{% endhint %}

### Установка

1. Перейдите по [ссылке](https://download.pixelexperience.org/alioth)
2. Скачайте последнюю сборку и рекавери
3. Скачайте ADB, драйвера
4. Запустите телефон в Fastboot
5. Скачайте [этот](https://gitlab.pixelexperience.org/android/vendor-blobs/wiki\_blobs\_alioth/-/raw/thirteen/android-13/vendor\_boot.img) vendor\_boot
6.  Установите этот vendor\_boot командой:

    ```
    fastboot flash vendor_boot <vendor_boot>.img
    ```
7.  Установите рекавери командой:

    ```
    fastboot flash boot_ab <recovery_filename>.img
    ```
8.  Перезагрузитесь в рекавери:

    ```
    fastboot reboot recovery
    ```
9. В рекавери: Factory reset -> Format data/factory reset -> Format data
10. Вернитесь в меню рекавери. Выберите Apply update -> Apply from ADB
11. Пишем в консоли:

    ```
    adb sideload <filename>.zip
    ```
12. Перезапускаемся.
