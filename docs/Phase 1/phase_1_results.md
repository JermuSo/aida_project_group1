# Projektisuunnitelma - Cars Data

## Tekijät: Jere Soininen, Pekka Pöyhönen, Sara Koskinen, Valtteri Pohto

## Kurssityö: AI / DA -Projekti TTC8070-3007

 ![AI/DA kurssi](aida.png)

### Tiivistelmä:
AI / DA -Projekti -kurssin työnä suunniteltiin ja toteutettiin AI / DA -moduulin aihealueeseen liittyvää data-analyysi projekti. Projektityössä analysoidaan dataa liittyen käytettyjen autojen myyntiin. Tarkoituksena on tuottaa analyysin avulla asiakkaalle lisäarvoa sen liiketoimintaan.

## 1.	Tausta ja lähtökohdat  ![Tilanne](tilanne.png)

### 1.1.	TILANNE 
Projektissa autokauppaketju on antanut toimeksiannon data-analyysistä. Tavoitteena on kehittää asiakkaan liiketoimintaa ja parantaa kilpailukykyä. Käytössä on suuri määrä dataa, jossa on monenlaisia tietoja, kuten autojen malli-, hinta- ja kokotiedot. Kattava otanta mahdollistaa syvällisen analyysin ja mallintamisen kone- tai syväoppimisen malleissa. Dataa on kuitenkin tutkittava, jaoteltava, korjattava ja jatkojalostettava, jotta sitä voidaan hyödyntää analysoinnissa ja mallintamisessa.

### 1.2.	ASIAKAS

Asiakas on Yhdysvalloissa toimiva autokauppaketju, joka keskittyy käytettyjen autojen vähittäismyyntiin Yhdysvaltojen markkinoilla. Asiakaskunta koostuu pääasiassa kotitalouksista, jotka etsivät kustannustehokkaita kuljetusvaihtoehtoja eri elämänvaiheisiin. Liiketoiminnassa korostuu asiakaslähtöinen lähestymistapa, jossa pyritään tarjoamaan kestäviä, edullisia ja laadukkaita ajoneuvoja jokaisen asiakkaan tarpeita vastaamaan.

Yrityksen ydintoiminta keskittyy käytettyjen autojen: 
- hankintaan, 
- varastointiin, 
- markkinointiin ja 
- jälleenmyyntiin. 

Käytettyjen autojen kysyntä on kasvanut Yhdysvalloissa, mikä kasvattaa markkinoiden kilpailua jatkuvasti. Yhtenä kilpailuvalttina yritys haluaa hyödyntää data-analytiikkaa liiketoimintansa kehittämisessä ja strategisten päätösten tukemisessa.   

Yritys kertoo, että keskeisinä liiketoimintahaasteina ovat varastonhallinta ja hintastrategia. Yrityksellä on suuret varastokustannukset ja tehokkaalla varaston kierrolla olisi positiivisia vaikutuksia liiketoiminnan kannattavuudelle. Nopeat myynnit ovat ensiarvoisen tärkeitä, jotta ajoneuvot eivät jää varastoon niiden arvon laskiessa.   

Käytettyjen autojen hinnat vaihtelevat suuresti riippuen esimerkiksi ajoneuvotyypin, iän, ajokilometrien, merkin ja lisäominaisuuksien mukaan. Oikean hinnan määritteleminen on haasteellista ja aikaa vievää, johon toivotaan ratkaisua data-analytiikan keinoin. 

## 2.	TAVOITTEET ![Tavoite](tavoite.png)

Projektin tavoitteena on suunnitella ja toteuttaa data-analytiikkaprojekti, jolla vastataan asiakkaan liiketoiminnan tarpeisiin. Projektin tavoitteet täytyy suhteuttaa käytettävissä olevaan aikaan. Tavoitteet voidaan jakaa seuraaviin osa-alueisiin:

### 2.1.    Liiketoiminnan tavoitteet

Projektin liiketoiminnallisisa tavoitteissa keskitytään autokauppaketjun toiminnan tehostamiseen ja kilpailukyvyn parantamiseen. Tavoitteisiin kuuluvat:
- Autojen myynnin nopeuttaminen:
    - Kasvatetaan varaston kiertonopeutta ja lyhennetään myyntiaikoja, jotta varastokustannukset pienenevät.
- Myyntihintojen optimointi:
    - Dataan perustuvan hinnoittelun kehittäminen ja sen käyttäminen päivittäisessä päätöksenteossa.
- Toiminnan kannattavuuden parantaminen:
    - Tunnistetaan keskeisiä kannattavuuteen vaikuttavia tekijöitä ja tarjotaan ratkaisuja tehokkuuden parantamiseen.


### 2.2.    Projektin etenemisen ja hallinnan tavoitteet

- Projektissa käytetään CRISP-DM-prosessimallia, joka määrittää selkeät vaiheet työn etenemiselle
- Laaditaan ja seurataan aikataulua, jotta projekti etenee maaliin suunnitellusti 7,5 viikon aikana
- Otetaan asiakas mukaan prosessiin pitämällä joka toinen viikko palaveri/katselmus työn tilanteesta
    - asiakas pääsee antamaan palautetta ja kehitysehdotuksia projektin aikana
- Tunnistetaan projektin riskit

### 2.3.	Data-analyysin ja mallintamisen tavoitteet

-	Luoda selkeä kuva käytettävästä datasta
-	Luoda integroitu, puhdistettu ja muotoiltu tietojoukko
-	Luoda koneoppimismalli numeerisilla tuloksilla ja visualisoinnilla
-	Arvioida ja tarkistaa mallin toimivuus

### 2.4.	Mallintamisen tavoitteet

-	Luodaan regressiomalli autojen myyntihinnan ennustamiseen 
    - tavoite Mean Squared Error (MAE) ~ 5-10 % auton hinnasta
    - tavoite R^2: >= 0.9
-	Luodaan luokittelumalli luokittelemaan autot nopeasti kaupaksi meneviin ja ei nopeasti kaupattaviin 
    - tavoite ROC-AUC: >= 0.9

Tavoitearvot perustuvat alustavaan analyysiin ja voivat tarkentua projektin edetessä.

### 2.5.	Projektin päättyminen

-	Data-analyysin ja mallintamisen vaiheiden jälkeen suunnitellaan ja toteutetaan käyttöönotto, seuranta ja huolto
-	Luodaan loppuraportti, kunnossapitodokumentaatio ja -suunnitelma. 
-	Projekti päätetään, kun loppuraportti ja mallintamisen aikana tuotettu malli on otettu käyttöön ja se on asiakkaan täysimääräisessä käytössä. Tuki- ja ylläpitopalvelusta sovittu erillisessä sopimuksessa.

## 3.	HAASTEET ![Haaste](haaste.png)
Projektin haasteeksi on todettu: 

-	tiukka aikataulu (7,5 viikkoa)
-	suuri ja osittain vajavainen lähtödata
-   auton lisäominaisuuksien ottaminen huomioon datan esikäsittelyvaiheessa
-   sopivien ennustemallien valinta rajallisessa ajassa
-   teknisten resurssien puute (laskentateho)


## 4.   AIKATAULU ![Aikataulu](aikataulu.png)

Projektille on annettu aikatauluksi 7,5 viikkoa alkaen 28.10.2024 ja päättyen 18.12.2024 loppuseminaariin. Alla on kuvattu suuntaa antava aikataulu. Koska käytössä on CRISP-DM, kuusivaiheinen prosessimalli dataan perustuvan projektin toteuttamiseen, voidaan odottaa iteratiivista etenemistä vaiheiden välillä.

```plantuml
@startgantt

Project starts the 2024-10-28
[Projekti aktiivinen] Starts 2024-10-28 and ends 2024-12-18
[Suunnittelu ja datan työstäminen, vaiheet 1-3 toteutus] Starts 2024-10-31 and ends 2024-12-1
[Vaiheiden 1-3 esittely (väliseminaari)] Starts 2024-12-2 and ends 2024-12-2
[Mallintaminen ja arviointi, Vaiheet 4-5 toteutus] Starts 2024-11-18 and ends 2024-12-17
[Loppuraportti, Vaihe 6 toteutus] Starts 2024-12-13 and ends 2024-12-17
[Projektien esittelytilaisuus (loppuseminaari)] Starts 2024-12-18 and ends 2024-12-18
@endgantt
```

## 5.   PROJEKTIN VAIHEET ![Vaiheet](vaiheet.png)

- [Vaihe 2](https://gitlab.labranet.jamk.fi/AC7766/aida-projekti-syksy-2024-ryhma-1/-/blob/main/docs/Phase%202/phase_2_results.ipynb?ref_type=heads) - Datan ymmärrys

- [Vaihe 3](https://gitlab.labranet.jamk.fi/AC7766/aida-projekti-syksy-2024-ryhma-1/-/blob/main/docs/Phase%203/phase_3_results.ipynb?ref_type=heads) - Esikäsittely

- [Vaihe 4](https://gitlab.labranet.jamk.fi/AC7766/aida-projekti-syksy-2024-ryhma-1/-/blob/main/docs/Phase%204/phase_4_results.ipynb?ref_type=heads) - Mallinnus

- [Vaihe 5](https://gitlab.labranet.jamk.fi/AC7766/aida-projekti-syksy-2024-ryhma-1/-/blob/main/docs/Phase%205/phase_5_results.ipynb?ref_type=heads) - Arviointi

- [Vaihe 6](https://gitlab.labranet.jamk.fi/AC7766/aida-projekti-syksy-2024-ryhma-1/-/blob/main/docs/Phase%206/phase_6_results.md?ref_type=heads) - Käyttöönotto

- [Loppuraportti](https://gitlab.labranet.jamk.fi/AC7766/aida-projekti-syksy-2024-ryhma-1/-/blob/main/docs/Phase%207%20Final%20report/final_report.md?ref_type=heads)


## 6.   TIIMI ![Tiimi](tiimi.png)

Tiimi koostuu neljästä kolmannen vuoden tieto- ja viestintätekniikan opiskelijasta, jotka kaikki suorittavat ammattiopintoina data-analytiikan ja tekoälyn opintokokonaisuutta (AI/DA-opintojaksoja) syksyllä 2024. Tiimillä on perusosaamista data-analytiikan, koneoppimisen ja tekoälyn menetelmistä sekä kokemusta datan käsittelystä ja analyysistä Python-ohjelmointikielen avulla. Tiimillä on vahva motivaatio soveltaa aiemmin oppimaansa käytännössä ja innostusta ratkaista liiketoimintaongelmia analytiikan ja koneoppimisen avulla.

### 6.1.    Roolit ja vastuut

Datan esikäsittelyssä:
-	Vastataan datan puhdistuksesta ja esikäsittelystä
-	Tehdään alkuanalyysit mitkä ominaisuudet vaikuttavat eniten auton hintaan ja myyntiaikaan.

Mallinnuksessa: 
-	Kehitetään ennustemallit hintojen ja myyntiajan arvioimiseen sekä testataan eri algoritmeja esim. regressio- ja luokittelumenetelmiä.

Visualisoinnissa:
-	Vastataan tulosten visualisoinnista selkeäksi ja informatiiviseksi asiakkaan kannalta. 
-	Toteutetaan graafeja esim. myyntinopeuksista, hinnanjakaumista ajoneuvotyypeittäin ja lisävarusteiden vaikutuksesta myyntinopeuteen ja hintaan.

Dokumentaatio ja projektin seuranta:
-	Dokumentoidaan projektin tuloksia ja tehdään suositukset asiakkaalle analyysitulosten perusteella. 
-	Seurataan, että projekti etenee suunnitellun aikataulun mukaisesti ja palautukset tulee tehtyä ajallaan

Seuraavassa taulukossa on CRISP_DM-mallin vaiheet, niiden vaiheita koskevat kuvaukset sekä projektiryhmän jäsenet, jotka ovat pääasiallisesti vastuussa kunkin vaiheen toteutuksesta.

| Vaihe    | Vaiheenkuvaus            | Vaiheen tuotos                                    | Päävastuussa                 |
|----------|--------------------------|---------------------------------------------------|------------------------------|
| Phase 1  | Business Understanding   | Projektisuunnitelma                               | Pekka, Sara                  |
| Phase 2  | Data Understanding       | Data Description Report                           | Jere, Valtteri               |
| Phase 3  | Data Preparation         | Integroitu, puhdistettu ja muotoiltu tietojoukko  | Jere, Pekka, Sara, Valtteri  |
| Phase 4  | Modeling                 | Koneoppimismallit                                 | Jere, Pekka, Sara, Valtteri  |
| Phase 5  | Evaluation               | Mallien arviointi                                 | Jere, Pekka, Sara, Valtteri  |
| Phase 6  | Deployment               | Käyttönottosuunnitelma                            | Jere, Valtteri               |
| Phase 7  | Final report             | Loppuraportti                                     | Pekka, Sara                  | 


### 6.2.    Tarvittavat työkalut ja teknologiat

Projektin toteuttamiseen käytettävät teknologiat valitaan tiimin taitojen ja asiakkaan tarpeen mukaan. Pääpaino on aiemmilla kursseilla tutuiksi tulleissa työkaluissa, jotka ovat laajasti käytössä datatieteessä yleensä. 

1. Datan ymmärtäminen ja esikäsittely:
    - __Python__ on pääasiallisena ohjelmointikielenä datan käsittelyyn, analyysiin ja mallinnukseen.
    - __Pandas ja NumPy__ ovat data-analyysin ja -käsittelyn työkalut, joilla muokataan ja esikäsitellään suurta määrää dataa tehokkaasti.

2. Koneoppiminen ja mallinnus:
    - __Scikit-learn__:ia käytetään koneoppimismallien rakentamiseen ja arviointiin. Se sisältää mm. helppokäyttöisiä regressio-, luokittelu ja klusterointialgoritmeja.
    - __TensorFlow ja Keras__  Tarjoavat alustan syväoppimismallien rakentamiseen.

3.	Visualisointi ja raportointi:
    - __Matplotlib ja Seaborn__ -kirjastoja käytetään visualisointien luomiseen ja analysointitulosten selkeyttämiseksi. 
    - __Markdown__:ia käytetään raportoinnin työkaluna

4.	Projektinhallinta ja dokumentointi:
    - __GitLab__ projektinhallintaan ja tehtävien seuraamiseen.
    - __Microsoft Office__ raportointiin ja dokumentaatioon.
    - __Teams__ yhteisiin kokouksiin ja yhteydenpitoalustana.