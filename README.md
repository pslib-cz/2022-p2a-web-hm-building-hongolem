# 2022-p2a-web-hm-building-hongolem
 [Github Pages](https://pslib-cz.github.io/2022-p2a-web-hm-building-hongolem/)

## To Do

* [x] Uklidit classy
* [x] Roztřídit classy
* [x] Uklidit CSS
* [x] Desktop
* [x] Mobile
* [x] Validator
* [x] Dohlazení
* [ ] Lighthouse

## Opravy pana Kazdy
* [x] bude dodrženo "kodérovo desatero"
* [x] ``<h1>`` chápu "největší nadpis“ pro jeho formátování, ne sémantiku
* [x] Vlastnost font-size a font-family nastavujeme selektoru html {}, ne body {}
* [x] Font-size nastavujte v jednotkách em/rem a ne v px pro ovlivnění z rodiče/dokumentu
* [x] V kontakt.html jsou kontaktní údaje (tel., mobil, adresa) klikatelné odkazy.
* [x] Každý samostatný ``<a>`` button/cta má být buď display block nebo inline-block
* [x] Nenastavovat width 100%, ale ani fixní výšku (existují výjimky)
* [x] Vytváření redundantních stylů pro totéž – text__novostavby / text__domy apod. má stejné vlastnosti
* [x] Neumí pracovat s formuláři.

### Kodérovo desatero (třicetitero)
* [x] ``<html>`` lang odpovídá skutečnému jazyku (cs, en, zxx)
* [x] ``<title>`` je nastaveno srozumitelně, používá „drobenkovou“ navigaci „page | site“
* [x] výchozí font-family a font-size patří do ``<html>``, ne ``<body>``
* [x] ``<h1>`` je unikátní a odpovídá obsahu stránky
* [x] tagy h1, h2… označují skutečné klíčové slovo (Prostřednictvím kterého bude někdo „googlit“ obsah stránky!)
* [x] každý ``<img>`` důsledně dodržuje alt s reálným popisem obsahu obrázku

* [x] zcela responzivní obrázky (mohou přejímat poměr stran z rodiče):
``width: 100%
height: 100%;
display: block;
margin, padding: 0;
object-fit: cover;``

* [x] tag ``<img />`` může mít atributy width, height nastavené na „maximální“ rozměr obrázku v layoutu – má to pozitivní vliv na Web Vitals Cumulative Layout Shift
* [x] CSS Grid používám zejména pro layout stránky (pomocí areas) a ortogonální skupiny (galerie)
* [x] neflexuji veškerý obsah, pokud to není nutné, tedy neporušuji (nenahrazuji) content flow (To znamená, že flex používám zejména pro horizontální rozmístění prvků!)
* [x] neduplikuji CSS napříč media queries – pouze pozměňuji patřičné vlastnosti
* [x] CSS dokumenty rozděluji podle užití, např. typography.css, layout.css, componets.css – nepojmenovávám (a nerozděluji) je dle sekce webu, kterou ovliňují – ne kontakt.css, zanrove.css
* [x] hlídám si, jaké CSS vlastnosti má tag definované defaultně – tj. například margin u ``<figure>`` nebo ``<p>``
* [x] navigaci na stránce vkládám do konstrukce: ``<nav>`` ``<menu>`` ``<li><a href=“#“>odkaz</a>`` ``</menu>`` ``</nav>``

#### Konvence zjednodušující návrh
* [x] vždy kóduji mobile-first (redukuji tak množství stylů, aplikovaných při načítání stránky pro malý display; zároveň mám jistotu, že na mobilu nebude něco „scházet“)
* [x] font-size, line-height, margin, padding, text-indent… používá em / rem jednotky (násobky velikosti písma)
* [x] pokud používám max-width, tak v px, em, výjimečně vw; ne v procentech [%]
* [x] všechny odkazy (tlačítka, menu, cta prvky) tvořené ``<a>`` tagem mají nastaven display: inline-block; případně display: block; – nikdy nezůstávají display: inline;
* [x] tag ``<a>`` má atribut href povinně vyplněný (stačí jen href="#" nebo href="javascript:void(0)")
* [x] nenastavuji elementům width: 100%; (to není téměř nikdy potřeba)
* [x] výšku (height, max-height) nastavuji prvkům jenom tam, kde nemůže dojít k nechtěnému „vytékání“ obsahu;
* [x] selektor :hover používám výhradně pro tag ``<a>``, případně prvky s kódem na události onclick
* [x] nepoužívám overflow: hidden; jako nápravu vlastních chyb (řeším příčiny, ne následek)
* [x] používám některou z metodik (např. BEM), pro redukci duplicitních stylových definic a zvýšení orientace / přehlednosti ve struktuře kódu
* [x] do tagu ``<img />`` patří jen informační grafika (fotky, klikatelné logo v navigaci); piktogramy a další designové prvky vkládám prostřednictvím css
* [x] obecně nevkládám „prázdné“ html elementy – vždy musí mít nějaký obsah (``<tag>obsah</tag>``)
* [x] nepoužívám tagy ``<br>`` a ``<hr>``
