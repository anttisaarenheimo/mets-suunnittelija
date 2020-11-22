# metsasuunnittelija

## Summary

Forestry management adviser for all forest owners in Finland based on high quality public forest data in Finland. The forest adviser could be integrated to the existing public metsaan.fi service. Building AI course project

## Background

Suomessa on yli 600 000 metsänomistajaa, joista kullakin on omat taloudelliset, luonnonhoidolliset ja muuhun metsän käyttöön liityvät tavoittensa. Heidän ongelmansa on se, millä toimenpiteillä noihin tavoitteisiin voidaan päästä. Olen itse yksi noista metsänomistajista.

## Data sources and AI methods

Suomessa on käytettävissä maailman paras metsävaratieto, joka on myös julkisesti saatavilla. Suomen metsävarat on kartoitettu säännöllisin väliajoin laserkeilaamalla puuston tiheys ja korkeus sekä kuvaamalla latvuston peittävyys kullekin 16*16m hilaruudulle erikseen.  Kartoitun datan perusteella kullekin hilaruudulle on arvioitu puuston korkeus, järeys, tilavuus ja runkoluku puulajeittain sekä valtapuiden osalta että keskimäärin.  Lisäksi hakkuiden  suorittamisesta ja myös muista metsänhoitotoimenpiteistä tehdy ilmoitukset metsäkeskukseen ovat liitetty kuviotasolla tähän dataan. Siten metsän kasvusta ja tehdyistä hoitotoimenpiteistä on syntynyt aikasarja, jonka perusteella voidaan analysoida erilaisten toimenpiteiden vaikutus metsän kasvuun, ja sitä kautta arvioida toimenpiteiden taloudellista kannattavuutta ja myös vaikutusta muihin metsänhoidon tavoitteisiin.  Datan ja sitä kautta toimenpidesuositusten laatua voidaan parantaa metsänomistajan antamilla lisätiedoilla metsänkasvatuksen tavoitteista, laskennassa käytettävästä sisäisestä korosta, metsänhoitotoimenpiteiden ja myytävien puutavaralajien tarjoushinnoista ja niiden toteutuneista määristä.  Suomalainen metsäntutkimus on kehitettänyt hyvinkin tarkkoja yksittäisten puun kasvutapaan perustuvia malleja metsän kasvusta, josta tunnetuin ja yleisesti käytetyin on julkinen Motti.  Motin kaikki laskentaparametrit löytyvät hiladatasta, tosin niiden tarkkus jonkin verran vaihtelee.  Motin lähdekoodi on saatavilla GitHubissa. Tämän ongelma lienee ainakin alkuvaiheessa parhaiten ratkaistavissa tilastoillisin menetelmin, mutta jos tilastollisessa tarkastelussa Motin kasvuarviot poikkeavat toteutuneesta kasvusta, niin kasvusimulointiin voitaisiin mahdollisesti kokeilla myös neuroverkon käyttöä.

## How is it used?

Luontevin paikka on julkinen metsaan.fi palvelu, jossa metsänomistaja jo nyt voi tarkastella metsäkiinteistön puustoa, kirjata hoitotoimenpiteitä, ja jossa jo nyt on kuviokohtaiset metsähoitosuosituksiin perustuvat toimenpidesuositukset. Niissä ei kuitenkaan millään tavalla huomoida yksittäisten toimenpiteiden taloudellista järkevyyttä tai sen vaikutusta metsänomistajan muihin tavoitteisiin.

## Challenges

Ensimmäinen haaste on datan valtava määrä, ja erityisesti datan saavutettavuus.  Avoimessa tietokantaformaatissa oleva hiladata on ladattavissa verkosta kuntakohtaisesti, mutta syystä tai toisesta kyseistä tietokantaformaattia tukeva Windows ohjelma ei pystynyt sitä aukaisemaan. Ensimmäinen haaste olisi näiden datan yhteensopivuusongelmien ratkaiseminen.  Toinen haaste on erityisesti datan yhteismitallisuus. Koska kaukokartoitusdatan laatu on koko ajan parantunut, vanhimmat metsävaratiedot eivät ole välttämättä kovin luotettavia, ja metsikkökohtaista uutta luotettavampaa dataa tulee hitaasti: kuvaus on tarkoitus tehdä tällä vuosikymmenellä kolmen vuoden välein, ja laserkeilaus kuuden vuoden välein.  Aikaisemmin kartoitus on tehty reilun kymmenen vuoden välein ja joitain yksittäisiä alueita ei ole vielä ehditty kartoittaa lainkaan. Siten aikasarjat voivat olla riittämättömiä suurimmassa osassa maata.

## What next?

Suomi vie kaukokartoitusteknologiaa aktiivisesti ulkomaille ja hyvät analyysityökalut olisi luonteva osa sitä.

