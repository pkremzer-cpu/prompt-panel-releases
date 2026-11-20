# Prompt Panel – kiadások

Ez a repó a **Prompt Panel** macOS-alkalmazás (Apple Silicon) **telepítőit** tartalmazza a
*Releases* oldalon. Forráskód nincs benne: a forrás privát repóban van.

Lebegő prompt-gombpanel a Claude és a ChatGPT asztali apphoz: gombnyomásra a hozzá tartozó, előre
megírt promptot beilleszti az éppen előtérben lévő AI-app szövegmezőjébe.

## Mit tartalmaz egy kiadás?

| Fájl | Tartalom |
|---|---|
| `Prompt-Panel-<verzió>-arm64.dmg` | telepítő (Apple Silicon, ad-hoc aláírással) |
| `Prompt_Panel_Telepitesi_utmutato.pdf` | telepítési és használati útmutató |
| `SHA256SUMS.txt` | SHA-256 ellenőrzőösszegek |

Ellenőrzés Terminálban, a letöltött fájlok mappájában: `shasum -a 256 -c SHA256SUMS.txt`

## Telepítés és frissítés

Lásd a kiadáshoz csatolt PDF-útmutatót. Röviden: nyisd meg a `.dmg`-t, húzd a **Prompt Panelt**
az **Applications** mappára (frissítésnél: **Csere**), majd indítsd el.

Az 1.1.0-tól az app naponta egyszer megnézi ennek a repónak a legfrissebb kiadását (névtelen
GitHub API-lekérdezés, személyes adat nélkül), és ha van újabb verzió, a panel alján jelzi.
Ez a menüsorban kikapcsolható (**Automatikus frissítéskeresés**).

## Licenc

Minden jog fenntartva – Kremzer Péter, 2026. A telepítő nem nyílt forráskódú szoftver; a benne
lévő harmadik féltől származó komponensek (Electron – MIT, uiohook-napi – MIT) licencei az
alkalmazáscsomagban találhatók.
