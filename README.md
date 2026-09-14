# Výslech – stažení a instalace

Výslech je interní appka Natima / Natios pro Mac a Windows. Čtyřikrát denně se zeptá, co děláš, z odpovědí složí denní souhrn a v pátek ho pošle do Freela.

**Stáhnout nejnovější verzi: [Releases → Latest](https://github.com/NatimaFilip/vyslech-releases/releases/latest)**

V sekci _Assets_ vyber soubor pro svůj počítač:

| Počítač                                  | Soubor                          |
| ---------------------------------------- | ------------------------------- |
| Mac s čipem Apple (M1, M2, M3, M4…)      | `Vyslech-x.y.z-mac-arm64.dmg`   |
| Mac s procesorem Intel                   | `Vyslech-x.y.z-mac-x64.dmg`     |
| Windows                                  | `Vyslech-x.y.z-win-setup.exe`   |

Nevíš, jaký máš Mac? Klikni na  vlevo nahoře → **O tomto Macu**. „Čip Apple M…“ = arm64, „Procesor Intel“ = x64.

Instalátor **neobsahuje AI klíč**. Ten dostaneš od Filipa jako soubor nebo text a vložíš ho jednou v Nastavení (viz níže). Po aktualizaci zůstane.

## Instalace na Macu

1. Otevři stažený soubor `.dmg` (dvojklik). Objeví se okno s ikonou Vyslech a složkou Aplikace.
2. Přetáhni ikonu **Vyslech** na složku **Aplikace**. Okno zavři, `.dmg` můžeš smazat.
3. Appka není podepsaná u Apple, proto ji macOS poprvé odmítne. Otevři **Terminál** (⌘ + mezerník, napiš „Terminál“, Enter), vlož tento řádek a stiskni Enter:
   ```
   xattr -cr /Applications/Vyslech.app
   ```
   Terminál nic nevypíše, to je správně. Kdyby macOS přesto hlásil, že je appka poškozená nebo od neověřeného vývojáře: Systémová nastavení → Soukromí a zabezpečení → sjeď dolů → **Přesto otevřít**.
4. Ve složce Aplikace spusť **Vyslech**. Ikona mikrofonu se objeví v horní liště u hodin a otevře se okno s Nastavením.
5. Do Docku: zatímco appka běží, klikni pravým na její ikonu v Docku → Volby → **Ponechat v Docku**.
6. Při prvním výslechu se macOS zeptá na mikrofon, klikni **Povolit**. Když klikneš Nepovolit, napravíš to v Systémová nastavení → Soukromí a zabezpečení → Mikrofon.
7. macOS oznámí, že se Vyslech přidal mezi položky přihlášení. To je v pořádku, appka se má spouštět sama po zapnutí počítače.

## Instalace na Windows

1. Spusť stažený `.exe`.
2. Objeví se modré okno „Systém Windows ochránil váš počítač“, protože instalátor není podepsaný. Klikni **Další informace** a pak **Přesto spustit**.
3. Instalace proběhne sama a appka se spustí. Ikona je vpravo dole u hodin (někdy pod šipkou ˄), zástupce je na ploše a v nabídce Start.
4. Při prvním výslechu appka požádá o mikrofon, povol ho. Když je mikrofon blokovaný globálně: Nastavení → Soukromí a zabezpečení → Mikrofon → povolit pro desktopové aplikace.

## První nastavení (Mac i Windows)

Po prvním spuštění se otevře Nastavení:

1. **Jméno a příjmení** – tak se bude jmenovat tvůj podúkol ve Freelu.
2. **AI klíč** – klikni **Načíst klíč ze souboru…** a vyber soubor od Filipa (např. `vyslech-klic.env`). Nebo klíč vlož jako text do pole. Pak klikni **Otestovat**, musí se ukázat „funguje“.
3. **Freelo e-mail** – e-mail, kterým se přihlašuješ do Freela.
4. **Freelo API klíč** – ve Freelu klikni na svůj avatar vpravo nahoře → **Nastavení** → sjeď úplně dolů na sekci **API klíč** a zkopíruj ho sem. Klikni **Otestovat**; musí se ukázat „funguje, přihlášen jako …“. Když hlásí, že nevidíš úkol Týdenní souhrn aktivit, napiš Filipovi, ať tě přidá do projektu.
5. Volitelně zapni **Číst otázky nahlas** a vyber hlas (tlačítko Přehrát ukázku).
6. Klikni **Uložit**. Okno můžeš zavřít, appka běží dál v liště.

Časy výslechů jsou 8:30, 11:00, 13:30 a 15:30 v pracovní dny (v Nastavení si je můžeš posunout, počet čtyř zůstává). V daný čas přijde notifikace, klikni na ni nebo na ikonu v liště → **Odpovědět na výslech**. Odpovídáš mikrofonem (klikni na kulaté tlačítko, mluv, klikni znovu) nebo tlačítkem **Raději napsat**.

## Aktualizace

Appka se neaktualizuje sama, ale sama ti řekne, že je nová verze (banner na Přehledu s tlačítkem Stáhnout, nebo Nastavení → Zkontrolovat novou verzi).

1. Ukonči appku: ikona v liště → **Ukončit Výslech**.
2. Stáhni nový instalátor a postupuj jako při instalaci. Na Macu potvrď **Nahradit** a znovu spusť `xattr -cr /Applications/Vyslech.app`. Na Windows projdi SmartScreen jako poprvé.
3. Nastavení, klíče i historie zůstanou, leží mimo aplikaci:
   - Mac: `~/Library/Application Support/Výslech/`
   - Windows: `%APPDATA%\Výslech\`

## Když něco nejde

- „Neplatný AI Gateway klíč“ → klíč je špatně vložený nebo byl zrušený, načti nový soubor od Filipa.
- „Vyčerpaný kredit nebo denní rozpočet“ → klíč má denní limit, zkus to zítra nebo napiš Filipovi.
- Freelo test hlásí, že nevidíš rodičovský úkol → nech se přidat do projektu ve Freelu.
- Přepis nefunguje → zkontroluj mikrofon v systémovém nastavení, nebo odpověz tlačítkem Raději napsat.
