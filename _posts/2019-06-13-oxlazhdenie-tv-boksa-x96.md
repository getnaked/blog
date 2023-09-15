---
id: 65
title: 'Охлаждение TV-бокса x96'
date: '2019-06-13T12:05:00+07:00'
author: getked
layout: post
guid: 'https://getked.ru/?p=65'
permalink: /oxlazhdenie-tv-boksa-x96/
categories:
    - 'Без рубрики'
---

Если вы решились купить эту приставку, то обязательно столкнётесь с перегревом. Под нагрузкой температура за 5 минут достигает 80 градусов и включается троттлинг — частота процессора с 1512 мегагерц падает до 1200, а на 81 градусе уже до 1000. Инженеры не подумали об отводе нагретого воздуха — при толщине корпуса менее двух сантиметров практически нет путей для его выхода. На дне корпуса у x96 есть бесполезная сетка из дырок, но горячий воздух идёт вверх и снова нагревает приставку. Так что первый шаг к охлаждению — кладите бокс вверх дном или на бок, чтобы USB-разъемы оказались сверху.

<figure class="wp-block-image size-large">![](https://getked.ru/wp-content/uploads/2021/02/tv-box-x96-lg.jpg)</figure>Дальше есть два варианта — либо пассивное охлаждение с помощью радиатора, либо активное через кулер. Если активное, то берётся 12-вольтовый кулер и запитывается от USB — там питание 5 вольт, из-за чего кулер будет работать в половину мощности и бесшумно. Очень хороший вариант, но мне не подошёл — подходящего по размеру кулера под рукой не оказалось, да и сетки для защиты лопастей тоже нет.

Я пошёл по первому варианту — доработка охлаждения установкой радиатора. Изначально роль радиатора выполняет термопрокладка и стальная пластина. Термопрокладка из-за своей большой толщины в 0.5 сантиметра слабо отводит жар, а у стальной пластины низкая теплопроводность — около 50 Вт/(м·K). Пришлось пластину заменить на аналогичную по размеру, но выпиленную из алюминия, где теплопроводность куда лучше — 210 Вт/(м·K).

<figure class="wp-block-image size-large">![](https://getked.ru/wp-content/uploads/2021/02/x96-aluminevaya-plastina-ohlazhdeniya-lg.jpg)</figure>Как оказалось, найти маленький радиатор проблема. В магазинах такого практически не встречается, но я нашел подходящий — Heat Sink Kit для Raspberry Pi. В комплекте три радиатора, для приставки нужен самый большой — 14×14×6 мм.

<figure class="wp-block-image size-large">![](https://getked.ru/wp-content/uploads/2021/02/radiator-dlya-x96-lg.jpg)</figure>На основании радиатора есть скотч, который пришлось удалить из-за слабого прилегания к процессору. Вообще его надо бы закрепить термоклеем, но есть риск что охлаждение получится слабым, а оторвать уже будет тяжело. Поэтому я нанёс термопасту DEEPCOOL Z3, прикрепил радиатор, сверху на него положил отрезанный слой термопрокладки толщиной в миллиметр и чтобы это всё не скользило слегка придавил крышкой с алюминиевой пластиной.

В результате при 2-х часовом просмотре Full HD-фильма максимальная температура составляет всего 65 градусов. Затраты: 185 рублей за термопасту и радиатор, алюминиевая пластина уже была в наличии.