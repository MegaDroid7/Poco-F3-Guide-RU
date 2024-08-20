---
description: Священный грааль.
icon: lungs
---

# OxygenOS 14.1 (OP 11R)

Много кто пытался портануть OOS на Poco F3. Лучше всего, как по мне, удалось Dell.

В этом порте есть всё, что нужно: фикс Integrity, работающий Mir Pay, предустановленный GCam и плавность от прошивки.

Первые 10 минут возможны тормоза при работе прошивки и нагрев устройства. Далее устройство работает идеально, без ощутимого нагрева.

Батарею да, кушает чуть больше, чем на стоке. Это беда всех портов OxygenOS. Но 6 часов экрана на BN59 я получил, что считаю неплохим результатом.

Последние 2-3 дня я пользуюсь этим портом и я им доволен. Добавить бы MIUI камеру и будет идеально, но увы.

Из минусов: не выключается doubletap2wake (dt2w), функции защиты OxygenOS не работают и не работает разблокировка по лицу. В остальном все функции работают идеально.

## Установка

1. Скачать порт - [ссылка](https://drive.google.com/file/d/11YISqM12\_OqSDYNm2N8YAU28ZMhu2JPX/view)
2. Скачать Firmware - [ссылка](https://github.com/XiaomiFirmwareUpdaterReleases/firmware\_xiaomi\_alioth/releases/download/stable-26.04.2024/fw\_alioth\_miui\_ALIOTHGlobal\_OS1.0.2.0.TKHMIXM\_b69e6a5400\_13.0.zip)
3. Загрузитесь в рекавери. [recovery-install.md](../beginning/recovery-install.md "mention")
4. Сделайте вайпы Dalvik ART Cache, Cache, Metadata, Data. Не трогаем Internal Storage
5. Прошейте Firmware
6. Прошейте порт
7. Сделайте Format Data (через yes)
8. Перезагрузите устройство.
