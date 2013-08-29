---
layout: post
title:  "Welcome to Jekyll!"
date:   2013-08-28 00:06:01
categories: jekyll blog wordpress
---

Az utóbbi időben ismét csendesen működő blogom története újabb fordulóponthoz érkezett: Wordpressről Jekyllre cseréltem
a motort, és bár a (mt) hosztolja az oldalaimat továbbra is, ezt az egyszerűség kedvéért github oldalak alá tettem fel.

A Jekyllről a [hivatalos oldalon][jekyll] találsz bővebb információt. Dióhéjban: A Jekyll egy igen egyszerű valami:
Megfelelő struktúrába rendezett és megfelelő szerkezetű oldalakból épít fel egy működés közben statikus oldalt. Nincs
tehát webes, vagy bármilyen szerkesztői rendszer, nincsenek idétlen frissítések, _on the fly_ szerkesztett sablonok,
nincsenek bugyuta _query_-k, csak pusztán a sablon, és tartalmak.

> Sok esetben nálam pont a Wordpress volt a visszatartó tényező mindenféle dolgok publikálásában: A 3-as PHP-t idéző
> szerkezete, a procedurális kialakítása, a könnyűnek mondott, de tisztán nem használható szerkezete, mind-mind oda vezetett,
> hogy nem éreztem jól magam azon a platformon.

Na de nézzük, mi is ez a Jekyll és hogyan működik?

A Jekyll alapjai
----------------
A Jekyll Ruby nyelven iródott, de ez első körben csak azért érdekes, mert kell, hogy legyen hozzá Ruby és Gems a gépeden.

- A telepítéshez egészen egyszerűen telepítsük a szükséges gemet:
{% highlight ruby %}
~ $ gem install jekyll
{% endhighlight %}
Innentől kezdve gyakorlatilag a Jekyll a rendelkezésünkre áll.

- Hozzunk létre egy új oldalt, és már kezdhetjük is a munkát:
{% highlight ruby %}
~ $ jekyll new az-en-csodalatos-oldalam
~ $ cd az-en-csodalatos-oldalam
~/az-en-csodalatos-oldalam $ jekyll serve
{% endhighlight %}
Ezek után a [http://localhost:4000][jekyll-local] linken nézegethetjük az új csodálatos oldalunkat.

A `jekyll serve` parancs csak a teszteléshez használandó éles környezetben az exportált tartalom adja az oldal megjelenítését.
(Ez alapértelmezés szerint a `_site` mappában kap helyet.)
Posztjaink alapértelmezés szerint a `_posts` mappában, `EEEE-HH-NNa-poszt-cime.formatum` elnevezési konvencióval szerepelnek.
Ezek statikus állományok, az állomány elején némi konfigurációs lehetőséggel, egyébként magával a [markdown][markdown]
&mdash; vagy más &mdash; szintaxisú szöveggel. Régebben huzamosabb ideig blogoltam Texpattern-nel is, mely a Textile formátumot
használja szövegek gyors, egyszerű WYSIWYG szövegszerkesztők használata nélküli szerkesztéshez, amit nagy örömömre a Jekyll
szintén ismer.

[jekyll]:       http://jekyllrb.com
[jekyll-local]: http://localhost:4000
[markdown]:     http://daringfireball.net/projects/markdown/basics
