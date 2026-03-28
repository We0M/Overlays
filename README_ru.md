# Overlays by WeoM

<div align="center">

**[English](README.md) | Русский**

[YouTube - ПОКАЗЫВАЮ КАК КРАСИВО СЛЕДИТЬ ЗА FPS И ТЕМПЕРАТУРАМИ В ИГРАХ - MSI Afterburner и RTSS](https://www.youtube.com/watch?v=GwYgzIkAgWc)
</div>

Набор оверлеев для RivaTuner Statistics Server (RTSS). Создавались на разрешении экрана 1920x1080.
Поддерживаемые платформы: для Full версий только AMD(cpu), остальные тестировались на cpu AMD и GPU NVIDIA, но должны работать на других платформах.

## Вариации оверлеев

- **AMD Full v3.0 graph** — полный оверлей с двумя вариантами графиков отображения загрузки ядер процессора
- **Regular** — вдохновлён сторонним оверлеем, автор неизвестен
- **Mini / Micro / Nano / Pico** — компактные варианты разного размера
- **Horizontal** — горизонтальный оверлей по мотивам NVIDIA
- **I2HARD AMD** — оверлей по мотивам I2HARD

## Содержание

- [Требования](#Требования)
- [Использованные шрифты](#Требования)
- [Установка](#Установка)
- [Важная информация](#Важная-информация)
- [Скриншоты](#Скриншоты)

## Требования

- [RTSS](https://www.guru3d.com/download/rtss-rivatuner-statistics-server-download/)
- [MSI Afterburner](https://www.msi.com/Landing/afterburner/graphics-cards)
- [HWiNFO](https://www.hwinfo.com/) (рекомендуется для правильного отображения Full версий)

## Использованные шрифты:
- Impact Bold 7
- Roboto Bold 7 [Скачать](https://fonts.google.com/specimen/Roboto)
- Unispace Bold 7 (шрифт по умолчанию RTSS)
- Bahnschrift Bold Condensed 7

## Установка

1. Скачайте и разархивируйте архив `overlays.zip` | **[Скачать последнюю версию](https://github.com/We0M/Overlays/releases/download/v1.0/Overlays.7z)**
2. Откройте **RTSS** и перейдите в:
   1. `Setup` → `Plugins`
   2. Убедитесь, что галочка рядом с `OverlayEditor.dll` включена.
   3. Дважды кликните по `OverlayEditor.dll`, чтобы открыть редактор.
   4. В OverlayEditor откройте вкладку **Оверлеи** → **Импорт**.
   5. Выберите нужный оверлей из папки, куда вы распаковали архив.
3. При необходимости измените источники данных под вашу систему

## Важная информация

> [!IMPORTANT]
> **Настройки пользователя в оверлеях по умолчанию заблокированы.**
>
> Во всех оверлеях игнорируются пользовательские настройки, чтобы у всех
> отображение было одинаковым. Поэтому изменение шрифта/масштаба не работает.
>
> Чтобы это разблокировать:
> 1. Откройте свойства оверлея.
> 2. Снимите галочку `Запретить настройки пользователя`.
> 3. Примените шрифт, стиль и размер, указанные в поле `Имя`.

> [!IMPORTANT]
> В оверлеях «AMD Full v3.0 graph …» некоторые датчики продублированы из LibreHardwareMonitor (LHM).
> Перед тем как полагаться на их показания, сравните их с датчиками из HWiNFO:
>
> 1. В LHM могут быть недоступны некоторые датчики.
> 2. Часть датчиков может показывать некорректные значения.
> 3. Названия датчиков могут не соответствовать реальному смыслу.
>
> Например, у меня в LHM напряжение SoC Voltage было подписано как `Vcore`,
> а датчик `Core (S12 TFN)` не отображал напряжение ядра вообще.

> [!CAUTION]
> **CPU clock из RTSS может вызывать статтеры.**
>
> На системе с Ryzen 5 5600G источник `CPU clock` из RTSS вызывал микрофризы
> (это было видно по графику Frametime и подтверждено через макросы `%PollingTime0%`, `%PollingTime1%`).
>
> Рекомендуется не использовать `CPU clock` из RTSS и оставлять источник частоты CPU,
> который предоставляет MSI Afterburner / HWiNFO.

## Скриншоты
<div align="center">

### Impact default 7
![AMD Full v3.0 graph v1 Impact](preview/AMD%20Full%20v3.0%20graph%20v1%20impact.png)
![AMD Full v3.0 graph v2 Impact](preview/AMD%20Full%20v3.0%20graph%20v2%20impact.png)

| ![Regular v1.0 impact](preview/Regular%20v1.0%20impact.png) | ![Mini v1.0 impact](preview/Mini%20v1.0%20impact.png) | ![Micro v1.0 impact](preview/Micro%20v1.0%20impact.png) | ![Nano v1.0 impact](preview/Nano%20v1.0%20impact.png) | ![Pico v1.0 impact](preview/Pico%20v1.0%20impact.png) |
| :---------------------------------------------------------: | :---------------------------------------------------: | :-----------------------------------------------------: | :---------------------------------------------------: | :---------------------------------------------------: |
|                        Regular v1.0                         |                       Mini v1.0                       |                       Micro v1.0                        |                       Nano v1.0                       |                       Pico v1.0                       |

### Font: Roboto Bold 7


![AMD Full v3.0 graph v1 Roboto](preview/AMD%20Full%20v3.0%20graph%20v1%20Roboto.png)
![AMD Full v3.0 graph v2 Roboto](preview/AMD%20Full%20v3.0%20graph%20v2%20Roboto.png)

| ![Horizontal v1.0 static FT](preview/Horizontal%20v1.0%20Roboto%20static%20FT.png) |
| :---------------------------------------------------------: |
|                        Horizontal v1.0 static FT                         |

### Font: Unispace Bold 7 (this is default font RTSS)
![AMD Full v3.0 graph v2 Unispace](preview/AMD%20Full%20v3.0%20graph%20v2%20Unispace.png)

### I2HARD | Font: Bahnschrift Bold Condensed 7
> Спасибо каналу I2HARD за идею этого оверлея, я только его повторил.

![I2HARD AMD v2.0](preview/I2HARD%20AMD%20v2.0.png)

</div>
