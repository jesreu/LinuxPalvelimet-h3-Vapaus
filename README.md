# LinuxPalvelimet-h3-Vapaus
    Kirjoittanut: Jesse Reunamo
    Kurssi:       Linux-palvelimet
    Linkki:       https://terokarvinen.com/2023/linux-palvelimet-2023-alkukevat/

## Tiivistelmä
Raportti erilaisista lisensseistä ja linux komentorivin toiminnoista

## Vapaa ohjelmisto ja avoin lähdekoodi

Vapaassa ohjelmistossa saat oikeudet: ajaa, kopioida, levittää, opiskella, muuttaa ja kehittää ohjelmistoa. Avoimen lähdekoodin ohjelmistoissa saat oikeudet: ajaa, kopioida, levittää, muuttaa ja opiskella ohjelmistoa. Käytännössä kaikki vapaat ohjelmistot ovat myös avoimen lähdekoodin ohjelmistoja, mutta kaikki avoimen lähdekoodin ohjelmistot eivät täytä vapaan ohjelmiston määritelmää. Avoimen lähdekoodin vaatimukset voivat olla hieman tiukempia, kuin vapaan. 

## Tehtävässä h2 asennettujen ohjelmien lisenssit

Asensin tehtävässä h2 ohjelmat: Terminator, Cool retro term ja terminology. Nyt haluaisin selvittää kunkin ohjelman käyttölisenssit.

### Terminator

    Lisenssi:     GNU GPL v2 licence
    Lähde:        Ohjelmiston dokumentaation sivulta
    Vapaa:        Kyllä
    
Oikeusvaikutukset: Käyttäjä voi hyvin vapaasti muokata, levittää, käyttää ja tutkia ohjelmistoa, kunhan pitää huolen lisenssin jatko leviämisestä mahdollisiin muokattuihin versioihin. 

### Cool retro term

    Lisenssi:     GNU GPL v2/3 licence
    Lähde:        Ohjelmiston github repo
    Vapaa:        Kyllä
    
Oikeusvaikutukset: Käyttäjä voi hyvin vapaasti muokata, levittää, käyttää ja tutkia ohjelmistoa, kunhan pitää huolen lisenssin jatko leviämisestä mahdollisiin muokattuihin versioihin. 

Epäselvää: Valitettavasti github repossa on molemmat 2.0 ja 3.0 GNU GPL licenssit, joten on vaikeaa sanoa kumpi versio on juuri se mitä ohjelmisto noudattaa. 

### Terminology

    Lisenssi:     BSD 2-Clause License
    Lähde:        Ohjelmiston github repo
    Vapaa:        Kyllä
    
Oikeusvaikutukset: Mahdollistaa koodin käyttämisen, muokkaamisen, levittämisen kunhan lisenssi siirtyy muokattuihin/levitettyhin versioihin. 

## Säännölliset lausekkeet

Säännöllisten lausekkeiden testausta varten luon uuden tekstitiedoston microlla komennolla `micro regex.txt` ja lisään tiedostoon testidataa.

![regex](https://user-images.githubusercontent.com/112503770/214770396-4d61852c-5b9f-43cd-8c15-02fe0667d0c8.png)


Nyt voimme testata säännöllisiä lausekkeita tiedostolla.

    grep -P 'K...a' regex.txt
    grep -P 'M.' regex.txt
    
Ensimmäinen komento hakee kaikki rivit joissa sanaa alkaa K kirjaimella ja päättyy a kirjaimeen, (.) merkki säännöllisissä lausekkeissa vastaa mitä tahansa merkkiä.
Toinen komento taas hakee kaikki rivit joissa on M kirjaimella alkava sana. 

![regex2](https://user-images.githubusercontent.com/112503770/214770409-2e599fd5-9bfe-4053-8d06-5da065d690b6.png)


## Putkittaminen
Putkittamisella tarkoitetaan | merkin käyttöä komennoissa. Merkin avulla voimme siirtää tietoa ensimmäiseltä komennolta toiselle. Voimme suorittaa edellisen tehtävän komennot myös putkittamalla ne. 

    cat regex.txt | grep -P 'K...a'
    cat regex.txt | grep -P 'M.'
    
![putkitus](https://user-images.githubusercontent.com/112503770/214770457-9cc6f505-e205-4e0d-9533-579f94f13f5c.png)

## Lähteet

    https://www.gnu.org/philosophy/free-sw.html
    http://lib.tkk.fi/Diss/2005/isbn9529187793/isbn9529187793.pdf
    https://www.gnu.org/philosophy/open-source-misses-the-point.html
    https://terminator-gtk3.readthedocs.io/en/latest/licensing.html
    https://github.com/Swordfish90/cool-retro-term/blob/master/gpl-2.0.txt
    https://github.com/borisfaure/terminology
    
