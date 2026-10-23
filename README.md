# iviKeyw

Az iviKeyw az **iviKeya Android-alkalmazás Windowsos fogadóprogramja**. A telefonon beolvasott vonalkódokat és QR-kódokat, valamint a kézi billentyűzeten küldött adatokat az aktív Windows-ablakba gépeli. Használható például Excelben vagy egy készletkezelő program beviteli mezőjében.

**A Windows-program díjmentes.** Az Android-alkalmazás jogosultsága külön kezelendő.

## Letöltés és telepítés

1. Töltsd le az [iviKeyw Windows-telepítőjét](https://github.com/ivisofthu/iviKeyw/releases/download/v2026.10.23-test/iviKeyw-Setup-2026.10.23-test.exe).
2. Indítsd el, válassz nyelvet, olvasd el és fogadd el a használati feltételeket.
3. Válaszd ki a telepítési helyet. Az asztali ikon és a Windows-bejelentkezéskori indítás opcionális.
4. Indítsd el az iviKeyw programot a Start menüből vagy az asztali ikonról.

**Rendszerigény:** Windows 10/11, x64. Python külön telepítése nem szükséges.

Alapértelmezett telepítési hely: `%LOCALAPPDATA%\Programs\iviSoft\iviKeyw`. A telepítés az aktuális felhasználóhoz történik, rendszergazdai jogosultság nélkül.

A telepítő nincs digitálisan aláírva, ezért a Windows biztonsági figyelmeztetést mutathat. Kizárólag az itt hivatkozott kiadásból töltsd le; ne kapcsold ki a Windows biztonsági védelmét. A kiadásnál SHA-256 ellenőrzőösszeg is található.

## Párosítás és használat

1. A telefon és a PC csatlakozzon ugyanahhoz a megbízható helyi hálózathoz.
2. Az iviKeyw alapból a tálcán indul. Az óra melletti iviKey ikonra kattintva nyisd meg az ablakot; az ikon a rejtett ikonok között is lehet.
3. Jelenítsd meg a PC-n a párosítási QR-kódot, és olvasd be az [iviKeya](https://github.com/ivisofthu/iviKeya) Beállítások oldalán. A QR-kód 9 másodperc után eltűnik, de újra megjeleníthető.
4. Válaszd ki a telefonon a PC-t és a kívánt slotot.
5. A PC-n kattints a célprogram megfelelő beviteli mezőjébe, majd olvasd be a kódot a telefonon.

A fogadó **mindig az aktív ablakba gépel**. Ellenőrizd a célmezőt és a bevitt eredményt. Ne hagyj parancssort vagy más, nem kívánt célablakot előtérben.

## Slotok és beállítások

| Slot | Alapértelmezett működés |
| --- | --- |
| S1 | Kód, majd Enter |
| S2 | Ctrl+N, kód, majd Enter |
| S3 | A kódban a `(SN)` utáni rész a következő `(` vagy sorvég előttig, majd Enter. Hiányzó vagy üres rész esetén nem gépel. |
| S4 | Csak a beérkezett adat |

A slotok neve és prefix/suffix műveletei a PC-n módosíthatók. A profilok külön JSON-fájlokként importálhatók és exportálhatók.

A **Beállítások** menüben a tálcán indulás és az összes bevitelre érvényes késleltetés állítható: **1–100 ms**, alapérték **2 ms**. A változásokat a főablak **Mentés** gombjával véglegesítsd.

## Hálózat és kilépés

- A telefon–PC kapcsolat HTTP-t használ, nem titkosított. Csak megbízható helyi hálózaton használd.
- A párosítási kulcsot és QR-kódot ne add át illetéktelennek.
- Ne állíts be internetes porttovábbítást. A telepítő nem módosítja a tűzfalat; szükség esetén csak a megbízható magánhálózaton engedélyezd a fogadó kapcsolatát.
- A program teljes leállításához használd a **Kilépés** parancsot.

## Eltávolítás és beállítások

Eltávolítás: **Windows Beállítások → Alkalmazások → iviKeyw → Eltávolítás**.

A beállítások és slotprofilok megmaradnak a `%LOCALAPPDATA%\iviSoft\iviKeyw` mappában. Ha már nincs rájuk szükség, biztonsági másolat készítése után ezt a mappát kézzel törölheted.

## Kapcsolat és licencek

**iviSoft / Duncsák Mihály egyéni vállalkozó**  
Weboldal: [ivisoft.hu](https://ivisoft.hu) · E-mail: [ivisoft@ivisoft.hu](mailto:ivisoft@ivisoft.hu)

A használati feltételek és az útmutató a telepített `legal` mappában találhatók. A külső összetevők licencei az `_internal\licenses` mappában érhetők el; a hozzájuk tartozó forráscsomag a [kiadás letöltései](https://github.com/ivisofthu/iviKeyw/releases/tag/v2026.10.23-test) között található. Ez a külső könyvtárak forrása, nem az iviKeyw saját alkalmazáskódja.
