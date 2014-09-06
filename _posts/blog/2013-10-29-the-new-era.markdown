---
layout: post
emphasized: true

author: laze
title:  "Az &uacute;j rend elj&ouml;vetele..."
excerpt: "Ahogy minden v&aacute;ltozik, &uacute;gy a webfejleszt&eacute;s is v&aacute;tozik, b&aacute;r err&#337;l sokszor mintha nem igaz&aacute;n venn&eacute;nk tudom&aacute;st. Pedig az &uacute;j rend m&aacute;r eg&eacute;szen m&aacute;sr&oacute;l sz&oacute;l, nem egyszer&#369; PHP &ndash; MySQL komb&oacute;kr&oacute;l..."
thumbnail: thumbnail-2013-08-28-welcome-to-jekyll.png
header: header-2013-08-28-welcome-to-jekyll.png

date:   2013-10-29 22:26:01

categories: personal

location: Budapest
tags:
  - mysql
  - mongodb
  - web
  - fejleszt&eacute;s
comments: false
---

### A régi út ###

Szükséged van egy alkalamazásra, mert így hozta az élet. Keresel a megfelelő fórumokon egy PHP fejlesztőt, &#189; - 3 év
tapasztalattal, aki Codeigniter szintű alapokon megírja _nagyjából_ azt amire szükséged van.

### Az új út. ###
Alkalmazás fejlesztõ vagyok, ezt írom a magamról menüpont alatt is, az alkalmazások széles skálájának ismeretével. Jelenlegi munkahelyemen online munkaidõ nyilvántartással foglalkozunk. Ezen a példán keresztül szeretném bebizonyítani azt, hogy az old-school dolgok mennyire nem mûködnek már, és mennyivel hatékonyabb eszközök állnak a rendelkezésünkre. Alkalmazás fejlesztõ vagyok. Ez nem azt jelenti, hogy tudom a PHP nyelvet és mögé tudok rakni egy MySQL adatbázist. Vagyis nem csupán ezt, bár erre is képes vagyok, sajnos. A PHP-val máskor fogunk foglalkozni, most az adatbázisról szeretnék inkább beszélni: A munkaidõ nyilvántartásba egy, már elkezdett projekt kapcsán csöppentem. Voltak adottságok, amelyeket mostanra már kinõtt a projekt, és amelyeket akkor még nem is láttunk át, de ma már tudjuk, hogy nem hogy kinõtte, de sokkal jobb megoldást is tudunk biztosítani helyette. A MySQL tábla alapú munkaidõ tárolás egyszerûnek tûnik: X napon Y ember Z órakor kezd, W órakor végez. Meg is van a rekord! Azonban jönnek a buktatók: Mi van, ha egyik nap kezd, másik nap végez? Akkor az elsõ sorban a vége nulla marad, a következõben meg a kezdet? És akkor hogyan lehet ellenõrizni, hogy ez nem hibás adatbevitel eredménye-e? Hogyan tudunk megkülönböztetni különbözõ jellegû bejegyzéseket? És hogyan kezeljem, hogy ezek átfedésben vannak-e?
Ez még csak a tárolás... Hogyan tudom utána gyorsan, egyszerûen megmondani, hogy ki, milyen állapotban van éppen? Hogyan tudok egyszerûen összesítéseket lekérdezni?