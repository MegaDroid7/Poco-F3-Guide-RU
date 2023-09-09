---
description: Выключаем ненужное, оставляем нужное.
---

# 🔋 Отключение ненужных приложений

Прошивка MIUI забита разным хламом: от индийских банков и детища Марка Цукерберга до китайских аналитических программ и сервисов, которые немного, но жрут батарейку. Скорее всего, вы захотите отключить их, чтобы они не мешали. Ниже представлены 2 способа, как сделать это.

Перед тем, как перейти к способам, ознакомьтесь со списком ненужных программ. Список взят из [этого поста](https://4pda.to/forum/index.php?showtopic=1022882\&st=0#entry106035555).

{% hint style="info" %}
Внимательно ознакомьтесь с каждым приложением и его описанием и сделайте свой выбор.
{% endhint %}

<details>

<summary>Полный список ненужных приложений с пояснениями</summary>

<pre><code><strong>com.google.android.projection.gearhead - Android Auto, для связи телефона с магнитолой в машине
</strong>com.android.bookmarkprovider - рекламные закладки от Google в браузере
com.google.android.partnersetup - связь с партнерами гугл
com.miui.audiomonitor - Karaoke работает отлично без него.
com.miui.hybrid - система по созданию сайтов для продажи и прочего
com.qti.xdivert – фантастическая вещь по переадресации сигнала с неактивной симки на активную во время разговора по активной, если учесть, что в телефоне всего 1 радио модуль, то непонятно как это РАБОТАЕТ
com.tencent.soter.soterserver - подтверждение китайских платежей в китайских соц сетях
com.qualcomm.wfd.service - Wfd Service – трансляция изображения с телефона на монитор
com.miui.yellowpage - Справочник - приложение, которое показывает какая компания Вам звонит и какой отдел и какой менеджер, есть всего один минус – работает только в Китае

com.google.android.apps.subscriptions.red - Google One
com.google.android.apps.wellbeing - Цифровое благополучие если не уверены не удаляйте.
com.google.android.apps.maps - Гугл карты
com.google.android.apps.youtube.music - YouTube Music
com.google.android.gm - стандартный почтовый клиент GMail, удаляем если пользуемся сторонним. Приложение постоянно собирает почту с gmail.
com.google.android.videos - Гугл фильмы
com.google.android.youtube - Ютуб
com.google.android.ims - Хрень от гугла
com.google.android.apps.tachyon - Google Duo
com.google.android.feedback - отзывы о маркете
com.android.emergency - Медецинская карта
com.google.android.cellbroadcastreceiver - Экстренные оповещения
com.android.chrome - Браузер хром
com.android.egg - пасхалка гугл
com.android.providers.partnerbookmarks - хрень для Google в Chrome.
com.android.stk - Сим меню

com.mi.globalbrowser - Mi Browser
com.xiaomi.mipicks - Магазин miui
com.xiaomi.glgm - ещё один магазинчик
com.micredit.in - электронный кошелек от xiaomi
com.xiaomi.joyose - Аналитика и реклама+
com.miui.android.fashiongallery - Карусель обоев+
com.mi.android.globalminusscreen - Лента виджетов
com.miui.touchassistant - Сенсорный помощник
com.miui.hybrid - Быстрые приложения / Quick Apps
com.xiaomi.glgm - Сервис-маркет игр от Xiaomi
com.xiaomi.mipicks - Маркет приложений от Xiaomi
com.miui.yellowpage - Справочник компаний для Китая
com.miui.analytics - Analytics шпион+
com.xiaomi.payment - Mi Credit электронный кошелёк для Китая
com.mipay.wallet.in - Основной компонент для Mi Credit
com.xiaomi.midrop - Mi Drop приблуда для передачи файлов
com.miui.msa.global - MSA рекламно аналитическая дрянь+
com.milink.service - трансляции изображения по WiFi на ТВ
com.miui.player - Mi музыка
com.miui.videoplayer - Mi видео
com.miui.miservice - Сервисы и обратная связь
com.miui.vsimcore - компонент приложения Mi Роуминг(виртуальные сим-карты в России не работает)
com.miui.daemon - приложение мониторит данные смартфона и отсылает их на китайский сервер
com.miui.mishare.connectivity - Mi Share

com.ebay.carrier - приблуда от eBay
com.netflix.partner.activation - Партнерское приложение от Netflix
com.my.games.vendorapp - MRGSVendorApp дрянь
com.facebook.system - Приложение Facebook
com.facebook.appmanager - Управление приложениями Facebook
com.facebook.services - Сервис Facebook, постоянно висит в памяти
</code></pre>

</details>

<details>

<summary>Стоковая MIUI</summary>

```
com.miui.analytics
com.google.android.projection.gearhead
com.android.egg
com.android.bookmarkprovider
com.android.chrome
com.android.providers.partnerbookmarks
com.facebook.system
com.facebook.appmanager
com.facebook.services
com.google.android.apps.subscriptions.red
com.google.android.partnersetup
com.xiaomi.joyose
com.xiaomi.payment
com.mipay.wallet.in
com.miui.mishare.connectivity
com.miui.videoplayer
com.miui.daemon
com.miui.msa.global
com.miui.hybrid
com.miui.audiomonitor
com.qti.xdivert
com.tencent.soter.soterserver
com.qualcomm.wfd.service
com.android.emergency
com.google.android.apps.maps
com.android.stk
com.miui.player
com.google.android.feedback
com.miui.miservice
com.miui.yellowpage
com.milink.service
```

</details>

<details>

<summary>Xiaomi.eu</summary>

<pre><code><strong>com.google.android.projection.gearhead
</strong>com.android.bookmarkprovider
com.google.android.partnersetup
com.qti.xdivert
com.tencent.soter.soterserver
com.qualcomm.wfd.service
com.google.android.ims
com.google.android.feedback
com.android.emergency
com.android.egg
com.android.providers.partnerbookmarks
com.android.stk
com.mi.globalbrowser
com.xiaomi.joyose
com.miui.android.fashiongallery
com.xiaomi.payment
com.milink.service
com.miui.player
com.miui.videoplayer
com.miui.miservice
com.miui.vsimcore
com.miui.daemon
com.miui.mishare.connectivity
</code></pre>

</details>

{% tabs %}
{% tab title="Отключение без root (adb)" %}
Воспользуемся простой программой ADB AppControl ([сайт](https://adbappcontrol.com/ru/#download)). Установите и запустите программу. На телефоне включите режим разработчика и включите "Отладка по USB" и "Установка через USB". Подключите устройство к компьютеру и следуйте инструкциям программы. После этого в поиске ищите нужное приложение и выберите пункт: "Отключить". Не забудьте применить изменение!

{% hint style="success" %}
Вы также можете скопировать список приложений в текстовый файл и использовать его как "пресет" для этой программы. Она сама найдёт и выделит все установленные на телефоне программы.
{% endhint %}

Ниже представлены видео, чтобы вам было понятно, как это делать.

{% embed url="https://youtube.com/shorts/0SyWNkNz0T4" %}
Отключаем отладку по USB
{% endembed %}

{% embed url="https://youtu.be/VqMSwJ5Eihk" %}
Настраиваем AppControl
{% endembed %}

{% embed url="https://youtu.be/GfvPaiSySX0" %}
Отключаем приложения через AppControl
{% endembed %}
{% endtab %}

{% tab title="Отключение с root (LP)" %}
Если у Вас нет доступа к компьютеру, то отключить приложения вы сможете с помощью Lucky Patcher. Скачайте APK ([Офиц.сайт](https://www.luckypatchers.com/download/), [PDALIFE](https://pdalife.to/lucky-patcher3-android-a1727.html)) и установите его на устройство, не обращая внимание на угрозу безопасности. Следуйте инструкциям на экране до финальной установки. Далее ищите приложение в поиске, нажмите на него, выберите "Инструменты" и нажмите на "Отключить приложение (заморозить)".



Ниже представлены видео, чтобы вам было понятно, как это делать.

{% embed url="https://youtu.be/zxZ22Lvc1Dg" %}
Видео установки Lucky Patcher
{% endembed %}

{% embed url="https://youtube.com/shorts/lYAKcv6nMd8" %}
Отключение приложения через Lucky Patcher.
{% endembed %}
{% endtab %}
{% endtabs %}

