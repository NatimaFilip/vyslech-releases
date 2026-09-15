# Výslech – stažení a instalace

Výslech je interní appka Natima / Natios pro Mac a Windows. Třikrát denně se zeptá, co děláš, z odpovědí složí denní souhrn a v pátek ho pošle do Freela.

## Který soubor stáhnout

Klikni na svůj řádek, stažení začne hned (vždy nejnovější verze):

| Máš | Stáhni |
| --- | --- |
| **Mac s čipem Apple** (M1, M2, M3, M4…) | **[Stáhnout Vyslech-mac-arm64.dmg](https://github.com/NatimaFilip/vyslech-releases/releases/latest/download/Vyslech-mac-arm64.dmg)** |
| **Mac s procesorem Intel** | **[Stáhnout Vyslech-mac-x64.dmg](https://github.com/NatimaFilip/vyslech-releases/releases/latest/download/Vyslech-mac-x64.dmg)** |
| **Windows** | **[Stáhnout Vyslech-win-setup.exe](https://github.com/NatimaFilip/vyslech-releases/releases/latest/download/Vyslech-win-setup.exe)** |

Nevíš, jaký máš Mac? Klikni na  vlevo nahoře → **O tomto Macu**. „Čip Apple M…“ = arm64, „Procesor Intel“ = x64. Když si nejsi jistý, zkus arm64; na Intelu se prostě nespustí a stáhneš druhý.

Všechna vydání: [Releases](https://github.com/NatimaFilip/vyslech-releases/releases). Instalátor **neobsahuje AI klíč**, ten dostaneš od Filipa jako soubor a vložíš ho jednou v Nastavení (viz níže). Po aktualizaci zůstane.

## Instalace na Macu

Nic se nepíše do Terminálu. Jen klikání.

1. Otevři stažený soubor `.dmg` (dvojklik). Objeví se okno s ikonou **Vyslech** a složkou **Aplikace**.
2. Přetáhni ikonu Vyslech na složku Aplikace. Okno zavři, `.dmg` můžeš smazat.
3. Otevři složku **Aplikace** (Finder → Aplikace) a dvakrát klikni na **Vyslech**.
4. macOS ukáže hlášku, že aplikaci nelze otevřít, protože Apple nemůže ověřit, že neobsahuje malware. Klikni **Hotovo** (ne „Přesunout do koše“).
5. Otevři **Systémová nastavení** (ikona ozubeného kola v Docku nebo  → Systémová nastavení) → v levém sloupci **Soukromí a zabezpečení** → sjeď úplně dolů k části **Zabezpečení**. Je tam věta „Aplikace Vyslech byla zablokována…“ a vedle ní tlačítko **Přesto otevřít**. Klikni na něj, potvrď **Otevřít** a zadej heslo k Macu nebo použij Touch ID.
6. Vyslech se spustí: ikona mikrofonu se objeví v horní liště u hodin a otevře se okno s Nastavením. Tohle povolení děláš jen jednou, pak už appka startuje normálně.
7. Do Docku: zatímco appka běží, klikni pravým na její ikonu v Docku → **Volby** → **Ponechat v Docku**.
8. Při prvním výslechu se macOS zeptá na mikrofon, klikni **Povolit**. Kdybys klikl Nepovolit, napravíš to v Systémová nastavení → Soukromí a zabezpečení → Mikrofon.
9. macOS ještě oznámí, že se Vyslech přidal mezi položky přihlášení. To je správně, appka se má spouštět sama po zapnutí počítače.

Na starším macOS (13, 14) jde krok 4 a 5 nahradit takto: ve složce Aplikace klikni na Vyslech **pravým tlačítkem → Otevřít → Otevřít**.

Až bude appka podepsaná u Apple, kroky 4 a 5 zmizí a appka se prostě otevře.

## Instalace na Windows

1. Spusť stažený `.exe` (dvojklik).
2. Objeví se modré okno „Systém Windows ochránil váš počítač“. Klikni na **Další informace** a pak na **Přesto spustit**.
3. Instalace proběhne sama a appka se spustí. Ikona mikrofonu je vpravo dole u hodin (někdy schovaná pod šipkou ˄), zástupce je na ploše a v nabídce Start.
4. Při prvním výslechu appka požádá o mikrofon, povol ho. Když je mikrofon vypnutý pro všechny aplikace: Nastavení → Soukromí a zabezpečení → Mikrofon → povolit přístup pro desktopové aplikace.

## První nastavení (Mac i Windows)

Po prvním spuštění se otevře Nastavení:

1. **Jméno a příjmení** – tak se bude jmenovat tvůj podúkol ve Freelu.
2. **AI klíč** – klikni **Načíst klíč ze souboru…** a vyber soubor od Filipa (např. `vyslech-klic.env`). Nebo klíč vlož jako text do pole. Pak klikni **Otestovat**, musí se ukázat „funguje“.
3. **Freelo e-mail** – e-mail, kterým se přihlašuješ do Freela.
4. **Freelo API klíč** – ve Freelu klikni na svůj avatar vpravo nahoře → **Nastavení** → sjeď úplně dolů na sekci **API klíč** a zkopíruj ho sem. Klikni **Otestovat**; musí se ukázat „funguje, účet …“. Když hlásí, že nevidíš úkol Týdenní souhrn aktivit, napiš Filipovi, ať tě přidá do projektu.
5. Volitelně zapni **Číst otázky nahlas** a vyber hlas (tlačítko Přehrát ukázku).
6. Klikni **Uložit**. Okno můžeš zavřít, appka běží dál v liště.

Časy výslechů jsou 8:15, 11:15 a 15:00 v pracovní dny (v Nastavení si je můžeš posunout, počet tří zůstává). V daný čas vyskočí okno appky do popředí a přijde notifikace; klikni na **Začít výslech** (nebo kdykoli na ikonu v liště → **Odpovědět na výslech**). Odpovídáš mikrofonem (klikni na kulaté tlačítko, mluv, klikni znovu) nebo tlačítkem **Raději napsat**.

## Aktualizace

Appka se neaktualizuje sama, ale sama ti řekne, že je nová verze: na Přehledu se objeví modrý pruh s tlačítkem **Stáhnout** (nebo Nastavení → Zkontrolovat novou verzi).

1. Ukonči appku: ikona v liště → **Ukončit Výslech**.
2. Klikni na Stáhnout a nový instalátor nainstaluj stejně jako poprvé. Na Macu při přetažení do Aplikací potvrď **Nahradit** a při prvním otevření znovu projdi **Přesto otevřít** v Systémových nastaveních. Na Windows projdi SmartScreen jako poprvé.
3. Jméno, klíče i historie zůstanou, jsou uložené mimo aplikaci.

## Když něco nejde

- „Neplatný AI Gateway klíč“ → klíč je špatně vložený nebo byl zrušený, načti nový soubor od Filipa.
- „Vyčerpaný kredit nebo denní rozpočet“ → klíč má denní limit, zkus to zítra nebo napiš Filipovi.
- Freelo test hlásí, že nevidíš rodičovský úkol → nech se přidat do projektu ve Freelu.
- Přepis je nepřesný → v Nastavení vyber správný mikrofon (ne ten v monitoru) a udělej Zkušební nahrávku, má ukázat úroveň aspoň 30 %. Mluv blíž. Do Slovníku pro přepis napiš názvy projektů a jména, která říkáš často.
- Appka nevidí mikrofon → zkontroluj mikrofon v systémovém nastavení, nebo odpověz tlačítkem Raději napsat.
