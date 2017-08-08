# React- ja Node.js-ohjelmointiprojektit

[React](https://facebook.github.io/react/) on Facebookin kehittämä JavaScript kirjasto interaktiivisten käyttöliittymien toteuttamiseen. Se on saavuttanut suuren suosion kehittäjien keskuudessa mm. yksinkertaisen ja joustavan komponenttirajapinnan, tehokkuuden vuoksi. Reactissa kaikki käyttöliittymäelementit ovat **komponentteja**: kirjautumislomake, navigaatipalkki, jne. Komponentit voivat sisältää toisia komponentteja muodostaen komponenttihierarkian. Komponentin päätehtävä on esittää dataa, jonka se saa sen vanhemmalta ja välittää tapahtumia (esim. painikkeen painallus komponentissa) sen vanhemmalle. Komponenttien visuaalinen esitys kuvataan usein Reactissa HTML:llää muistuttavalla **JSX** syntaksilla.

[Node.js](https://nodejs.org/en/) on Chromen V8 JavaScript moottorin päälle rakennettu asynkroninen ja tapahtumapohjainen suoritusympäristö. Node suunniteltiin skaalautuvien verkkosovelluskehittämiseen ja soveltuu erittäin hyvin mm. web-palvelinohjelmiston toteuttamiseen, vaihtoehdoksi esim. Rubylle ja Javalle. Noden pakettiekosysteemi [npm](https://www.npmjs.com/) on laajin avoimen lähdekoodin kirjastojen ekosysteemi. Nodea on hypetetty viime vuosina todella paljon ja osittain syystäkin. Vaikka Node häviää raa'assa laskentatehossa esim. Javalle, soveltuu se hyvin sovelluksiin, jotka voivat hyödyntää sen ei-blokkaavia I/O-operaatioita.

Kurssi(t) suoritetaan hyväksytty/hylätty merkinnällä toteuttamalla vain jompikumpi tai molemmat projektit. **Kummastakin kurssista voi saada maksimissaan viisi opintopistettä**. **Ansaitut opintopisteet määräytyvät projekteihin käytettyjen työtuntien perusteella, niin että n. 15 työtuntia vastaa aina yhtä opintopistettä**. Oman projektin aiheen saa itse päättää, mutta siinä täytyy käyttää pääosin projektin teknologiaa (siis joko React tai Node.js).  

:warning: **Kursseilla vaaditaan kohtalaisia JavaScript taitoja, eikä sen aikana käydä läpi mitään JavaScriptiin itseensä liittyviä asioita. Jos et osaa yhtään JavaScriptiä, kurssien työmäärä on todella suuri. Kurssit suoriteen myös erittäin itsenäisesti ja resursseja täytyy pystyä etsimään itse (hyödyllisiä resursseja toki jaetaan jossain määrin).**

:mega: **Kursseilla on yhteinen [Telegram](https://telegram.org/) keskustelualue, joka löytyy [täältä](https://t.me/joinchat/AAAAAELqEtpB36A8KkYo_Q). Keskustelualueelle voi kysyä kysymyksiä Reactiin ja Nodeen liittyen ja vastata muiden opiskelijoiden kysymyksiin. Ohjaajan nikki on kaltsoon.**

## Ohjaajan yhteystiedot

* Nimi: Kalle Ilves
* Telegram: kaltsoon
* Email: kalle.ilves[at]helsinki.fi

## Aikataulu

Kurssit kestävät kaksi viikkoa ja niiden aikataulut ovat samat (yhteinen aloitusluento ja yhteinen ohjaustuokio).

* Aloitusluento: 8.5. klo 16-18 luokassa D122
  * [Täältä](https://docs.google.com/presentation/d/1Ub9hfh4eJJx2pC3yjwcGrjhsXPrb_C8iUY7dRRM9oP8/edit?usp=sharing) löytyy aloitusluennon diat
* Ohjaustuokio: 11.5. klo 14-16 luokassa B221
* Projektin palautuksen deadline: 26.5. klo 23:59 (koskee molempia projekteja). Katso palautustapa "Suorittaminen"-osiosta alapuolelta

## Suorittaminen

1. Luo projektillesi [GitHub](https://github.com) repositorio :house_with_garden:. Lisä repositorioosi `README.md` tiedosto, jossa kuvailet lyhyesti, mistä projektissasi on kyse ja annat lyhyet asennus- ja käynnistysohjeet (esim. "Lataa tämän repositorion lähdekoodi, suorita `npm install` ja sen jälkeen `npm start`"). Kerro asennusohjeissa myös, miten projektisi testit suoritetaan (esim. "Suorita testit suorittamalla `npm test`").

2. Toteuta unelmiesi projekti 🦄 ✨ 
   * **Älä aloita liian kunnianhimoisesta projektista** ("aion tehdä Facebookin")! Aloita perustoiminallisuuksista ja rakenna sen ympärille toiminallisuutta kurssin aikarajan puitteissa ([Walking Skeleton](http://alistair.cockburn.us/Walking+skeleton)).
   * Pidä työtunneistasi tuntikirjanpitoa, esim. [Google Sheetsiin](https://www.google.com/sheets/about). **Ei tuntikirjanpitoa, ei kurssisuoritusta**:exclamation:
      * Tee jokaisen työpäiväsi päätteeksi merkintä tuntikirjanpitoosi. Merkinnän tulee sisältää **päivämäärä, lyhyt kuvaus, mitä teit projektiisi liittyen ja käyttämäsi työtunnit**. Lisää myös johonkin **työtuntiesi summa**. **Tuntikirjanpidon työtunnit määräävät saamasi opintopisteet**, joten niiden kirjaaminen on erittäin tärkeää.
      * Aihealueeseen perehtyminen kerryttää myös työtuntejasi, joten muista kirjata myös opiskeluun käyttämäsi työtunnit. Kerro kuvauksessa lyhyesti, mitä opit.
      * **Jos teet sekä React, että Node.js ohjelmointiprojektit, erittele niihin käytetyt työtunnit toisistaan** (käytä esim. kahta välilehteä Google Sheetsissä).
   * Kirjoita testejä(!) Testaaminen on kivaa, kun työkalut ovat oikeat. Mitään testikattavuusvaatimuksia ei ole, mutta **on tärkeää, että opit mitä kannattaa testata ja miten**.
   * Käytä mielellään [CI](https://en.wikipedia.org/wiki/Continuous_integration)-palvelinta (kuten [Travis](https://travis-ci.org/)) testiesi suorittamiseen. Miksi? Jokaisen toiminallisuuden lisäämisen yhteydessä haluat varmistaa, ettei sen integroiminen riko mitään muuta osaa sovellustasi. Testien suorittaminen manuaalisesti ennen jokaisen commitin pushaamista on mahdoton ajatus. Jos sovellusta kehittää useampi henkilö, CI-palvelin on käytännössä välttämättömyys, joten siihen kannattaa tutustua jo nyt. 
   * Julkaise projektisi, mieluiten niin usein kuin mahdollista ([Continuous Delivery](https://en.wikipedia.org/wiki/Continuous_delivery))
      * Jos toteutat pelkän React sovelluksen (ei palvelinpuolen toteusta), niin [Firebase](https://firebase.google.com/docs/hosting/quickstart) on yksi varteenotettava julkaisualusta. 
      * Jos toteutat Node.js sovelluksen (joka yksinään, tai React sovelluksen kera), niin [Heroku](https://devcenter.heroku.com/articles/getting-started-with-nodejs#introduction) on yksi hyvä vaihtoehto.
      * **Julkaise sovelluksesi "From day one"**. Sovelluksestasi ei ole hirveästi iloa, jos se on käytettävissä vain omalla koneellasi.
   * Tutustu [React](https://github.com/Kaltsoon/react-nodejs-projektit-k17/wiki/React-resurssit) ja/tai [Node.js](https://github.com/Kaltsoon/react-nodejs-projektit-k17/wiki/Node.js-resurssit) resursseihin, riippuen minkä/mitkä projektit aiot tehdä.    
3. Palauta projektisi kurssin deadlineen mennessä [tämän lomakkeen](https://docs.google.com/forms/d/e/1FAIpQLSchdQ0SzBoBHR3XETaS7dajE0n8oL_L1uMTogk5QfS0zP9X4Q/viewform?usp=sf_link) kautta :package: