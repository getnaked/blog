---
id: 662
title: 'Как приглушать звук игры/музыки в OBS когда говоришь в микрофон'
date: '2023-04-30T12:20:09+07:00'
author: getked
layout: post
guid: 'https://getked.ru/?p=662'
permalink: /kak-priglushat-zvuk-igry-muzyki-v-obs-kogda-govorish-v-mikrofon/
enclosure:
    - "https://getked.ru/wp-content/uploads/2023/04/test-zvuka-ducking.mp4\n629992\nvideo/mp4\n"
categories:
    - 'Без рубрики'
---

Эту штуку ещё называют сайдчейн (Sidechain) или дакинг (Ducking). Если не использовать, то на каждом стриме начинается:

> <cite>*У тебя музыка голос перекрывает*  </cite>

> <cite>*Игра слишком тихая, ничего не слышно*</cite>

Сейчас исправим: звуки будут громкими, а когда начнёшь говорить они станут тише.

Запускай OBS и переходи в *Фильтры* того источника, в котором звук игры/музыки. У меня это *Устройство воспроизведения*:

<figure class="wp-block-image size-large">![](https://getked.ru/wp-content/uploads/2023/04/OBS-1024x715.png)</figure>В появившемся окне нажимай слева снизу на *+* и выбирай *Компрессор*:

<figure class="wp-block-image size-large">![](https://getked.ru/wp-content/uploads/2023/04/OBS-kompressor-1024x898.png)</figure>Погнали настраивать. Можно выставить настройки как у меня, а можно по своему вкусу:

- Степень сжатия: это соотношение затухания звука. Например, значение равно 2:1 — если звук превысит порог на 10 дБ, то он будет затушен до 5 дБ.
- Порог срабатывания: громкость, при которой компрессор начнет работать.
- Атака: время, через которое компрессор начнет работать.
- Спад: время, через которое компрессор перестанет работать.
- Выходное усиление: средний уровень громкости.
- Источник приглушения/сайдчейн-компрессии: выбрать тот источник, где у вас звук микрофона.

<figure class="wp-block-image size-large">![](https://getked.ru/wp-content/uploads/2023/04/OBS-kompressor-nastrojki-1024x898.png)</figure>Пример того, как это звучит на стриме когда фоном играет Mikulski — Jane Doe:

<figure class="wp-block-video"><video controls="" src="https://getked.ru/wp-content/uploads/2023/04/test-zvuka-ducking.mp4"></video></figure>Если глянуть осциллограмму из видео, то сразу заметно работу сайдчейн-компрессии:

<figure class="wp-block-image size-large">![](https://getked.ru/wp-content/uploads/2023/04/sidechain-1024x384.png)</figure>Осталось сохранить настройки и пользоваться.