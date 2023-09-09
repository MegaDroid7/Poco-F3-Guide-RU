---
description: Никакая прошивка не обходится без установки легендарного TWRP.
---

# 🔃 Установка Recovery

Ни одна установка модификаций не может обойтись без установки кастомного рекавери. Самыми популярными рекавери для установки на устройство являются TWRP от SKKK и OrangeFox. Чем они отличаются?

| TWRP SKKK                  | OrangeFox                          |
| -------------------------- | ---------------------------------- |
| Старый привычный интерфейс | Новый интерфейс                    |
| Стабильность               | Кастомизация                       |
|                            | Можно включить фонарик             |
|                            | Поддерживает MIUI OTA              |
|                            | Встроенный менеджер Magisk         |
|                            | Встроенный менеджер приложений     |
|                            | Защита Recovery с помощью PIN-кода |

Несмотря на большое количество преимуществ в сторону OrangeFox, лично я советую ставить TWRP от SKKK.

Скорее всего вы слышали о TWRP от brigudav и TWRP от Nebrassy. TWRP от brigudav известен тем, что в его рекавери вшиты множество скриптов для установки а так же расширен функционал для мододелов. А про TWRP от Nebrassy ничего сказать не могу - как по мне обычный TWRP. Но если вы знаете, чем полезен именно этот TWRP - [свяжитесь со мной](https://t.me/MegaDroid7), добавлю в заметки.

<details>

<summary>Ссылки для скачивания Recovery</summary>

Обновляемый репозиторий Recovery на [SourceForge](https://sourceforge.net/projects/recovery-for-xiaomi-devices/files/alioth/) от [Camerado](https://4pda.to/forum/index.php?showuser=2777963)

OrangeFox - [OrangeFox](https://orangefox.download/ru-RU/device/alioth) (Android 12, Android 13 для Beta-релизов)

TWRP SKKK - [AKR-Dev](https://dl.akr-developers.com/?dir=skkk/TWRP) (Android 11, Android 12)

TWRP Brigudav - [4PDA](https://4pda.to/forum/index.php?showtopic=1019227\&st=16680#entry116126056) (Android 12)

TWRP Official - [TeamWin](https://twrp.me/xiaomi/xiaomi\_redmik40\_pocof3\_mi11x.html) (Android 11, Android 12)

TWRP Nebrassy - [4PDA](https://4pda.to/forum/index.php?showtopic=1019227\&st=12780#entry113558072) (Android 11)

</details>

{% hint style="warning" %}
После установки Рекавери Magisk слетает. Если вам нужны Root-права, то после установки Рекавери заново установите Magisk.
{% endhint %}

{% tabs %}
{% tab title="Установка из рекавери" %}
Для начала загрузимся в рекавери:

```
fastboot boot recovery.img
```

Далее:

1. Выберите Advanced / Дополнительные
2. Выберите пункт: Flash current TWRP
3. Согласитесь с выбором
4. Если у вас были root-права, переустановите Magisk
5. Перезагрузите устройство
{% endtab %}

{% tab title="Установка OrangeFox" %}
Пакет с OrangeFox поставляется в виде установочного архива, который нужно будет установить из-под любого рекавери.

Для начала разархивируем архив и достанем оттуда файл recovery.img. Теперь загрузимся в OrangeFox:

```
fastboot boot recovery.img
```

Мы лишь запустились в рекавери. Теперь нам нужно перекинуть архив с рекавери в память устройства и установить его. Устройство само перезагрузится в новое рекавери. Теперь вы можете пользоваться всеми возможностями OrangeFox.
{% endtab %}
{% endtabs %}
