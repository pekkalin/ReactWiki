## Aloitus
1. Asenna [Node.js](https://nodejs.org/en/).
2. Tutustu [Express](https://expressjs.com/) sovelluskehykseen.
3. Asenna [Express Generator](https://expressjs.com/en/starter/generator.html) ja luo projektin runko sen avulla. 
4. Tutustu Expressiin syvällisemmin ja leiki hetki sen kanssa. Ala sen jälkeen toteuttamaan jotain pientä osaa sovelluksestasi.
5. Tee ensimmäinen testi, joka testaa mitä tahansa (katso alempaa vinkkejä testaamiseen). Kannattaa myös kokeilla [Travista](https://travis-ci.org/) tässä vaiheessa.
6. Julkaise sovelluksesi esim. [Herokun](https://devcenter.heroku.com/articles/getting-started-with-nodejs#introduction) kautta. 

## Seuraavaksi

Nämä kannattaa tsekata (:exclamation:= erityisen hyödyllinen):

* Tietokanta: [Sequelize](http://sequelize.com) on hyvä ORM PostgreSQL ja MySQL tietokannoille. MongoDB:lle hyvä abkstraktio on [Mongoose](http://mongoosejs.com/)❗️ 
* Testaaminen: [Ava](https://github.com/avajs/ava), tai [Mocha](https://mochajs.org/) testien suoritusympäristönä ja oman sovelluksen API:n testaamiseen [supertest](https://github.com/visionmedia/supertest). Kun joudut luomaa stubeja, mockeja, spyita, niin [Sinon](http://sinonjs.org/) on hyvä valinta❗️   
* Hyvän koodin kirjoittaminen: [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)❗️
* Asynkronisuus tuottaa päänvaivaa?: Käytä Node.js >= v7.8.0 version [async/await](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function) toiminallisuutta [Promisen](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) kanssa. 
* Vaihtoehto Expressille: [Hapi](https://hapijs.com/).
* Reaaliaikaiset sovellukset (esim. chatit) websockettien avulla: [Socket.io](https://socket.io/).
