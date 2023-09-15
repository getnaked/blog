---
id: 164
title: 'Вывести на стрим название трека'
date: '2021-01-08T07:49:00+07:00'
author: getked
layout: post
guid: 'https://getked.ru/?p=164'
permalink: /vyvesti-na-strim-nazvanie-treka/
categories:
    - 'Без рубрики'
---

Есть трансляция, есть желание отображать на экране играющую сейчас песню. Погнали.

Скачайте архив с [Stream Music Displayer](https://obsproject.com/forum/resources/stream-music-displayer.107/), разархивируйте и запустите.

В выпадающем списке Select Player выбираем плеер или нужный сервис. Например, можно отображать песню из открытой в браузере вкладки YouTube (работает в Firefox и Chrome). После выбора нажимаем Start.

<figure class="wp-block-image size-large">![](https://getked.ru/wp-content/uploads/2021/02/Stream-Music-Displayer.png)</figure>Запускайте нужную вам песню или видео, если всё сделано правильно в разархивированной папке появится файл с названием current\_song.txt

<figure class="wp-block-image size-large">![](https://getked.ru/wp-content/uploads/2021/02/Stream-Music-Displayer-File-1024x347.png)</figure>Теперь запустите OBS и в источниках добавьте Текст (GDI+). Если у вас OBS от СтримЛабса, то найдите похожий пункт.

<figure class="wp-block-image size-large">![](https://getked.ru/wp-content/uploads/2021/02/OBS-gdi-2-1024x622.png)</figure>В настройках выберите текстовый файл current\_song.txt, нужный цвет и размер шрифта.

<figure class="wp-block-image size-large">![](https://getked.ru/wp-content/uploads/2021/02/OBS-gdi-config-2-1024x622.png)</figure>Если вам не нравится формат надписи выводимого трека или хочется перевести слова, то можно в Stream Music Displayer перейти в меню Tools — Options и на вкладке Generals сделать по-своему:

<figure class="wp-block-image size-large">![](https://getked.ru/wp-content/uploads/2021/02/SMD-Options.png)</figure>Чтобы сбавить нагрузку на CPU поставьте Refresh Rate равным 5 секунд.

А ещё можете подписаться на мой канал [get\_ked](https://www.twitch.tv/get_ked): детективные/логические/тактические игрушки и иногда озвучка комиксов.