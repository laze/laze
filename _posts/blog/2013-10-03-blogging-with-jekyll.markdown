---
layout: post
emphasized: true

author: laze
title: "Szevasz vil&aacute;g, itt a blogom!"
excerpt: "Mit is jelent pontosan, hogy Jekyllt haszn&aacute;lok Wordpress helyett, &eacute;s hogyan illeszkedik mindez a napi rutinba? Le&iacute;rtam a folyamatot, tess&eacute;k!"
thumbnail: header-2.png
header: header-2.png

date: 2013-10-03 0:37:13

categories: personal

location: Budapest
tags:
 - (mt)
 - jekyll
 - why not wordpress
 - workflow
 - don't stress
comments: true

---
Igen sok különböző filozófia alapján építkező webalkalmazást találhatunk, ha tartalom megosztásra, csúnyábban _blogolásra_
keresünk megoldást. Wordpress, Textpattern, Movable Type, és még sokan mások, de aztán ott vannak a SaaS megoldások is,
egyebek mellett a blogger.com, a blog.hu, és még ki tudja mi minden más.

Hogy ezek mellett miért a Jekyll-t választottam? Elmondom.

Alapvetően azt mondanám, hogy két teendőnk van:

1. Előállítani a tartalmat,
2. És előadni, tálalni a tartalmat.

### A tartalom előállítása ###
A tartalom előállításához nyugalom szükséges. A lehetősége annak, hogy átlássam amit írok, hogy alakíthassam a szerkezetét
amikor már eljutottam egy szintre a gondolataim összegyűjtésében. Mivel bizonyos tartalmak előállítása akár hosszadalmas
is lehet, nem megy első blikkre, de nem is az a feladata, nos, ezeket a tartalmakat valahol meg kell őrizni, hogy bármikor
hozzá lehessen nyúlni. Ezen a ponton úgy gondolom, egy _notepad_ talán még hasznosabb is, mint bármilyen web alapú alkalmazás.

Persze a notepad marhára nem _cool_, én sem használom.

[Dragon Zoltán][dragon] ajánlotta a blogján egyszer az [OmmWriter][ommwriter] szövegszerkesztőt, ami már sokkal _coolabb_,
én néha használom is de az inkább hosszabb, komolyabb tanulmányokhoz való, tapasztalataim alapján. Feljegyzésekhez, napi
szintű munkavégzés mellett a használatát nehézkesnek éreztem, ehhez én valami sokkal egyszerűbb eszközt gondolnék. Mondjuk
olyat, amit amúgyis használok, például a kódszerkesztőt.

Én a Word-öt elejétől fogva úgy használom nagyjából ahogy kell: írom a dokumentumot, jelölöm a címeket, bekezdéseket,
idézeteket, aztán a végén egyetlen lépésben formázok. És ez egy sarkalatos pont: Azt szeretném, hogy amit írok szöveget,
abban megjelelölhessek dolgokat, tudjam, hogy minek kell félkövérnek vagy dőltnek lenni, mi lesz cím, mi bekezdés, és így
tovább. Nem ezeket akarom látni konkrétan, nem a _félkövérségét akarom látni a betűnek_, hanem tudni akarom, hogy ez majd
félkövér lesz. Ez gyakorlatilag a _markup_ nyelvek sajátossága: Textile, Markdown, Liquid, és a többi...
Ha a szöveget csak begépelem, ezek a megoldások sokkal jobban használhatók, mint a WYSIWYG szövegszerkesztők vagy a HTML
maga, ugyanis a jelölőnyelvek sokkal kényelmesebben olvashatók az emberi szem számára, mint a HTML, vagy más leírónyelvek.

A Jekyllnek megvan az az óriási előnye, hogy valamennyi poszt egy-egy statikus állomány. Tehát nincs adatbázis. A `jekyll
build` parancsa rakja össze a sablonokból és a tartalmakból az oldalt, amit akár a `jekyll serve` parnccsal is kiszolgálhatunk,
de innentől kezdve bármilyen statikus kiszolgáló is jó.

> Ha a GitHub-on hosztoljuk az oldalunkat, akkor a [GitHub Pages][github] képes a Jekyll által generált tartalmak kiszolgálására.

Mivel oldalaimat már régóta a [(mt) mediatemple][mediatemple] szolgáltatja, én egész egyszerűen a `jekyll build` parancs
eredményét töltöm fel FTP-n a szerverre.

Ezért nagyon találó a _blogolj, mint egy hacker_ jelmondat a Jekyll stábjától. A mindennapi munkám során használt programkód
szerkesztők teljesen jól alkalmasak a posztok szerkesztésére, rendezésére, egyebekre. Nem kell hozzá újabb programot
telepíteni, futtatni, semmi ilyesmi, használom, megnyitom, szerkesztem, bezárom, és nem okoz fennakadást.

### A tartalom tálalása ###
A másik pedig, és ezzel már ügyesen át is kötöttünk, a sablonok szerkesztése. Kevés, szerver oldali `if`-fel összerakhattam
a doboozokat, amik aztán összeálltak. Annak idején a Wordpress-szel is ez volt a bajom, többek között: Bonyolult struktúrában
kell bonyolult sablonokat létrehozni, és widgeteketen keresztül szerkesztgetni bizonyos tartalmi elemeket. Ebből a szempontból
anno a textpattern ezerszer jobb volt, mint a Wordpress. A Wordpress másik utálatos tulajdonsága tulajdonképpen egy borzalmas
örökség, és ez maga a PHP. A PHP egy mára már több sebből vérző, de egyszerűsége és igénytelen kialakítása miatt az egyszerűbb
fejlesztők körében ma is igen népszerű programnyelv, ugye, ahol az objektum orientált működés az utóbbi idők beleerőszakolása
csupán.

És a Jekyll iskola mit mond?

Egy alap HTML nyelvű sablon, bármilyen más sablon nyelvi elemekkel, mint például Twig, vagy Erubis. Ennyi. Ebben mindig a
`content` elemet fogja a Jekyll a következő lépcső visszatérési eredményével feltölteni. Az állományok tetején pedig
egy YAML nyelvű fejlécet szúrhatunk be. Ezzel az eszköztárral már minden megoldható, ami a hétköznapi blogolást intézi, és
nem kell azon töprengeni, hogy nem objektum oritentált régi blogmotorra hogyan húzzak egy webáruházat rá.

### Összességében? ###
Azt mondhatom, hogy úgy érzem, jó döntést hoztam. Csatlakozik ahhoz a döntési sorozathoz, melynek első lépése a Nokia N9
megvásárlása volt: hogy csökkentsük a mindennapi stresszeket, ahol csak lehet, 0-ra. Nem úgy, mint a rezisharcban, 10%-al,
hanem az élet minden területén, ahol be tudtuk azonosítani, hogy mi a baj, ott próbáljuk is redukálni egészen nullára a stresszt,
azt a feszültséget, mely az élet adott területén fennáll.

Tehát ez az új blogom. Remélem értékeled, szeretni fogod.

[dragon]:         http://www.dragonweb.hu/
[ommwriter]:      http://www.ommwriter.com/
[github]:         http://pages.github.com/
[mediatemple]:    http://www.mediatemple.com/