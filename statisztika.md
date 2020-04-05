# Magyar koronavírus halálozási statisztikák

Az itt látható statisztikák a [koronavirus.gov.hu/elhunytak](https://koronavirus.gov.hu/elhunytak) oldalon található táblázat alapján készültek.
Az ábrák egyesével megtalálhatók a `fig` könyvtárban, az ábrákat előállító kód pedig [itt](hungary_analysis.ipynb) érhető el.

Az orvosi információk feldolgozásában Lauter Beatrix segített.

Készítette: Ács Judit

## Összes elhunyt száma nemek szerint

![Death count](fig/line_death_count.png)

## Újonnan elhunytak száma

A hivatalos adatok reggelente frissülnek, az ábra az x-tengelyen lévő nap előtti reggeltől aznap reggelig elhunytak számát ábrázolja.

![New death count](fig/line_new_deaths.png)

## Korcsoportonként

![By age group](fig/bar_death_by_age_group.png)

## Korcsoportonként és nemenként

![By age group](fig/bar_death_by_age_group_and_gender.png)

# Alapbetegségek

Az alapbetegségeket igyekeztünk egységesíteni.
Az összerendelések [itt](name_mapping.tsv) érhetők el.

## Alapbetegségek számának hisztogramja

Az ábra azt mondja meg, hogy hány olyan beteg van, akinek 0, 1 stb. alapbetegsége van.
Egy beteghez 7 alapbetegség volt beírva, ez eddig a legmagasabb szám.

A "adat feltöltése folyamatban" és a "nincs adat" mezőket 0 alapbetegségnek vettük.

![Condition count histogram](fig/condition_histogram.png)

## 10 leggyakoribb alapbetegség

Az alapbetegségek különböző részletességgel szerepelnek, pl. iszkémiás szívbetegség, máshol csak szív és érrendszeri betegség.

![10 most common disease](fig/bar_most_common_diseases.png)

## Betegségek osztályzása és az előfordulások száma

A betegségeket a [Betegségek nemzetközi osztályozása](https://hu.wikipedia.org/wiki/Betegs%C3%A9gek_nemzetk%C3%B6zi_oszt%C3%A1lyoz%C3%A1sa) szerint kategorizáltuk, kivéve a magas vérnyomást, amit külön kategóriának vettünk.
A kategorizálás [itt](categories.tsv) érhető el.

![Disease category](fig/bar_icd.png)
