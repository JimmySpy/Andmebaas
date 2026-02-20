2+ miljoni rea sisestamine igasse mitte-lookup tabelisse (AI abil)
 Grupp: IS24

Eesmärk
Luua skript (kasuta Bun-i), mis täidab sinu skeemi tabelid realistlike andmetega nii, et vähemalt ühes tabelis on vähemalt 2 000 000 rida ning teistes tabelites võimalikult palju ridu, säilitades tervikluse ja jõudluse.

Nõuded
Vähemalt ühes mitte-lookup tabelis ≥ 2 000 000 rida.
Teistes mitte-lookup tabelites maksimaalne mõistlik maht, proportsioonid põhjendatud.
Andmed peavad välja nägema ehtsad (nimed, e-kirjad, aadressid, summad, kuupäevad, seosed).
Võõrvõtmed kehtivad, orvukirjeid ei ole.
Sisestus toimub partiidena mass-sisestuse võtetega, mitte rida-real.
Indeksite strateegia: minimaalsed sisestuse ajal, taastamine pärast täitmist.
Lahendus peab olema reprodutseeritav (fikseeritud seeme või muu mehhanism).
Tulemus esitatakse Git-repo lingina.
Esitamise vorm
Repos peavad olema:

dump.sql – skeem.
Seemneskript – skript, mis täidab skeemi suurandmetega.
README.md – samm-sammuline juhend nullist käivitamiseks:

eeldused (andmebaasi versioon, tööriistad, .env väärtused),
käsud andmebaasi loomiseks ja dump’i laadimiseks,
seemneskripti käivitamise juhend,
oodatud tulemus (milline tabel saavutab 2M rida, teiste mahud ka).
Repo nime nõue
Repo nimi peab kajastama projekti iseloomu.
Keelatud on geneerilised või sisutud nimed (nt andmebaasiskeema-loomine, projekt1, testrepo).
Soovitatav on kasutada nime, mis peegeldab andmebaasi teemat või ülesande sisu (nt filmide-andmebaas, e-pood, auto24-kloon).
Soovituslik töövoog
Skeemi kaardistus: märgi lookup vs mitte-lookup tabelid; joonista sisestusjärjekord.
Andmesünteesi kavand: kirjelda, kuidas genereeritakse igale väljale realistlik väärtus.
Partiipõhine genereerimine: vali partiisuurused, kasuta transaktsioone.
FK-järjekord: sisesta esmalt viidatavad tabelid, siis viitavad tabelid.
Indeksite käsitlemine: mass-sisestuse ajaks minimaalsed indeksid, taastamine hiljem.
Paralleelsus: täida sõltumatuid osi paralleelselt.
Hindamiskriteeriumid
PASS

Vähemalt ühes mitte-lookup tabelis ≥ 2 000 000 rida.
Teistes mitte-lookup tabelites maksimaalselt mõistlik maht, proportsioonid põhjendatud.
Andmed näevad ehtsad välja.
Võõrvõtmed kehtivad, orvukirjeid ei ole.
Sisestus tehtud partiidena mass-sisestuse võtetega.
Lahendus on reprodutseeritav.
Repo nimi on sisuline, mitte geneeriline.
Repo sisaldab dump.sql, seemneskripti ja README.md.
README.md põhjal saab nullist lahenduse edukalt käima.
READMEs on kirjas milline tabel on 2M, teistes mahud, kestus, ehtsuse ja tervikluse kirjeldus.

Kriteeriumid
Ülesande esitamiseks peavad kõik kriteeriumi olema tethud.

Kõigis mitte-lookup tabelites on ≥ 2 000 000 rida.
Andmed näevad ehtsad välja (väljade semantika on usutav, kirjeldatud on kasutatud lokaate/formaate/vahemikke).
Võõrvõtmed kehtivad, orvukirjeid ei ole; sisestusjärjekord on loogiline.
Sisestus on tehtud partiidena ja kasutatud on mass-sisestuse tehnikaid.
Esitatud on raport: ridade arvud, kogukestus, ehtsuse tagamise kirjeldus, kinnitused tervikluse kohta.
Lahendus on reprodutseeritav (fikseeritud seeme või muu mehhanism).
Vähemalt ühes mitte-lookup tabelis ≥ 2 000 000 rida.
Teistes mitte-lookup tabelites maksimaalselt mõistlik maht, proportsioonid põhjendatud.
Andmed näevad ehtsad välja.
Võõrvõtmed kehtivad, orvukirjeid ei ole.
Sisestus tehtud partiidena mass-sisestuse võtetega.
Lahendus on reprodutseeritav.
Repo nimi on sisuline, mitte geneeriline.
Repo sisaldab dump.sql, seemneskripti ja README.md.
README.md põhjal saab nullist lahenduse edukalt käima.
READMEs on kirjas milline tabel on 2M, teistes mahud, kestus, ehtsuse ja tervikluse kirjeldus.
README juhised peavad olema vähemalt Dockeri jaoks. Windows ja Mac juhiste lisamine on vabatahtlik.