# PS4 Сервер 9.00u (Русская версия by tChibo)


Это небольшая модификация <a href=https://github.com/stooged/PS4-Server-900>PS4 Сервера 9.00</a>.

Единственные файлы, которые теперь требуются в хранилище spiffs esp8266, — это .bin пейлоады, все остальное обрабатывается внутри, включая генерацию списка пейлоадов.

Вы сами все еще можете изменить html файлы, загрузив свой собственный index.html, если в хранилище spiffs нет index.html, будут использоваться внутренние страницы.

Если у вас возникли проблемы с компиляцией скетча, убедитесь, что <a href=https://github.com/esp8266/Arduino>ESP8266 библиотека</a> обновлена.

Добавлена возможность выключать и включать USB-устройство с помощью контакта D7 на плате, чтобы вызвать реле для управления питанием USB-устройства(флэшки).

Идея состоит в том, чтобы отключить питание 5 В на USB-флэшкке и включить и выключить его с помощью реле, которое управляется устройством esp8266, и включать и выключать его во время начальной загрузки эксплойта, что устраняет необходимость подключать и отключать USB флешку.


<a href="https://youtu.be/WrJMKA0y-Lg" target="_blank">Видео</a>


Вы можете сделать это с помощью USB-кабеля «мама-папа», это базовая схема того, как его настроить.

<b>TRR1A05D00 5 Вольт SPST DIL Герконовое реле

<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/diag.jpg><br>

BESTAR BR-500 Герконовое реле (5V, 500Ω)</b>

<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/diag1.jpg><br>

<br>

другой способ настроить его - использовать npn-транзистор и отрезать землю от USB-устройства, которое было показано <b><a href=https://www.psxhax.com/threads/ps4-server-9-00-ps4-server-9-00u-for-esp8266-d1-mini-pro-by-stooged.10685/post-189470>blumenal</a></b> на psxhax.

используемые детали: 

<b>1k резистор<br>
1.1k резистор<br>
BC 548 NPN транзистор</b>

Это базовая схема того, как это настроить.

<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/diag2.jpg><br>


<br><br>

# Кабельные моды

это тестовый кабель, который я сделал, и людям будет проще всего его сделать.

используемые детали:<b>

D1 Mini Pro v1 ESP8266 плата.

BESTAR BR-500 Герконовое реле (5V, 500Ω)

<a href=https://www.jaycar.com.au/0-5m-usb-2-0-a-male-to-usb-a-female/p/WC7708>0.5m USB 2.0 A «папа» на USB «мама»</a>
</b>

<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/10.jpg><br>

<br><br>

Я закончил тем, что напечатал на 3D-принтере небольшую коробку для реле и ESP8266 для кабельного мода, я залил сторону реле / проводов горячим клеем и склеил коробку вместе.

Файлы для печати коробки для 3d-принтера вы моможе скачать  - <a href=https://github.com/stooged/PS4-Server-900u/tree/main/STL>здесь</a>

<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/11.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/13.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/12.jpg><br>

<br><br>


# Альтернативный метод 


Этот кабель сделал для проверки метода от blumenal, и он отлично работает, поэтому, если вы можете найти эти детали, это альтернатива реле, код не требует изменений для работы любого метода.


<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/14.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/15.jpg><br>



<br><br>


# Usb Chip В Коробке

Я сделал этот кабель для друга, и я решил впаять USB-чип в схему, и я сделал коробку для одного USB-кабеля.

<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/23.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/24.jpg><br>

итоговый результат:

<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/25.jpg><br>



<br><br>


# PS4 PHAT

используемые детали:
<br>
<b>
D1 Mini Pro v1 ESP8266 плата.

<a href=http://www.dobe-game.com/en/productshow-55-151.html>PS4 USB HUB TP4-810</a>

TRR1A05D00 5 Вольт SPST DIL Герконовое реле.

SanDisk Ultra Fit 8gb usb флешка
</b>

some pictures of the mod:
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/1.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/2.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/3.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/4.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/5.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/6.jpg><br>

конечный результат:
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/8.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/7.jpg><br>

<br><br>

# PS4 SLIM

В слимке usb-хаб намного меньше места, но вы можете просто вставить плату.

используемые детали:

<b>
<a href=http://www.dobe-game.com/en/productshow-54-167.html>PS4 Slim USB HUB TP4-821</a>

TRR1A05D00 5 Volt SPST DIL Герконовое реле.

D1 Mini ESP8266 плата.</b>

<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/16.jpg><br>

итоговый результат:

<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/17.jpg><br>


<br><br>


# PS4 PRO

хаб для прошки.

используемые детали:

<a href=http://www.dobe-game.com/en/productshow-53-177.html>PS4 Pro USB HUB TP4-832</a>

TRR1A05D00 5 Volt SPST DIL Герконовое реле.

D1 Mini Pro v1 ESP8266 плата.

SanDisk Ultra Fit 8gb usb флешка

этот вариант доработки немного другой, я удалил один из USB-портов, вытащил чип из USB-накопителя и припаял его прямо к хабу, а затем заблокировал отверстие для удаленного порта.

<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/18.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/19.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/20.jpg><br>
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/21.jpg><br>

итоговый результат:
<img src=https://github.com/stooged/PS4-Server-900u/blob/main/Images/22.jpg><br>

<br>
