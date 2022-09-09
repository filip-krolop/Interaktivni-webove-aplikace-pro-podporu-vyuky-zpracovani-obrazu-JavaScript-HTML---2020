# Interaktivní webové aplikace pro podporu výuky zpracování obrazu (JavaScript, HTML, CSS) - 2020
Bakalářská práce

---

## Stručný popis:

V rámci bakalářské práce jsem tvořil jednodušší webové applety v HTML, CSS a JavaScriptu na téma **Interaktivní webové aplikace pro podporu výuky zpracování obrazu**. Jedná se o drobnější programy, jejichž cílem bylo podpořit teorii probíranou ve výuce předmětu **Základy počítačové sazby a grafiky** a studentům znázornit základní principy pro lepší pochopení probírané problematiky paletové reprezentace obrazu, míchání barev v odlišných modelech, převodu barevného obrazu na šedotónový či umělého obarvení obrazu.

Jedná se o 4 jednodušší programy, jejichž účelem bylo podpořit teorii probíranou ve výuce a znázornit základní principy při konverzi mezi jednotlivými barevnými modely a prostory nebo při přebarvení obrazu. Všechny zmíněné applety fungují v čistém JavaScriptu a bez využití externích frameworků a knihoven třetích stran, jejich nasazení vzhledem k povaze programů a zadání práce nebylo uvažováno. Mohu doplnit, že applet pro převedení barevného obrazu do stupňů šedi pracuje s použitými obrázky na úrovni jednotlivých pixelů, kdy na každou barevnou složku R/G/B daného pixelu je aplikován určitý přepočet a nová hodnota je poté vykreslena do elementu Canvas na stránce. Na podobném principu práce na úrovni pixelů byl dotvořen i applet na demonstraci umělého obarvení obrazu. Zbylé dva programy jsou po technické stránce velmi jednoduché a využívají pouze základních elementů HTML jazyka, doplněnými o interakci za využití JavaScriptu.

Applety byly odladěny pro použití v prohlížeči Google Chrome.

---

## Ukázka:

**http://testsempr.8u.cz/applety_ukazka/**

---

## Popis jednotlivých appletů:

 - **MichaniBarev** - Applet demonstruje vztahy a vzájemné přepočty mezi barevnými kanály a základními barvnonosnými složkami vybraných barevných modelů. Pomocí posuvníků je možno nastavit hodnoty pro konkrétní barevný model, současně se provede přepočet hodnot pro ostatní barevné modely a výsledná nastavená barva se promítne do náhledové plochy (vnější čtverec v pravé horní části appletu). Uvnitř tohoto čtverce se současně vykresluje inverzní barva k aktuálně nastavené hodnotě.

 - **PaletReprezObr** - Applet znázorňuje strukturu a principy paletové (indexové) reprezentace barev v obrazu. Hodnota pixelu v obraze nezastupuje přímo jeho barvu, ale jako ukazatel odkazuje na pozici v převodní tabulce palety barev. Pomocí nastavení v levé horní části appletu si můžeme vybrat jednu z předdefinovaných velikostí obrazu (matice) s pevně definovaným vzorem, případně provést nahodilé vyplnění matice náhodným rozmístěním indexů 1 - 6, které představují konkrétní barvy palety (lze přenastavit v pravé horní části appletu).

 - **PrevodBarObrSedot** - Převod vybraného barevného obrázku do šedotónové podoby. V levé části appletu se nachází originální obrázek, vpravo se vykresluje přepočtený snímek. Uživatel si může vyzkoušet jednu ze tří metod - průměrování hodnot jednotlivých barevných kanálů RGB modelu, vlastní nastavení jednotlivých složek RGB kanálu a také skrz převod do barevného prostoru Lab.

 - **NepraveBarvy** - Applet demonstrující techniku umělého obarvení obrazu pomocí vybraných barevných palet. V levé části appletu se nachází originální obrázek, vpravo se vykresluje přepočtený snímek. Uživatel má možnost definice vlastní palety výběrem palety s názvem Lineární gradient, tím se zpřístupní další ovládací prvky pro nastavení koncových bodů skrz jednotlivé barevné kanály RGB modelu, kterými může uživatel omezit barevný rozsah původního šedotónového gradientu. Při této úpravě dojde k interpolaci všech hodnot mezi oběma nastavenými koncovými body a výsledek se vykreslí v podobě výstupního obrazu do pravé části appletu. Na závěr je možné také otestovat vliv gamma korekce pro nastavenou barvicí paletu, výsledek se rovněž promítne do výstupního snímku.
 
## Pokyny k instalaci:

Je doporučeno nejprve umístit applety na web, při spuštění z lokálního disku/PC nemusí applety správně fungovat. Toto se týká zejména appletů:

 - Převod barevného obrazu na šedotónový
 - Převod šedotónového obrazu na barevný (nepravé barvy)