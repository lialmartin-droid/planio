# Plánio 1.1.0

Osobní kalendář směn, dovolené, náhradního volna, svozů odpadu a vlastních událostí. Česká aplikace pro telefon i počítač, bez účtu a bez instalace balíčků.

## Nahrání na GitHub Pages

1. Rozbal ZIP.
2. Na GitHubu vytvoř repozitář, například `planio`.
3. Nahraj **obsah rozbalené složky** do kořene repozitáře. Soubor `index.html` musí být přímo v kořeni, společně s `app.mjs`, `core.mjs`, `styles.css`, `sw.js` a složkou `assets`. Nenahrávej samotný ZIP.
4. Otevři **Settings → Pages → Build and deployment**.
5. Vyber **Deploy from a branch**, větev **main**, složku **/(root)** a ulož.
6. Po dokončení publikace otevři odkaz, který GitHub zobrazí v Pages.

Po pozdější aktualizaci nahraj nové soubory na stejné místo. V aplikaci otevři **Nastavení → Zkontrolovat aktualizaci aplikace**. Aktualizace nemění klíč s uloženými záznamy. Pro jistotu si před aktualizací vždy stáhni zálohu.

## Instalace na iPhone

Otevři stránku GitHub Pages v **Safari**, klepni na **Sdílet → Přidat na plochu** a nech název **Plánio**. Aplikace má vlastní ikonu pro iPhone, favicon, PWA manifest a offline režim. Po prvním úspěšném načtení funguje i bez internetu.

Pro běžné používání se drž stejné ikony a zařízení. Různé prohlížeče nebo instalace nemusí sdílet stejné údaje. Samotný `index.html` otevřený z aplikace Soubory není vhodný způsob spuštění: moduly a offline režim potřebují webovou adresu.

## První nastavení

### 1. Pracovní cyklus

Klepni na **Cyklus**. Každá položka odpovídá jednomu pracovnímu týdnu. Výchozí pořadí je ranní → odpolední → noční; kliknutím na položku ji odebereš, tlačítkem přidáš další. Můžeš vytvořit libovolnou posloupnost včetně volného týdne a 12hodinových směn.

Vyber pondělí prvního týdne cyklu a datum, od kterého se má nový rozpis použít. Tlačítko **Vyplnit zbytek roku** nastaví opakování, které pokračuje i v následujících letech. Víkendy jsou automaticky volné. Volbu **Ve svátky automaticky volno** můžeš vypnout. Svátky neovlivňují posun týdenního cyklu.

Starší rozpis před datem změny zůstává zachovaný. Jednotlivé ručně změněné dny zůstávají zachované i po novém nastavení cyklu. Nemusíš nic doplňovat každý leden.

V **Časy a barvy směn** nastav názvy, začátky, konce, barvy a neplacené přestávky. Výchozí 8hodinové směny jsou 06–14, 14–22 a 22–06. U 12hodinových směn jsou výchozí časy 06–18 a 18–06. Přestávka je zpočátku 0 minut; zadej skutečnou neplacenou přestávku podle své evidence. Změna typu směny ovlivňuje všechny dny tohoto typu; jednorázové změny dělej v detailu dne.

### 2. Zbývající dovolená a náhradní volno

V **Moje volno** vyber rok a u dovolené, požární hlídky a první pomoci klepni na **Zadat zbývající hodiny**. Zadej aktuální zůstatek podle práce, například 60 hodin dovolené. Další zadané volno se automaticky odečte; týden pondělí–pátek spotřebuje 37,5 hodin a zbude 22,5 hodin.

Zadaný aktuální zůstatek je nová výchozí hodnota. Starší čerpání, které je již zahrnuté v tomto zůstatku, se neodečítá podruhé. Budoucí, už naplánované volno se od tohoto zůstatku dál rezervuje. Pole proto uvádí zůstatek podle práce **před odečtením budoucích plánů**. Další získané hodiny lze připsat zvlášť s datem.

**Dovolená na celý pracovní den spotřebuje vždy 7,5 h.** Nezáleží na tom, zda je směna v kalendáři zadaná jako osmihodinový časový rozsah. Celodenní volno znamená žádnou práci; nepočítá se zbylá půlhodina. Víkendy a svátky bez směny dovolenou nespotřebují.

U obou druhů náhradního volna vidíš samostatný stav **NEČERPÁNO**, **NAPLÁNOVÁNO** nebo **ČERPÁNO**, počet hodin a poslední čerpání. Pokud už bylo NV použité před zahájením evidence, při zadání zůstatku zaškrtni **NV jsem už v tomto roce čerpal mimo evidenci dnů**. Tato značka pouze potvrzuje čerpání; zadané zbývající hodiny nesnižuje znovu.

Volno na budoucí datum je naplánované. V dnešním a minulém datu se považuje za čerpané. Pokud se čerpání neuskutečnilo, záznam změň nebo zruš. Náhradní volno lze zadat na týden i vlastní období; počet hodin NV za celý den lze upravit.

Pokročilé zadání celoročního nároku zůstává pod rozbalovací volbou v dialogu. Tím lze znovu přejít na účetnictví od začátku roku. Pro běžné použití stačí aktuální zůstatek.

Každý rok má samostatné zůstatky. Nároky a převody zadáš podle skutečných údajů.

### 3. Svozy odpadu

V záložce **Svozy** přidej samostatná pravidla pro **směsný odpad, plasty a karton**. Zvol den týdne, první známý termín a interval, například každé 2 týdny. Cyklus je ukotvený v prvním známém datu, takže není závislý na sudém nebo lichém čísle kalendářního týdne. Pravidla pokračují přes přelom roku, dokud je neukončíš nebo nepozastavíš.

Každý jednotlivý svoz lze přesunout nebo zrušit. Ostatní termíny zůstávají zachované. Jednorázové změny jsou vypsané i pod seznamem svozů, odkud lze obnovit původní termín.

## Každodenní používání

- **Kalendář:** celé dny mají barvu směny. Dovolená a náhradní volno mají modré šrafování. Tečky označují svozy, značky další události a poznámky. Svátky mají výrazný zlatý rámeček a označení SV. Celý název je výrazně uvedený v detailu dne; tlačítko Přehled svátků zobrazí celý rok. Po klepnutí na den otevřeš všechny podrobnosti.
- **Čísla týdnů:** ISO týdny začínají pondělím; na přelomu roku patří týden k odpovídajícímu týdennímu roku. Existuje i týden 53.
- **Navigace:** šipky přepínají období, kulaté tlačítko vrací dnešek. Klepnutím na název měsíce vybereš měsíc a rok přímo. Lze přepnout měsíční a týdenní zobrazení.
- **Detail dne:** změň směnu jen pro daný den, zadej volno v hodinách a rozliš celou směnu či částečné volno, skutečně odpracované hodiny a poznámku. Pro výjimečnou sobotní směnu vyber skutečný typ směny.
- **Skutečnost:** prázdné pole znamená nezapsaný den, nikoliv 0 hodin. Zapsaná nula znamená skutečně odpracovaných 0 hodin. Přesčas je kladný rozdíl skutečnosti proti plánovaným pracovním hodinám po odečtení volna.
- **Chytré volno:** klepni na výrazné **+ Volno** přímo v kalendáři nebo na tlačítko v Moje volno. Zvol **Celý týden najednou** a libovolný den tohoto týdne, nebo **Vlastní období od–do**. Všechny pracovní dny se zadají jedním potvrzením. Sleduj potřebné hodiny, zůstatek i souvislé volno včetně okolních víkendů a svátků. Volno se zapíše pouze tam, kde je pracovní směna. Tlačítko Zrušit tento druh volna v období umožní vrátit celé období jedním potvrzením a uvolní jeho hodiny. Výpočet zohlední i již zadané volno. U překročení zůstatku nebo náhrady jiného druhu volna se zobrazí upozornění.
- **Vlastní události:** přidej lékaře, školení nebo rodinnou akci s poznámkou. Časy jsou volitelné; vyplň oba nebo ani jeden. Událost může být jednorázová nebo se opakovat po dnech, týdnech či měsících. Měsíční událost 31. dne vynechá měsíce bez 31. dne. Úprava opakované události platí pro celou sérii.
- **Přehled:** plánované hodiny, plán práce po odečtení volna, zapsaná skutečnost, přesčasy, počty směn, nočních a víkendových směn. Noční směny mají správně konec následující den. Pracovní hodiny představují smluvenou délku směny; změna letního času její délku automaticky nemění.
- **Vzhled a filtry:** tmavý, světlý nebo systémový režim; samostatně lze skrýt směny, volno, svozy, události a svátky.

## Připomínky a export do kalendáře

V nastavení nebo pod svozy vyber **Export kalendáře**, rok a typy záznamů. Stáhne se soubor `.ics`. Svozy obsahují připomenutí 1 nebo 2 dny předem v nastavený čas. Svoz je v exportu zapsaný v 08:00; tento čas je pouze orientační, skutečný čas svozu se neurčuje.

Soubor otevři nebo importuj v kalendářové aplikaci s podporou ICS. Nabídka importu záleží na aplikaci, kterou soubor na iPhonu otevřeš. Lze jej například importovat přes Kalendář na Macu do iCloudu a tím dostat do iPhonu. Vytvoř si pro import samostatný kalendář **Plánio**.

Po změně rozpisu proveď nový export a nahraď starý import; nejde o automatickou synchronizaci. Opakovaný import může způsobit duplicity podle použité kalendářové aplikace. Připomenutí následně zajišťuje systémový kalendář, nikoliv zavřená PWA. Plánio samo nemá server, který by na pozadí posílal push upozornění.

U částečného volna se pracovní směna v ICS uvádí v původním časovém rozsahu s označením „část směny“ a poznámkou o počtu pracovních hodin, protože samotný počet hodin volna neurčuje, kterou část dne nepracuješ.

## Zálohování a bezpečné uchování údajů

**Nastavení → Stáhnout zálohu** vytvoří JSON se všemi údaji. Ulož si ho do Souborů nebo iCloudu. **Obnovit zálohu** ověří strukturu a teprve po potvrzení nahradí současné údaje. Před obnovením si stáhni současnou zálohu.

Data zůstávají lokálně v prohlížeči. Neodesílají se na GitHub ani do jiných účtů. Smazání dat webu, soukromý režim, odinstalace aplikace nebo výměna telefonu mohou záznamy odstranit. Automatická kopie předchozího uložení pomáhá při poškozeném hlavním souboru, ale nenahrazuje vlastní staženou zálohu. Zálohu bez potřeby veřejně nezveřejňuj: obsahuje tvůj rozpis a poznámky.

## Ověření

Prošlo 33 automatických kontrol: datum a ISO týdny, svátky, směnový cyklus, víkendy, změna cyklu, noční směny, oddělené zůstatky, chytré plánování přes dva roky, svozy a jejich výjimky, opakované události, export ICS, obnova zálohy a napojení základních formulářů.

Nové kontroly ověřují také 7,5hodinovou dovolenou, zadání celého týdne, aktuální zůstatek bez dvojího odečítání, stavy náhradního volna a zvýraznění svátků.

Kontrola formulářů používá jednoduché prostředí bez prohlížeče. Nevypovídá o skutečném rozložení stránky, klávesnici ani importu ICS v iOS. Přímo na iPhonu a v Safari aplikace při této přípravě ověřena nebyla.

Pro vývojářské spuštění kontrol stačí Node.js: `node --test tests/*.test.mjs`. Pro běžné používání Node.js nepotřebuješ.

Zdroj přehledu českých svátků: [MPSV – zákon č. 245/2000 Sb.](https://ppropo.mpsv.cz/zakon_245_2000). Pohyblivé velikonoční svátky aplikace vypočítává pro vybraný rok.

## Aktualizace z verze 1.0.0

Nahraj nové soubory na stejné místo a v aplikaci spusť kontrolu aktualizace. Používá se stejný klíč uložených údajů; směny, svozy, poznámky a další záznamy zůstávají zachované. Staré zálohy lze načíst. Původní celodenní dovolená počítaná z celé směny se opraví na 7,5 hodin; částečné volno se zachová. Pak si v Moje volno případně nastav aktuální zůstatek podle práce.
