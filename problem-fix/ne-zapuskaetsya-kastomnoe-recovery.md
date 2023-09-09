---
description: Вы точно всё прошили?
---

# Не запускается кастомное Recovery

Во время установки прошивки или её использования вам захочется зайти в Recovery, но может произойти такая ситуация, что никакое Recovery не будет нормально запускаться. И, как обычно, проблема решается очень просто - установкой vendor\_boot от Pixel Experience.

{% hint style="info" %}
vendor\_boot нужен для правильной работы Recovery.
{% endhint %}

vendor\_boot от Pixel Experience вы можете скачать [отсюда](https://gitlab.pixelexperience.org/android/vendor-blobs/wiki\_blobs\_alioth/-/raw/thirteen/android-13/vendor\_boot.img).

Установка:

{% code fullWidth="false" %}
```
fastboot flash vendor_boot vendor_boot.img
```
{% endcode %}
