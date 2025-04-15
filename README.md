# Hospital db
 
Meeskond:
Tammo Tammisto
Kristi Kuus

Valitud andmebaas:
SQLITE

Miks valisime SQL-andmebaasi, mitte NoSQL?
Struktureeritud andmed
Tugevad seosed (JOINid)
Andmete terviklikkus ja reeglid
Tuntus ja tugi
Skaalautuvus
Kuna haigla süsteemis on palju seotust (patsiendid ↔ arstid ↔ ajad ↔ haiguslood ↔ arved jne), on SQL optimaalne.

Funktsionaalsed nõuded:
1. Patsiendi andmete haldamine
2.Arstide haldamine
3.Aja planeerimine
4.Protseduuride ja ravimite määramine
5.Patsiendi viibimine haiglas
6.Arsti ja õe koolitus
7.Töötajate ülesanded ja töögraafikud
8.Visiidiga seotud arved

Mittfunktsionaalsed nõuded:
1.Süsteem peab olema optimeeritud, et päringud, mis hõlmavad vähemalt 1000 patsiendi ja töötaja andmekirjeid, annaksid tulemusi vähem kui 2 sekundi jooksul.
2.Süsteem peab tagama andmete konfidentsiaalsuse ja turvalisuse, sh kasutajate autentimise ja volituste haldamise, et ainult volitatud töötajad pääseksid patsiendi andmetele juurde.
3.Skaleeritavus
4.Andmebaasis peab olema rakendatud vajalikud piirangud (nt võõrvõtmed, unikaalsuse piirangud), et vältida andmete sisestamisel vigade tekkimist. Kõik väljad, mis on määratud "NOT NULL", peavad olema täidetud õige ja kehtiva väärtusega.