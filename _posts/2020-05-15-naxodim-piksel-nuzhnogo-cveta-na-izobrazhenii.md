---
id: 76
title: 'Находим пиксель нужного цвета на изображении'
date: '2020-05-15T12:09:00+07:00'
author: getked
layout: post
guid: 'https://getked.ru/?p=76'
permalink: /naxodim-piksel-nuzhnogo-cveta-na-izobrazhenii/
categories:
    - 'Без рубрики'
---

Нужен был скрипт, который загрузит изображение и будет искать на нём заданный цвет. Если такой цвет есть, то вывести сообщение. Не особо красиво, зато работает. Исходник на Python, переменным r\_query, g\_query и b\_query нужно присвоить цвет в формате RGB, переменной url — адрес изображения.

```
<pre class="wp-block-code">```
#! /usr/bin/env python
# -*- coding: utf-8 -*-
 
from PIL import Image
import urllib2
 
r_query = 177
g_query = 255
b_query = 70
url = 'https://getked.ru/files/line.png'
result = 'Цвет не найден'
 
img = Image.open(urllib2.urlopen(url))
rgb = img.convert('RGB')
for x in range(img.size[0]):
	for y in range(img.size[1]):
		r, g, b, = rgb.getpixel((x, y))
		if r == r_query and g == g_query and b == b_query:
			result = "Цвет найден"
#если пиксель нужного цвета найден, то прерываем поиск
 
print result
```
```