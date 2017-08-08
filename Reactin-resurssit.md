## Miten pääsen alkuun?

1. Asenna [Node.js](https://nodejs.org/en/)
2. Ota ensiaskeleet Reactiin [täällä](https://facebook.github.io/react/docs/hello-world.html). Myös [tämä](https://reacttraining.com/online/react-fundamentals) React trainingin opas kannattaa kurkata.
3. Tutustu [Create React App](https://github.com/facebookincubator/create-react-app) generaattoriin ja asenna se. Jos olet kokenut kehäkettu, niin voit myös lähteä tyhjästä (avainsanat Googletusta varten ovat mm. "Webpack" ja "Babel"). Webpackiin ja Babeliin kannattaa tutustua pintapuolisesti vaikka käyttäisikin Create React Appia.
4. Tee aluksi jotain pientä Reactin kanssa ja ala sen jälkeen miettimään, mikä rooli Reactilla voisi olla omassa projektissasi.
5. Tee ensimmäinen testi, joka testaa mitä tahansa (katso alempaa vinkkejä testaamiseen). Kannattaa myös kokeilla [Travista](https://travis-ci.org/) tässä vaiheessa.
6. Julkaise sovelluksesi esim. [Firebasen](https://firebase.google.com/docs/hosting/quickstart) kautta.
   * Create React App rakentaa julkaisuvalmiin version sovelluksestasi, kun suoritat komennon `npm run build`. Komennon suorittamisen jälkeen kaikki tarvittavat tiedostot löytyvät `build` kansiosta. Suorita `npm run build` komento aina ennen kuin julkaiset sovelluksesi.
   * [Kirjaudu Firebaseen](https://console.firebase.google.com/) ja luo sinne uusi projekti.
   * Asenna Firebasen CLI: `npm install -g firebase-tools`.
   * Luo projektisi juureen `firebase.json`-tiedosto (tai lisää olemassa olevaan tiedostoon) ja lisää sinne seuraava kohta:
```json
{
  "hosting": {
    "public": "build",
    "ignore": [
      "firebase.json",
      "**/node_modules/**"
    ]
  }
}
```
   * Suorita `firebase deploy`. Joudut ehkä valitsemaan projektisi komennon yhteydessä.
   * Tämän jälkeen voit julkaista sovelluksesi milloin haluat suorittamalla komennon `npm run build && firebase deploy`.

## Homma hallussa! Mitä seuraavaksi?

Riippuu täysin projektissa, Googlettamalla löytyy vaikka mitä JavaScript maailmasta. Jos etsit valmiita kirjastoja, [npm](https://www.npmjs.com/) on paikka josta kannattaa etsiä. Tässä kuitenkin lista kirjastoja, manuaaleja ja työkaluja, joista voi olla hyötyä (:exclamation:= erityisen hyödyllinen).

* Sovelluksen tilanhallinta: [Redux](http://redux.js.org/)❗️ 
* Testaaminen: [Ava](https://github.com/avajs/ava), tai [Jest](https://facebook.github.io/jest/) testien suoritusympäristönä ja React komponenttien testaamiseen [Enzyme](https://github.com/airbnb/enzyme). Selaimen DOM-renderöinnin ja muiden ominaisuuksien simuloimiseen kannattaa käyttää [jsdom](https://github.com/tmpvar/jsdom):ia [browser-env](https://github.com/lukechilds/browser-env):in kanssa. Kun joudut luomaa stubeja, mockeja, spyita, niin [Sinon](http://sinonjs.org/) on hyvä valinta❗️   
* Hyvän koodin kirjoittaminen: [Airbnb React/JSX Style Guide](https://github.com/airbnb/javascript/tree/master/react)❗️
* Tiedon tallennus: [Firebase](https://firebase.google.com/) tai selaimen natiivi [IndexedDB](https://developer.mozilla.org/en-US/docs/Web/API/IndexedDB_API) ([Dexie](http://dexie.org/) on hyvä abkstraktio)❗️
* Mahtavia React resursseja: [Awesome React](https://github.com/enaqx/awesome-react)
* Nätit käyttöliittymät: [reactstrap](https://reactstrap.github.io/) ja [React Toolbox](http://react-toolbox.com/#/) 