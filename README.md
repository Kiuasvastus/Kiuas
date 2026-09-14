# K.I.U.A.S. — verkkosivut

Seuran etusivu. Yksi staattinen HTML-tiedosto, ei kehystä eikä käännösvaihetta.
Julkaistaan GitHub Pagesilla.

## Tiedostot

```
index.html      koko sivu: rakenne, tyylit, skriptit ja logo samassa tiedostossa
favicon.png     välilehden ja puhelimen kotinäytön ikoni
og.jpg          kuva joka näkyy kun linkki jaetaan (WhatsApp, Telegram, some)
fonts/          Familjen Grotesk ja IBM Plex, tarjoillaan omalta palvelimelta
```

Kaikki tiedostot kuuluvat repon juureen. Älä siirrä niitä alikansioihin —
`index.html` viittaa niihin suhteellisilla poluilla.

## Sisällön muokkaaminen

Kaikki teksti on `index.html`:ssä `<body>`-osiossa. Kaksi sääntöä:

1. **Jokainen teksti on kahtena kielenä.** Esimerkiksi:

   ```html
   <span lang="fi">Tulevat tapahtumat</span><span lang="en">Upcoming events</span>
   ```

   Muokkaa **molemmat**. Jos muokkaat vain suomen, englanninkielinen sivu
   näyttää vanhaa tekstiä eikä virhettä tule mistään.

2. **Sähköpostiosoitetta ei kirjoiteta näkyviin.** Se kootaan selaimessa,
   jotta roskapostirobotit eivät löydä sitä. Muokkaa vain attribuutteja:

   ```html
   <a class="mail" data-user="hallitus" data-domain="kiuas.rocks">
   ```

## Navigaatio ja lämpömittari

Oikean reunan lämpömittari rakentuu automaattisesti yläpalkin navigaation
perusteella. Kun lisäät tai poistat linkin yläpalkista, mittarin merkinnät,
asteet ja korkeudet päivittyvät itsestään. Mittaria ei tarvitse koskea.

Mittari näkyy vain yli 1280 pikselin leveydellä. Sitä kapeammalla yläpalkin
navigaatio hoitaa saman tehtävän.

## Mitä sivu EI tee

Ei evästeitä. Ei analytiikkaa. Ei lomakkeita. Ei yhtään ulkopuolista
verkkopyyntöä — fontitkin tulevat omalta palvelimelta. Siksi sivusto ei
tarvitse evästeilmoitusta eikä tietosuojaselostetta.

Jos lisäät myöhemmin analytiikan, upotetun kartan, YouTube-videon tai
yhteydenottolomakkeen, tämä ei enää pidä paikkaansa ja tietosuoja-asiat
on käytävä läpi uudelleen.

## Lisenssit

Fontit ovat SIL Open Font License 1.1 -lisenssin alaisia. Lisenssitiedostot
ovat `fonts/`-kansiossa ja niiden on pysyttävä siellä.
