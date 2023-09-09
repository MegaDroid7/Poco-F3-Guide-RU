---
description: Я хочу поставить рекавери!
---

# (recovery\_a) no such partition



![Ошибка no such partition](<../.gitbook/assets/image (21).png>)



Такая ошибка возникает, когда вы пытаетесь прошить раздел, который не существует на телефоне. Как же так, тогда откуда идёт рекавери? Раздел с рекавери называется recovery\_ab. Если быть точнее:

1. recovery\_a - рекавери в первом слоте
2. recovery\_b - рекавери во втором слоте
3. recovery\_ab - рекавери в обоих слотах

Поэтому для установки рекавери следует писать:

<pre><code><strong>fastboot flash recovery_ab recovery.img
</strong></code></pre>

Либо же, если ваше рекавери является TWRP или OrangeFox, то установить его можно следующим способом:

Для начала запустимся в рекавери:

```
fastboot boot twrp_or_fox.img
```

Далее:

1. Выберите Advanced / Дополнительные
2. Выберите пункт: Flash current TWRP / Flash current OrangeFox
3. Согласитесь с выбором
4. Если у вас были root-права, переустановите Magisk
5. Перезагрузите устройство
