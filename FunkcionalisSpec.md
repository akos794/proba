# Funkcionális Specifikáció

## Áttekintés

A projektünk célja egy olyan rendszer létrehozása ami segít a felhasználóknak
kikapcsolódást nyújtani a kártyajátékok világában. Szolgáltatásunk több féle platformon
szeretnénk elérhetővé tenni pl. számítógépes porgram vagy mobil applikáció formájában.
A rendszer teljesen ingyenesen használható lesz letöltés után mobilon, számítógépen vagy 
regisztrálás után internen is. A játékok nyomonkövetik, hogy a kezdés óta mennyit 
nyertünk és jelenleg milyen téttel játszunk. Minden kör után láthaja a felhasználó 
az aktuális nyereményét és egyenlegét.

## Használati esetek

Admin: Az admin beléphet minden más szerepkörbe, hogy a rendszer hibamentes működését ellenőrizhesse. Az admin(ok) feladata a rendszer problémamentes működése. Ez egyben jár azzal, hogy az egész rendszerhez van hozzáférésük. Az admin(ok)nak hozzá kell tudni férniük a felhasználók listájához, hogy az esetleges változásokat el tudják végezni. Tudniuk kell a felhasználók jogosultságait, szerepkörét, jelszavát, és felhasználónevét módosítani. Képesnek kell lenniük arra, hogy felhasználókat vegyenek fel a rendszerbe és, hogy rakjanak le belőle. Képesek üzenetet küldeni az összes felhasználónak, valamint globális üzeneteket, amelyeket mindenki megkap egyszerre.

## Jelenlegi helyzet

[KövetelménySpec](KovetelmenySpec.md#Jelenlegi-helyzet)

## Követelménylista

 Modul | ID | Név | v. | Kifejtés 
--- | --- | --- | --- | ---
Jogosultság | K1 | Bejelentkezési felület | 1.0 | A felhasználó az email címe és a jelszava segítségével bejelentkezhet. Ha a megadott email cím vagy jelszó nem megfelelő, akkor a felhasználó hibaüzenetet kap. 
Jogosultság | K2 | Regisztráció | 1.0 | A felhasználó a felhasználói nevének, email címének és jelszavának megadásával regisztrálja magát. A jelszó tárolása kódolva történik az adatbázisban.Ha valamelyik adat ezek közül hiányzik, vagy nem felel meg a követelményeknek, akkor a rendszer értesíti erről a felhasználót 
Jogosultság | K3 | Jogosultsági szintek | 1.0 | Admin: új játék lehetőségek feltöltése, Felhasználó: játékok indítása, toplista megtekintése, jelszó módosítása, Vendég: regisztráció, belépés 
Modifikáció | K4 | Felhasználó módosítása | 1.0 | A felhasználó módosítani tudja saját felhasználónevét. Ehhez szükséges a régi és az új felhasználónév megadása, az új megerősítése, valamint a felhasználó jelszavának megadása 
Modifikáció | K5 | Jelszó módosítása | 1.0 | A felhasználó módosítani tudja saját jelszavát. Ehhez szükséges a régi és az új jelszavának megadása, valamint az új megerősítése 
Modifikáció | K6 | Elfelejtett felhasználónév/jelszó | 1.0 | Ha a felhasználó elfelejtette a felhasználónevét, vagy a jelszavát akkor ezzel az opcióval egy Adminhoz tud fordulni 
Feladattípus | K7 | Poker | 1.0 | A játékos illetve az osztó is 2-2 lapot kap, az asztalra lekerült 5 lap után a nyertes viszi az összegyűlt nyereményt
Feladattípus | K8 | BlackJack | 1.0 | A játékosok illetve az osztó is 2-2 lapot kap, lehetőség van jabb lapok kérésére. Akinek 21-hez közelebbi lap értéke van az nyer és viszi az összegyűlt nyereményt
Statisztika | K9 | Topplista | 1.0 | Egy lista a játékosok pontszámairól, a lista elején a legtöbb pontot, zsetont elért felhasználó található.
Felület | K10 | Üzenetek | 1.0 | A felhasználók egymás között tudnak küldeni üzeneteket, jogosultságuktól függően
Felület | K11 | Fórum | 1.0 | Egy felhasználói fórum, ahol a felhasználók tudnak érdekességekről beszélni, vitatkozni
Jogosultság | K12 | Admin felület | 1.0 | Felület az admin fiókkal rendelkező felhasználó számára. Tartalmaz egy felületet az új játékok feltöltéséhez


## Képernyő tervek

Az applikáció megnyitásakor egy bejelentkező felületet kapunk<br>
<img src=https://github.com/SzutorRobert/AFP_LEV_2020_10/blob/develop/Doc/Login.jpg height="300px" width="150px" ><br>
Bejelentkezés után a menüben a felhasználó választhat a játékok közül, befizethet és látja az egyenlegét<br>
<img src=https://github.com/SzutorRobert/AFP_LEV_2020_10/blob/develop/Doc/Main.jpg height="150px" width="300px" ><br>
Poker választása után <br>
<img src=https://github.com/SzutorRobert/AFP_LEV_2020_10/blob/develop/Doc/Poker.jpg height="150px" width="300px" ><br>
BlackJack választása után<br>
<img src=https://github.com/SzutorRobert/AFP_LEV_2020_10/blob/develop/Doc/BlackJack.jpg height="150px" width="300px" ><br>


