---
description: Адаптация гайда от прошивок к ядру.
---

# ⏩ Универсальный гайд по установке кастомных ядер

Хотя установка ядра происходит в одно действие, но на нашем устройстве есть некоторые моменты, которые могут ввести в заблуждение неопытных пользователей. Этот гайд написан для того, чтобы прояснить их.

{% hint style="danger" %}
Все действия вы выполняете на свой страх и риск! Не забывайте, что кодовое имя вашего устройства - alioth!
{% endhint %}

{% hint style="success" %}
Ниже представлены гайды по установке ядер для различных типов прошивки. Выбирайте гайд в соответствии с вашей прошивкой.
{% endhint %}

{% tabs %}
{% tab title="AOSP" %}
Установка и обновление ядра выполняются следующим способом:

1. Скачайте нужное вам ядро
2. Перезапустите телефон в Recovery [recovery-install.md](../beginning/recovery-install.md "mention")
3. Установите ядро с помощью прошивки скачанного ZIP-файла
4. Перезапуститесь в систему
{% endtab %}

{% tab title="MIUI" %}
Особенность установки ядра на прошивки MIUI заключается в том, что нужно патчить DTBO. Многие ядра автоматически определяют тип прошивки и зашивают DTBO во время установки. Некоторые имеют два разных исполнительных файла (например в [RealKing](realking.md)), а в [NGK](no-gravity-kernel.md) DTBO поставляется отдельно от файла прошивки.

Поэтому, установка и обновление ядра выполняются следующим способом:

1. Скачайте нужное вам ядро
2. Если предложено, то скачайте DTBO
3. Перезапустите телефон в режим Recovery [recovery-install.md](../beginning/recovery-install.md "mention")
4. Установите ядро с помощью прошивки скачанного ZIP-файла
5. Если скачан файл DTBO, установите DTBO. Для этого нажмите снизу справа "Установить ISO-файл", выберите файл DTBO, выберите из предложенных разделов DTBO и выполните установку
6. Перезапуститесь в систему.
{% endtab %}
{% endtabs %}