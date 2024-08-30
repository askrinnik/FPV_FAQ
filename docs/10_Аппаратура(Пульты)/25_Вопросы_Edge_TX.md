# Вопросы и решения для пультов с прошивкой EdgeTX

## Первичная настройка аппаратуры на Edge TX 
<font color="red">**Видео от Валентины.**</font>    
[Гайд для начинающих: как настроить аппаратуру на EdgeTx [Radiomaster Boxer ELRS]. YouTube: PropWash Service](https://www.youtube.com/watch?v=wU67j2G5Ibg)

От @Konstantin_Gr  
1. Выбираешь модель: фпв дрон.  
2. Включаешь внутренний приёмник  
3. Покетрейт на 250 Гц без букв спереди  
4. ADC фильтр отключить  

## Как сделать так, чтобы при нажатии кнопок на пульте раздавалось голосовое сообщение
Разберем на примере привязки голосовой азвучки при нажатии кнопки `ARM` (SA).  
 - Нажимаем кнопку `MODEL`. Попадаем в список моделей. Допустим мы хотим это настрпоить на активной модели.  
 - Кнопкой `PAGEDOWN` листаем на экран `SPECIAL FUNCTIONS (9/11)`  
 - Выбираем пустую строку и нажимаем на ролик.  
 - Нажимаем кнопку `ARM`. На экране отобразится значок `SA↓` (со стрелкой вниз). Нажимаем на ролик.  
 - переходим роликом в следующее поле и нажимаем на ролик.   
 - прокручиваем до `Play Track` и нажимаем на ролик.   
 - переходим в следующее поле и нажимаем на ролик.   
 - прокручиваем до `armed` и нажимаем на ролик. 
 - нажимаем несколько раз кнопку ARM и наслаждаемся звуком :)

Для `DISARM` нужно выбрать `SA↑` и трек `disarm`

## Как отключить кнопки триммирования стиков (trim)
Иногда можно случайно задеть кнопки трима, тем самым сбив настройку стиков.  
Реакцию на кнопки можно отключить:  
- Нажимаем кнопку `MODEL`  
- Переходим на экран 3/11 `FLIGHT MODES`  
- Заходим в `FM0`
- Переходим в Trims. Там стоит `:0:0:0:0` 
- Выставляем `:--:--:--:--`  

## Как откалибровать стики на аппаратуре 
[Як калібрувати стіки на пульті для FPV дрона(укр). YouTube: Є-Дрон](https://www.youtube.com/watch?v=RCaF2GHLe8g)

## Пульт зависает при попытке зайти в ExpressLRS скрипты
Такое зависание происходит если в модели отклучены оба передатчика (внутренний и внешний).  
Проверь что в модели выставлен Internal CRSF (Если передатчик встроенный), External CRSF (если передатчик внешний).  
Также во вкладке Hardware выставлен Internal CRSF вместо Multi (для внутреннего передатчика)

[Як активувати тубмлери та кнопки на пульті (EdgeTX). YouTube: Жвавий Дрон](https://www.youtube.com/watch?v=LybG0QXf7pU)  
 
## Прошивка для аппаратуры EdgeTX
[Официальный сайт](https://edgetx.org/)

[GitHub репозиторий EdgeTX проекта](https://github.com/EdgeTX/edgetx)

[How to Update EdgeTX in your Radio](https://oscarliang.com/flash-edgetx/)

[User Manual for Monochrome Screen Radios with EdgeTX](https://github.com/EdgeTX/edgetx-user-manual/tree/2.7/b-and-w-radios)

[Manual for OpenTX 2.2](https://doc.open-tx.org/manual-for-opentx-2-2)

## Изменение голосовой озвучки
[Adding sounds to your EdgeTX SD Card / No sounds after upgrading to EdgeTX](https://www.youtube.com/watch?v=jZ29qmtMSyU)  
[EdgeTX-edgetx-sdcard-sounds- Sound packs for EdgeTX](https://github.com/EdgeTX/edgetx-sdcard-sounds)

Можно подготовить свои голосовые файлы:  
Заходим на сайт с нейронкой, например, [play.ht](https://play.ht/), выбираеv голос, пишешь фразу и сохраняешь, потом конвертируеv в 32 килогерца 16 бит, моно и сохраняем.  
Имя файла нужно дать такое как и у того файла, озвучку которого заменяем.

## [Українізація OpenTX - EDGE - FreedomTX 13:08](https://youtu.be/4y8Xvei-NMk?si=_DWQJWdCbDi6c_b2&t=788)
[Посилання на Google Disk](https://drive.google.com/drive/folders/1qzFfbYw4vBnAh9kmXtYUbzmgwg7lizD0)
