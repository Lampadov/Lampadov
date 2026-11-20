<div align="center">
  <img src="assets/pcb-top-view.svg" alt="Вид на печатную плату сверху. Импульсы идут к микросхеме и расходятся по дорожкам" width="100%">
  <h1>Ilya Lampadov</h1>
  <p><strong>Инженер встраиваемой техники · Embedded Systems Engineer</strong></p>
</div>

## Обо мне

Разрабатываю электронные изделия и довожу их до рабочего устройства. Работаю с микросхемами разной сложности, запускаю платы, пишу драйверы и прошивки. Проверяю на стенде, как всё это работает вместе.

В своих статьях для портала Миландр разбираю такие задачи на конкретных платах. Ниже — проекты, у которых можно открыть исходники и повторить описанный опыт.

## Избранные проекты

### TinyUSB для микроконтроллеров Миландр

Подключаем К1986ВЕ92FI к ПК и видим USB-диск. Открываем с него страницу и управляем светодиодами прямо из браузера. На том же порте TinyUSB работают ещё шесть примеров, среди них виртуальный COM-порт, мышь и клавиатура. [Проект](https://github.com/Lampadov/tinyusb-milandr-examples) · [Драйвер USB](https://github.com/Lampadov/tinyusb-milandr-examples/blob/main/src/tusb_MDR32Fx.c) · [Демо MSC + WebUSB](https://github.com/Lampadov/tinyusb-milandr-examples/tree/main/examples/msc-webusb).

<p align="center">
  <img src="assets/webusb-preview.png" width="600" alt="Веб-интерфейс со светодиодами и кнопками отладочной платы">
</p>

### Другие примеры

| Задача | Что посмотреть |
| --- | --- |
| Измерительный тракт | Как поток от изолированного модулятора превращается в 24-разрядные отсчёты в ADCUI. [MDR1206FI + MDR5103FI](https://github.com/Lampadov/mdr1206fi-adcui-demo) |
| Внешняя память | Чтение, запись и проверка памяти К1636РР4У через SSP на двух платформах. [Драйвер Flash](https://github.com/Lampadov/k1636rr4u-flash-driver) |
| Обработка сигналов | Пик 333 Гц в FFT и сравнение аппаратного CORDIC с `math.h`. [CMSIS-DSP и CORDIC](https://github.com/Lampadov/milandr-embedded-dsp) |
| Запуск и отладка | Сборка через GNU Make и запуск из ОЗУ через J-Link или CMSIS-DAP. [К1986ВЕ8Т в VS Code](https://github.com/Lampadov/k1986ve8t-vscode-template) |
| ОСРВ | Задачи FreeRTOS на двух МК и системный тик RTX5 от TIMER1. [FreeRTOS и RTX5](https://github.com/Lampadov/milandr-rtos-examples) |
