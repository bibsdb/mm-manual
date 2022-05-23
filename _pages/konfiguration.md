---
permalink: /konfiguration
toc: true
toc_label: "Indhold på siden"
sidebar:
  title: "Vejledninger"
  nav: sidebar-sample
---



DDB CMS Manual - Konfiguration
==============================


Om vejledningen
---------------

Vejledningen beskriver de forskellige konfigurationsmuligheder i DDB CMS. Vejledninger har primært et teknisk fokus, og er rettet mod medarbejdere, som skal håndtere den tekniske opsætning/konfiguration af hjemmesiden - f.eks. som webmaster eller lignende. Hvis du primært søger vejledning til DDB CMS’ redaktionelle funktioner anbefales “DDB CMS Manualen”.

Hvis du ikke tidligere har arbejdet med DDB CMS kan det anbefales først at læse afsnittet “Sådan er DDB CMS struktureret” i “DDB CMS Manualen”, der giver en overordnet beskrivelse af sitets struktur og pointen med de forskellige strukturelle elementer.

Anvendt notation
----------------

### Notation

Nogle steder i vejledningen er der behov for at henvise til hele eller dele af URL'en.Det foregår sådan:

* Tekst i “\[ \]” indikerer, at der er forskelle alt efter hvilket biblioteks hjemmeside der henvises til.
* Ved henvisning til undersider udelades bibliotekets adresse så http://www.biblioteketsnavn.dk fjernes og det er kun den relative-URL, der er tilbage f.eks. “/stiens navn”
* Ved henvisninger til undersider, der er individuelle for hvert biblioteket indsættes \[BIBLIOTEKETS\_NAVN\] i URL'en.

### Sti til funktioner

I nogle afsnit beskrives funktioner, hvor en admin-sti er angivet i parentes, f.eks. (Sti: admin/structure/menu/manage/main-menu). Du kan bruge stien i stedet for at klikke dig frem til den pågældende funktion. Du kan enten skrive stien ind direkte efter hjemmesidenavnet (husk / efter hjemmesidenavnet): f.eks. \[\]/admin/structure/menu/manage/main-menu

Eller du kan på alle jeres sider efter sidens adresse skrive #overlay= og derefter stien: f.eks. \[\]/arrangementer#overlay=admin/config/ting/resevable

Farver og logo
--------------

### Skift logo på hjemmesiden

I øverste venstre hjørne af DDB CMS vises som udgangspunkt logoet for Danskernes Digitale Biblioteker. For at skifte logoet gør du følgende:

Fremgangsmåde:

1. Klik ind på “Udseende -> Indstillinger (ved “DDBasic (standardtema)” )“ (Sti: admin/appearance/settings/ddbasic).
2. Under afsnittet “Logo”: Fjern markering ved “Brug standard logo”.
3. Upload fil. OBS. Anbefalet højde er 44px og fleksibel bredde.
4. Tryk på knappen “Gem indstillinger”.

#### Visning af logo/biblioteksnavn på mobilvisning

Ved skærme mindre end 600px bredde vises logoet ikke. Ønskes bibliotekets navn vist i stedet, skal "Sitets navn" være slået til under Udseende> Indstilliger> DDBasic V 2.0 (Sti: admin/appearance/settings/ddbasic) og Sitets navn skal være udfyldt under Indstillinger > System > Generel information (Sti:admin/config/system/site-information).

### Skift farver på hjemmesiden

DDB CMS giver en række muligheder for at tilpasse farverne, så de f.eks. afspejler bibliotekets øvrige visuelle udtryk. Nedenfor er en præsentation af de forskellige indstillingsmuligheder.

OBS. For at ændre i farvetemaet kræver det rettigheder som “Lokal administrator”.

#### Kort om farver og tilgængelighed

Tilgængelighed handler om at give flest mulige mennesker adgang til indholdet på din hjemmeside. Med det forkerte farvevalg kan indhold og funktionalitet blive umulig at læse og bruge for borgere med forskellige former for synsnedsættelse og lignende.

Det er derfor vigtigt at overholde standarder for farvevalg, som beskrevet i en række internationale retningslinjer for tilgængelighed på nettet, der hedder WCAG 2.0 (Web Content Accessibility Guidelines 2.0). Offentlige myndigheder i Danmark er forpligtet til at overholde WCAG 2.0 på niveau A og AA.

WCAG2 specificerer bl.a. krav til kontrastforholdet mellem elementer på hjemmesiden.

På nettet findes værktøjer, som kan teste om dine farvevalg overholder WCAG2 f.eks. http://webaim.org/resources/contrastchecker/ eller http://www.dasplankton.de/portfolio-item/contrast-a/.

#### Sådan ændrer du farve på hjemmesiden

1. Klik ind på “Udseende -> Indstillinger (ved “DDBasic V2.0 (standardtema)” )“ (Sti: admin/appearance/settings/ddbasic).
2. Under sektionen “Farvevalg” vælges "Tilpasset" og farveindstillinger for de forskellige områder af hjemmesiden kan herefter indstilles.
3. Tryk på knappen “Gem indstillinger” i bunden af siden.

![](/system/rich/rich_files/rich_files/000/000/363/original/2018-03-13%2010_27_42-Udseende%20_%20%E2%80%93%20Google%20Chrome.png)

#### Gennemgang af redigeringsmulighederne

Nedenfor er en kort gennemgang af de forskellige muligheder for at justere farverne fra redigeringsgrænsefladen i DDB CMS:

* Primær
* Sekundær
* Tekst
* Text link
* Text on primary
* Text on secondary

Farvesammensætningen består af en primær og en sekundær farve samt en tekstfarve. Den primære farve benyttes blandt andet som baggrundsfarve i hovedmenuen, mens den sekundære farve benyttes til at fremhæve handlingsknapper. Man kan dog vælge, at den primære og den sekundære farve er den samme.

Tekstfarven kan defineres som en tilhørende såvel som den primære som den sekundære farve. Eftersom tekstfarven skal være læsbar, giver systemet valget i mellem sort og hvid samt den primære og den sekundære farve.

I det nye design anvendes fonten Fakt Pro. Fakt Pro er designet til skærmbrug og er baseret på elementer fra Helvetica og Futura. Der benyttes fem forskellige skriftstørrelser.

Se eksempel på skrifttype og -størrelse her: \[\[http://devdraft.server003.b14cms.dk/node/706/b14view/ab1b5590#57\]\].

Biblioteker på webmaster-løsningen kan vælge at udskifte skrifttypen.

##### Primær

“Primær” definerer baggrundsfarven for hovedmenuen, checkboxes og radioknapper.

Farven på “Primær” er som udgangspunkt støvet blå (farvekode: #4d898e).

![](/system/rich/rich_files/rich_files/000/000/364/original/2018-03-13%2010_38_26-Udseende%20_%20%E2%80%93%20Google%20Chrome.png)

##### Sekundær

Sekundærfarven bruges som baggrundsfarve for log-ind knappen, pileknapper på karruseller etc.
Farven på "Sekundær" er som udgangspunkt koralfarvet (farvekode: #f66d70)

![](/system/rich/rich_files/rich_files/000/000/365/original/2018-03-13%2010_38_41-Udseende%20_%20%E2%80%93%20Google%20Chrome.png)

##### Tekst

"Tekst" definerer farven på tekst-links og paneloverskrifter.
Vælg en farve, som er læselig på hvid baggrund.

Vælg mellem: Sort, Primær og Sekundær.
Standardfarven er sort, men ønskes farvede emneord og tekstlinks, skal denne skiftes til primær eller sekundær.

![](/system/rich/rich_files/rich_files/000/000/366/original/2018-03-13%2010_38_53-Udseende%20_%20%E2%80%93%20Google%20Chrome.png)

##### Text link

"Text link" definerer farven på tekstlinks inde i brødteksten.
Her kan vælges mellem Primær og Sekundær tekstfarve.

##### Text on primary

“Text on primary” definerer farven på tekster, der vises på baggrund af primærfarven.
Her kan vælges mellem Hvid og Sort. Standardvisningen er Hvid.

##### Text on secondary

“Text on primary” definerer farven på tekster, der vises på baggrund af sekundærfarven.
Her kan vælges mellem Hvid og Sort. Standardvisningen er Hvid.

### Indsæt et baggrundsbillede

I DDB CMS er det muligt at indsætte et baggrundsbillede for hjemmesiden. OBS. For bedst mulige resultat anbefales en billedstørrelse på 2560px1440px. Husk at komprimere billedet, for at mindske indlæsningstiden hos slutbrugerne.

Fremgangsmåde: Sådan indsætter du et baggrundsbillede på hjemmesiden

1. Klik på “Backgrounds” i genvejsmenuen. Alternativt kan du finde “Backgrounds” under (Sti: admin/config/user-interface/backgrounds)
2. Klik på “Vælg fil” og find det billede, du ønsker at bruge.
3. Ud for “Background image 1” sætter du flueben ud for “Use picture as the site's default background”.
4. Klik på knappen “Gem indstillinger”.
5. Hvis billedet ikke vises, skal du rydde cachen. Klik på “Ryd alle cacher” under Indstillinger -> Ydelser (Sti: admin/config/development/performance).

### Skift favicon/genvejsikon for hjemmesiden

Som udgangspunkt anvendes drupals standardlogo som favicon/genvejsikon: ![](/system/rich/rich_files/rich_files/000/000/395/original/drupal.png)

Det er muligt at skifte ikonet på følgende måde:

1. Åben “Udseende -> Indstillinger (under DDBasic V 2.0 (standardtema)) -> Indstillinger for genvejsikon (fane nederst på siden)” (Sti: admin/appearance/settings/ddbasic).
2. Fjern fluebenet i checkboksen “Brug standard genvejsikonet”.
3. Upload ikon eller indsæt sti til det billede du ønsker at anvende.
4. Klik på knappen “Gem indstillinger”.

Overlay
-------

Det er muligt at slå overlay fra og til på følgende elementer på sitet: Ting object/forsidekarrusel, nyheder, grupper/temasider (visning på forsiden), tabroll. Som standard er overlay slået til på alle elementerne. Konfigurationen findes under: /admin/appearance/settings/ddbasic

### Disable Ting Object Overlay (Forsidekarrusel)

Det er muligt at fjerne den grå gradient med tekst, som lægger sig hen over materialeforsiderne i diverse karruseller. Dette gøres ved at sætte flueben i Disable overlay ud for Disable TING OBJECT OVERLAY under /admin/appearance/settings/ddbasic. Klik herefter på "Gem"; husk at cleare cashe. Overlayet bliver vist som standard.

MED overlay:

![](/system/rich/rich_files/rich_files/000/001/234/original/Sk%C3%A6rmbillede%202020-02-18%20kl.%2014.19.43.png)

UDEN overlay:

![](/system/rich/rich_files/rich_files/000/001/233/original/Sk%C3%A6rmbillede%202020-02-18%20kl.%2014.21.33.png)

### Disable DING NEWS OVERLAY

Det er muligt at fjerne den grå gradient med tekst, som lægger sig hen over nyheder (visningen på forsiden samt visning i nyhedsoversigten) Dette gøres ved at sætte flueben i Disable overlay ud for Disable DING NEWS OVERLAY under /admin/appearance/settings/ddbasic. Klik herefter på "Gem"; husk at cleare cashe. Overlayet bliver vist som standard.

Nyheder MED overlay:
![](/system/rich/rich_files/rich_files/000/001/235/original/Sk%C3%A6rmbillede%202020-02-18%20kl.%2014.25.42.png)

### Nyheder UDEN overlay:

![](/system/rich/rich_files/rich_files/000/001/237/original/Sk%C3%A6rmbillede%202020-02-18%20kl.%2014.27.53.png)

Disable DING GROUP OVERLAY

Det er muligt at fjerne den grå gradient med tekst, som lægger sig hen over temasider (grupper) der vises på forsiden. Dette gøres ved at sætte flueben i Disable overlay ud for Disable DING GROUP OVERLAY under /admin/appearance/settings/ddbasic. Klik herefter på "Gem"; husk at cleare cashe. Overlayet bliver vist som standard.

Temasider MED overlay:

![](/system/rich/rich_files/rich_files/000/001/238/original/Sk%C3%A6rmbillede%202020-02-18%20kl.%2014.40.57.png)

Temasider UDEN overlay:

![](/system/rich/rich_files/rich_files/000/001/240/original/Sk%C3%A6rmbillede%202020-02-18%20kl.%2014.44.17.png)

###

Disable DING TABROLL OVERLAY 

Det er muligt at fjerne den grå gradient med tekst, som lægger sig hen over elementer i tabroll´en. Dette gøres ved at sætte flueben i Disable overlay ud for Disable DING TABROLL OVERLAY under /admin/appearance/settings/ddbasic. Klik herefter på "Gem"; husk at cleare cashe. Overlayet bliver vist som standard.

Tabroll MED overlay:

![](/system/rich/rich_files/rich_files/000/001/242/original/Sk%C3%A6rmbillede%202020-02-18%20kl.%2014.45.35.png)

Tabroll UDEN overlay:
![](/system/rich/rich_files/rich_files/000/001/241/original/Sk%C3%A6rmbillede%202020-02-18%20kl.%2014.48.04.png)

Personalisering
---------------

### Min liste / Huskeliste

Kendte slutbrugerne kan tilføje materialer til en personlig huskeliste. Huskelisten opbevares i en national service, "Material List". På værk- og materialevisningssider vises knappen "Tilføj til huskeliste". Klikker brugeren herpå tilføjes materialet til huskelisten. Senest tilføjede materiale ligger øverst på listen. Tilføjer bruger samme materiale til huskelisten to eller flere gange, ligger materialet kun én gang på listen. Bruger kan slette materialer enkeltvis igen fra Huskelisten.

Brugen af Følg søgning forudsætter konfiguration af integrationen til Adgangsplatformen, Material List servicen og Brøndprofilen.

#### Adgangsplatformen (/admin/config/ding/adgangsplatformen)

* Tilbagekald access token: https://login.bib.dk/oauth/revoke
* Tokenclient
  * Client ID: \*\*\*\*\* (NB. Må ikke deles)
  * Client secret: \*\*\*\*\* (NB. Må ikke deles)

NB. Det er muligt at se om en låner er autentificeret mode Adgangsplatformen ved at logge ind og åbne /ding\_react/user.js så man får vist:

window.ddbReact = window.ddbReact || {};
window.ddbReact.userAuthenticated = true;
window.ddbReact.setToken('\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*');

#### Material List servicen (/admin/config/ding/react)

* Services
  * Material List servicen: https://prod.materiallist.dandigbib.org
* Migrering
  * Timeout for migrering af lister: 5

#### Brøndprofilen (/admin/config/ding/provider/opensearch)

Brøndprofilen skal være sat til "opac".

Det kan tjekkes ved at åbne /ding/variables og se efter elementet "opensearch\_search\_profile".

Brøndprofilen konfigureres under /admin/config/ding/provider/opensearch

### Følg søgning

Kendte slutbrugere kan gemme søgninger i en personlig liste, "Søgninger jeg følger". "Søgninger jeg følger" opbevares i en national service, "Follow Searches". Når bruger har lavet en søgning, vises en stjerne yderst th i søgefeltet. Klikker bruger herpå, kan bruger give sin søgning en titel, og gemme. Senest gemte søgning ligger øverst på listen. Bruger kan slette gemte søgninger enkeltvis igen fra listen. Bruger kan se sin gemte søgning ved at klikke på "Vis søgeresultat"; søgningen vises sorteret med nyeste udgivelsesår først.

Brugen af Følg søgning forudsætter konfiguration af integrationen til Adgangsplatformen og Follow Searches servicen.

Konfiguration af adgangsplatformen (/admin/config/ding/adgangsplatformen)

* Tilbagekald access token: https://login.bib.dk/oauth/revoke
* Tokenclient
  * Client ID: \*\*\*\*\* (NB. Må ikke deles)
  * Client secret: \*\*\*\*\* (NB. Må ikke deles)

Follow Searches servicen (/admin/config/ding/react)

* Services
  * Follow Searches servicen: https://prod.followsearches.dandigbib.org
* Migrering
  * Timeout for migrering af lister: 5

### Migrering af lister og gemte søgninger

Fra og med DDB CMS release 31-1 migreres alle brugernes personlige lister fra OpenList over i den nye Materiael List, og alle lister slås sammen til én liste som er Huskelisten. Tidligere delte og/eller offentliggjorte lister gøres private igen, og kan således fremadrettet kun tilgås af pågældende bruger, der oprindeligt har oprettet listen. Endvidere migreres alle brugernes "Søgninger jeg følger" samt "Forfattere jeg følger" fra OpenList over i den nye Follow Searches, og samles i én oversigt "Søgninger jeg følger".  I forbindelse hermed tildeles brugerne et nyt entydigt brugerid (GUID). 

Dermed kan brugerne (på sigt):

* se deres personlige huskeliste samt søgninger de følger på andre brugergrænseflader (f.eks. Biblioteket app´en)
* se deres personlige huskeliste samt søgninger de følger på tværs af biblioteker
* se deres personlige huskeliste samt søgninger de følger på netbiblioteket (f.eks. eReolen)

Migreringen sker automatisk i det øjeblik en bruger logger ind på hjemmesiden, efter biblioteket har opgraderet til release 31-1.

Placering af indhold på forsiden og sektioner
----------------------------------------------

### Forfremmelse af indhold til forsiden

Under "Indstillinger -> Ding -> Promote content types to front page" (/admin/config/ding/fe-promote) kan det vælges at alle nyheder eller arrangementer som standard forfremmes til forsiden. Ved oprettelse af et nyt arrangement/nyhed kan dette fravælges for det enkelte indholdselement under "Udgivelse". Det er altså ikke længere nødvendigt for redaktører at få en administrator til at forefremme deres indhold, såfremt administrator én gang har valgt at indholdstypen er forfremmet som standard.

### **Oprettelse af sektioner**

* [Se hvordan du opretter en sektion her](https://platform.dandigbib.org/projects/ddb-cms/wiki/Ddb-cms-manual_struktur-og-indhold#Opret-en-sektion).

### Panels in place forudsætninger

Panels in Place giver brugeren mulighed for at flytte de enkelte moduler op og ned på forsiden.

* Rolle: For at bruge Panels skal man være logget ind som lokaladmin

### Hvordan placerer man et nyt element på forsiden eller sektioner?

* Log ind
* Klik på “Rediger denne side” nederst på forsiden eller sektionen.

![](/system/rich/rich_files/rich_files/000/000/004/original/panels_dump1.png)

Siden er nu opdelt i placeholders i fuld bredde placeret under hinanden.

![](/system/rich/rich_files/rich_files/000/000/003/original/panels_dump2.png)

* Klik på “tilføj”-knappen og vælg det modul, du ønsker at placere på forsiden.

### Opsætning af de enkelte moduler

#### 1) Tab-roll (“Ting frontpage tab-roll”)

1\. Gå til forsiden eller en sektionsforside. Tryk på ’Rediger denne side’ i bunden.

![](/system/rich/rich_files/rich_files/000/000/741/original/2rediger.jpg)

2\. Tryk på ’Add’.

![](/system/rich/rich_files/rich_files/000/000/742/original/3add.jpg)

3\. Tryk på "Ding frontpage tabroll’’ i dropdown.
![](/system/rich/rich_files/rich_files/000/000/918/original/Ding%20tabroll.JPG)

4\. Vælg om tabrollens titel skal vises, vælg hastighed, klik "Afslut", og klik "Gem"
BEMÆRK: Der kan kun være én tabroll på sitet.

#### 2) Forsidekarruseller

Læs om forsidekarruseller i ["DDB CMS Manual - Struktur og indhold"](https://platform.dandigbib.org/projects/ddb-cms/wiki/Ddb-cms-manual_struktur-og-indhold_next-version#Forsidekarruseller)

#### 3) Temasider (“View: Ding Group temapages”)

* Vælg evt. ny titel
* Klik afslut Note: For at indholdet skal vises i karussellen kræves det, at tab-rollen er udgivet.

#### 4) Sektioner

Man kan vise udvalge sektioner på forsiden, på samme måde som de gamle temasider.
Vælg "Section Group"
 ![](/system/rich/rich_files/rich_files/000/001/669/original/section%20group.png)

Navngiv din sektion.

I det tomme felt "Selected section" skriver man titlen på den sektion, men gerne vil vise på forsiden. Systemet foreslår selv de mulige, når du begynder at skrive (type ahead)
Klik på titlen på den sektion, der skal vises på forsiden
![](/system/rich/rich_files/rich_files/000/001/545/original/Sk%C3%A6rmbillede%202020-12-18%20kl.%2016.38.32.png)

Vælg den pågældende sektion ved at klikke på en af de titler, systemet foreslår![](/system/rich/rich_files/rich_files/000/001/546/original/Sk%C3%A6rmbillede%202020-12-18%20kl.%2016.38.53.png)

Klik på "Add content" for at tilføje en sektion mere
Klik på "Afslut" / "Finish" for  at gemme

#### 5) Kampagner (“Relevant campaigns”)

Vælg evt. ny titel

Vælg antal kampagner på forsiden under “Campaign Count”

Klik afslut

![](/system/rich/rich_files/rich_files/000/000/013/original/panels_dump11.png)

Note: Hvilke kampagner der skal vises på forsiden, bestemmes i opsætningen af den enkelte kampagne. Under “campaign rules” vælges typen: path med værdien:

![](/system/rich/rich_files/rich_files/000/000/015/original/panels_dump12.png)

#### 6) Nyheder (“View: Ding news: news list frontpage”) (\*)

* Vælg evt. ny titel
* Klik afslut Note: For at indholdet skal vises i karussellen skal det være udgivet og forfremmet til forsiden

#### 7) Begivenheder (“View: Ding events: events list frontpage”) (\*)

* Vælg evt. ny titel
* Klik afslut Note: For at indholdet skal vises i karussellen skal det være udgivet og forfremmet til forsiden

(\*) BEMÆRK! Elementtyperne “Ding news: news list frontpage” og ”Ding events: events list frontpage” forventes afløst af elementtypen ”Nodelist”. Derfor er det ikke muligt at tilføje disse elementtyper – men da alle DDB CMS-sites fra fødslen er spundet med disse elementer på forsiden, vil de stadig findes mange steder. Men hvis man først sletter dem, er det ikke muligt at få dem tilbage. Dog vil man vha ”Nodelist” kunne skabe elementer med samme funktioner.

#### 8) Åbningstider (“all openings hours”)

Note: Indholdet redigeres i indholdstypen bibliotek

#### 9) Nodelist

##### **Tilføj nodelist**

1. Klik på "Rediger denne side"
2. Tilføj (”add”) et panel i ”panels in place” (hvis menuen dækker over valgmulighederne, kan du trykke add længere nede på siden under fx secondary content).
3. Vælg ”nodelist” i oversigten over moduler
   * Nodelisten er sat til at kunne indeholde både nyheder, arrangementer og sider.
   * For at opnå det bedste resultat anbefales det ikke at blande indholdstyperne, men oprette særskilte nodelister for nyheder, arrangementer og sider.
4. Giv nodelisten en titel
5. Under ”List type” vælges, hvordan artiklernes listebillede skal vises.
   * "Carousel" viser indhold lidt som tabroll på forsiden, men med pile til at bladre mellem indholdet.
   * "Rolltab" viser indhold ligesom tabroll på forsiden
   * ”Promoted nodes” viser billeder i 3 kolonner med skiftevis stort og medium forsidebillede.
   * ”Nodes in blocks” viser artiklerne i 3 kolonner
6. Vælg indhold
   * Alt indhold. Som udgangspunkt vises alt publiceret indhold (”all content”) begrænset til max 4 artikler (”item limit”). I dropdownen kan man vælge at vise op til 100 artikler.
   * Sættes flueben ved ”show upcoming events only” vises kun fremtidige arrangementer
   * ![](/system/rich/rich_files/rich_files/000/000/750/original/01content.jpg)

##### **Indhold i nodelist**

1. Tilpasset indhold (custom)
   * Ønsker man at bestemme præcis hvilke artikler der skal vises i nodelisten, klik på ”custom content” (tilpasset indhold).
   * Under ”selected content” søger man de enkelte artikler frem.
   * Artiklerne skal være publiceret for at kunne blive fremsøgt under ”selected content”
   * ![](/system/rich/rich_files/rich_files/000/000/751/original/02custom.png)
   * Klik på ”Add content” Man kan tilføje lige som mange individuelle artikler, som man ønsker.
2. Dynamisk indhold
   * Ønsker man at filtre de viste artikler udfra taxonomier, klik på ”dynamic content”.
   * Den dynamiske filtrering fungerer bedst hvis man ikke kombinere de enkelte indholdstyper (nyheder, arrangementer, sider)
   * Dynamisk indhold og tilpasset indhold (custom) kan kombineres i samme nodeliste
3. Dynamiske nyheder
   * I feltet ”field” vælger man hvilket parameter, nyhederne kan filtreres efter:
   * Kategorier (”category”), tilknyttede emneord (”tags”) eller bibliotek (”library”). Det er også muligt at filtre indholdet efter temaer (”groups”)
     Man  kan oprette lige så mange filtre, man ønsker.
   * ![](/system/rich/rich_files/rich_files/000/000/752/original/03dynamisknyhed.png)
   * Et eksempel på en nodeliste, som filtrerer nyheder efter kategori (anbefalinger), tag (børnelitteratur) og bibliotek (lokalbibliotek):
   * ![](/system/rich/rich_files/rich_files/000/000/753/original/04eksnyhed.png)
4. Dynamiske arrangementer
   * I feltet ”field” vælger man hvilket parameter, arrangementer kan filtreres efter:
   * Arrangementskategorier (”category”), tilknyttede emneord (”tags”), målgrupper (”target”) eller bibliotek (”library”). Det er også muligt at filtre indholdet efter arrangør (”organizer”) og temaer (”groups”)
   * Et eksempel på en nodeliste som kombinerer arrangementer med målgruppen (for børn) og tilpasset indhold (arrangementet: mød forfatteren: Elisabeth Egholm):
   * ![](/system/rich/rich_files/rich_files/000/000/754/original/05dynamiskarr.png)
5. Dynamiske sider
   * I feltet ”field” vælger man hvilket parameter, sider kan filtreres efter: Tags, bibliotek og temaer (”groups”)
   * Et eksempel på en nodeliste med sider som kombinerer tilpasset indhold (om at bruge lister) med sider, som er tagget med ”kager”
   * ![](/system/rich/rich_files/rich_files/000/000/755/original/06dynasider.png)

##### **Sortering af indhold**

1. Sortering af indhold
   * Indholdet i nodelisten kan sorteres efter oprettelsesdato, titel og om indholdet er sat til at være klæbrigt på forsiden.
   * Under additional links kan man linke til eksterne eller interne sider eller til andre sektionsforsider. Linkes skal indholde både tekst og link
   * ![](/system/rich/rich_files/rich_files/000/000/756/original/07sotering.png)

##### **Gem og afslut**

1. Gem nodelisten.
   * Når opsætningen af nodelisten er færdig klik på ”finish)
   * ![](/system/rich/rich_files/rich_files/000/000/757/original/08gem.png)
   * Til slut klikkes på ”save” for at gemme ændringerne i hele panels in place
   * ![](/system/rich/rich_files/rich_files/000/000/758/original/09save.png)

### Flytning af modulerne

* Log ind som lokaladmin
* Klik på “Rediger denne side”
* Klik på ikonet yderst til højre

![](/system/rich/rich_files/rich_files/000/000/014/original/panels_dump13.png)

* Hold musetasten nede og bevæg ikonet op eller ned
* Når modulet forlader sin oprindelige plads vises en horisontal gul stribe

![](/system/rich/rich_files/rich_files/000/000/016/original/panels_dump14.png)

* Bevæg musen op eller ned indtil der igen viser sig en gul stribe
* Slip musen

![](/system/rich/rich_files/rich_files/000/000/017/original/panels_dump15.png)

* Klik på “gem” hver gang et modul flyttes

### Åbningstider

På forsiden kan der være to veje til åbningstiderne - den ene er et bredt panel, som vises under sidens indhold, og den anden er egentlig to veje til samme indhold, nemlig enten linket til Biblioteker i hovedmenuen eller knappen Åbningstider øverst til højre på siden.

![](/system/rich/rich_files/rich_files/000/000/034/original/opening-hours_dump4.PNG)

![](/system/rich/rich_files/rich_files/000/000/031/original/opening-hours_dump2.PNG)

Knappen kan deaktiveres eller aktiveres under Struktur -> Menuer -> Topbar menu, hvor hakket under Aktiveret fjernes i rækken med Opening hours.

![](/system/rich/rich_files/rich_files/000/000/033/original/opening-hours_dump3.PNG)

For at få vist åbningstider på forsiden i vandret panel, skal man under Indstillinger -> Ding -> Ding DDBasic opening hours sætte hak i boksen "Show opening hours on frontpage".

![](/system/rich/rich_files/rich_files/000/000/032/original/opening-hours_dump1.PNG)

Kontaktinformation
------------------

### Adresseoplysninger i footeren/sidefoden

I footeren er det muligt at indsætte adresseoplysninger. For at ændre adresseoplysninger forudsættes at din bruger har administratorrettigheder.

**Fremgangsmåde: Ændre adresseoplysninger i footeren.**

1. Gå til “Struktur -> Blokke -> Footer adresse (klik på “indstil” yderst til højre) (Sti: admin/structure/block/manage/block/1/configure).
2. I feltet “Indhold” indtastes den ønskede adresse.
3. Tryk på knappen “Gem blok” nederst på siden.

### Kontaktformular

DDB CMS tilbyder som udgangspunkt en kontaktformular, der findes på (Sti: https://bibliotekets-hjemmesideadresse.dk/contact). Kontaktformularen indeholder fem hovedfelter:

* Navn
* Din e-mail-adresse
* Emne
* Meddelelse
* Kategori: Dropdown-feltet “kategori” indeholder kategorier til præcisering af formålet med henvendelsen f.eks. “Aflevering” og “Fornyelse af materiale”. Det er muligt at redigere og tilføje kategorier på følgende måde:

Fremgangsmåde: Tilføj kategori:

1. Åbn “Struktur -> Kontaktformular” (Sti: https://bibliotekets-hjemmesideadresse.dk/admin/structure/contact)
2. Klik på “+ Tilføj kategori” i toppen af siden.
3. Udfyld de forskellige relevante felter f.eks. navngiv kategorien, udfyld modtageradresse og skriv evt. autosvar, der sendes når henvendelser modtages på den specifikke kategori.
4. Klik på knappen “Gem”.
5. Tjek at kategorien er tilgængelig i dropdown-menuen “Kategori” på kontaktformularen (Sti: https://bibliotekets-hjemmesideadresse.dk/contact).

Mellem besked-feltet og knappen "Send besked" findes en tekst, der linker til bibliotekets persondatapolitik med stien /persondata
**OBS!** Det er vigtigt, at i via [oversættelsesmodulet](https://platform.dandigbib.org/projects/ddb-cms/wiki/Ddb-cms-manual_konfiguration#Overs%C3%A6t-tekst-i-gr%C3%A6nsefladen) finder teksten og retter linket til at pege på jeres side om behandling af persondata.

Webforms / webformularer
------------------------

Webformularer kan oprettes på 2 måder:
a) Sammen med indholdstyperne nyheder, arrangementer og sider
b) Som en selvstændig indholdstype
For begge typer gælder det, at alle henvendelser automatisk slettes efter en periode, der som default er 6 måneder.
Ønskes denne periode ændret, kan det gøres under /admin/config/webform\_purge/manage under "Days to retain":
![](/system/rich/rich_files/rich_files/000/001/670/original/Days%20to%20retain.jpg)

Endvidere gælder det for alle webforms, at der som default er slået en såkaldt "progress bar" til, som ser sådan her ud:

![](/system/rich/rich_files/rich_files/000/001/716/original/1%20start%202%20complete.jpg)

Ønskes denne fjernet, skal man gå ind under /admin/config/content/webform og fjerne fluebenet i "Show progress bar" under "Progress bar".

Dermed fjernes den fra alle webforms.

![](/system/rich/rich_files/rich_files/000/001/717/original/Show%20progress%20bar.jpg)

### Webformularer tilknyttet en nyhed, event eller statisk side

Opret en Nyhed
Gem nyheden
Klik på rediger
Vælg fanebladet Webform

![](/system/rich/rich_files/rich_files/000/000/035/original/webforms_dump1.png)

![](/system/rich/rich_files/rich_files/000/000/036/original/webforms_dump2.png)

#### Form Components

Opret elementer i formularen
Tilføj navn på feltet, vælg type (tekstfelt, tekstområde, e-mail, dropdown osv.)
Sæt flueben hvis feltet skal udfyldes af brugeren
Klik tilføj

![](/system/rich/rich_files/rich_files/000/000/037/original/webforms_dump3.png)

Skal der ikke opstilles særlige betingelser for dette felt, klik “save component”.

![](/system/rich/rich_files/rich_files/000/000/038/original/webforms_dump4.png)

Tilføjer man et e-mail-felt til formularen er det vigtigt at sætte flueben ved valideringen af den afsendt mailadresse

![](/system/rich/rich_files/rich_files/000/000/039/original/webforms_dump5.png)

Ønsker man et drop down felt vælges typen “Select options”.

![](/system/rich/rich_files/rich_files/000/000/040/original/webforms_dump6.png)

Tilføj en titel på feltet og skriv de enkelte valgmuligheder brugeren skal præsenteres for.
Afslut med “save component”

![](/system/rich/rich_files/rich_files/000/000/041/original/webforms_dump7.png)

Oversigt over formular med titel, type, obligatoriske- og valgfri felter

![](/system/rich/rich_files/rich_files/000/000/042/original/webforms_dump8.png)

#### Conditionals

I fanebladet “Conditionals” kan du opsætte betingelser for, hvordan input i ét af felter, kan påvirke visningen af andre felter i formularen

![](/system/rich/rich_files/rich_files/000/000/043/original/webforms_dump9.png)

Et eksempel - hvis emnefeltet ikke indeholder Borgerservice, vil e-mail feltet ikke blive vist for brugeren.

![](/system/rich/rich_files/rich_files/000/000/044/original/webforms_dump10.png)

#### E-mails

Under fanebladet E-mails vælges modtageren af webformularen.

![](/system/rich/rich_files/rich_files/000/000/045/original/webforms_dump11.png)

![](/system/rich/rich_files/rich_files/000/000/046/original/webforms_dump12.png)

##### Sådan sendes indholdsfelter fra formularen til e-mail-adressen

På grund af GDPR sendes indholdet af formularen som default ikke til denne e-mail-adresse der er angivet da forbindelsen ikke er krypteret.
Hvis det vurderes at indholdet ikke kommer til at indeholde personfølsomme oplysninger kan udvalgte felter i formularen sendes med e-mailen ved at vælge e-mail-templaten "Custom template".

Sådan gør du:

1. Åben "Form components" fanebladet.
2. Tryk på "Redigér" ud for det felt i formularen du ønsker at medtage i e-mailen.
3. Kopier værdien af feltet "Field key" fx "e\_mail\_adresse" fra eksemplet herunder.
   ![](/system/rich/rich_files/rich_files/000/001/543/original/2020-12-18%2009_15_41-Window.png)
4. Åben "E-mails" fanebladet.
5. Udfyld den e-mail-adresse formularen skal sende til og tryk på "Tilføj" knappen.
   ![](/system/rich/rich_files/rich_files/000/001/544/original/2020-12-18%2009_16_38-Window.png)
6. Scroll ned til "E-MAIL-TEMPLATE"
7. Vælg "Custom template"
8. Skriv følgende i e-mail-skabelonen hvor "e\_mail\_adresse" i dette tilfælde er den field key du kopierede fra fra "Form components" under der felt du vil medtage i e-mailen:
   \[submission:values:e\_mail\_adresse\]

Gentag for de øvrige felter du ønsker e-mailen skal indeholde.

#### Form settings

![](/system/rich/rich_files/rich_files/000/000/047/original/webforms_dump13.png)

Under Form settings kan man komponere en tekst der bekræfter modtagelsen af formularen. Det kan enten være ren tekst eller ved at redirecte brugeren til en anden side

![](/system/rich/rich_files/rich_files/000/000/048/original/webforms_dump14.png)

Under Form settings kan man også begrænse antallet af formularer, som den enkelte bruger kan sende.

![](/system/rich/rich_files/rich_files/000/000/049/original/webforms_dump15.png)

#### Afslutning opsætningen og visning af formular

Klik på “gem indstillinger”, når opsætningen af formularen er afsluttet
Klik på vis for at se, hvordan nyheden og den tilknyttede formular ser ud

![](/system/rich/rich_files/rich_files/000/000/050/original/webforms_dump16.png)

#### Statistik

Under fanebladet Resultater finder man statistik over inputtet fra formularen

![](/system/rich/rich_files/rich_files/000/000/051/original/webforms_dump17.png)

### Webformularer som en selvstændig indholdstype

Klik på tilføj indhold
Vælg Webform
Skriv Titel
Sæt flueben ved Tilbyder et menu-link, hvis formularen skal forankres i menustrukturen (hovedmenu eller sekundær menu)
Klik på Gem

![](/system/rich/rich_files/rich_files/000/000/052/original/webforms_dump18.png)

Fortsæt opsætningen af formularer i afsnittet link til pkt. a)

Adgangsplatformen - Log ind og Single Sign-on
---------------------------------------------

Adgangsplatformen:

1. Betyder et ensartet log ind flow på tværs af bibliotekernes brugergrænseflader, hvor brugerne når de trykker på "Log ind" knappen bliver sendt til en selvstændig loginside - sådan som de kender det fra NemLog-in.
2. Single Sign-on så brugerne kan hoppe imellem to bibliotekstjenester, f.eks. fra DDB CMS til Filmstriben, uden at skulle logge ind igen.

### Konfiguration af integrationen til Adgangsplatformen

**Forudsætninger**:

1. Aktivering af "ding\_adgangsplatformen" modulet.
   1. Redaktørbiblioteker får automatisk modulet Adgangsplatformen aktiveret under opgradering.
   2. Webmaster- og Programmørbiblioteker skal selv aktivere modulet under /admin/modules.
2. Client ID og Client secret
   1. Redaktørbiblioteker får automatisk konfigureret modulet Adgangsplatformen med deres Client ID og Client secret på staging- og produktionsmiljøerne.
   2. Webmasterbiblioteker får automatisk konfigureret modulet Adgangsplatformen med deres Client ID og Client secret på produktionsmiljøerne samt når de opgraderer på development- og stagingmiljøerne.
   3. Programmørbiblioteker skal kontakte https://kundeservice.dbc.dk og bede om at få oprettet deres Client ID og Client secret til konfiguration af modulet Adgangsplatformen.
3. Biblioteker der benytter pin-koder på mere end 4 cifre skal oplyse det til DBC.

**Sådan konfigureres integrationen til Adgangsplatformen**

1. Åben /admin/config/ding/adgangsplatformen.
2. Kopier det Client ID du har modtaget via https://kundeservice.dbc.dk og indsæt det i "Client ID" feltet.
3. Kopier den Client secret du har modtaget via https://kundeservice.dbc.dk og indsæt den i "Client secret" feltet.
4. Tryk på "Save configuration" knappen.

![](/system/rich/rich_files/rich_files/000/001/093/original/Adgangsplatformen_konfiguration.png)

### Verifikation af låner autentifikation

Når en låner er logget ind er det muligt at verificere dennes autentifikation og se låneren token under /ding\_react/user.js.

Token benyttes blandt andet for integration med Openplatform i React komponenterne.

Bibliotekssystemet FBS
----------------------

### Slet inaktive providerbrugere

Åben “Indstillinger -> Ding -> Ding provider” (Sti: /admin/config/ding/provider)

Nederst på siden vises følgende valgmuligheder:

![](/system/rich/rich_files/rich_files/000/000/229/original/2017-11-28%2010_27_45-Ding%20provider%20_%20%E2%80%93%20Google%20Chrome.png)

### "Opret bruger"

"Opret bruger" giver mulighed for at en bruger kan oprette en brugerprofil uden at skulle møde op på det lokale folkebibliotek. Dermed kan man også oprette sig som bruger udenfor bibliotekets åbningstid og få adgang til licensbelagte e-ressourcer mv.

Funktionerne findes ved at trykke på fanebladet "Log ind", hvor de vises lige under  "Ny bruger?" vises til højre for "Log ind-knappen".![](http://platform.dandigbib.org/attachments/download/2733/NemID.png)

"Opret bruger" forudsætter:

1. aktivering af moduler og konfiguration af DDB CMS.
2. opkobling til Serviceplatformen for automatisk tildeling af lånerkategori

#### Aktivering af "Opret bruger":

1. Redaktørbiblioteker: Opret en sag hos DBC kundeservice: https://kundeservice.dbc.dk/ og bed om aktivering af "Ding gatewayf" modulet for "Opret bruger med NemID".
2. Webmaster og programmørbiblioteker: Aktivér modulet “Ding gatewayf” under /admin/modules.
   1. Sørg endvidere for at deaktivere modulet “Ding Wayf” (modulet skal ikke længere anvendes)

**Redaktørbiblioteker** kan tage de nye funktioner i brug, når DBC giver besked om at modulerne er aktiveret og konfigureret.

**Webmaster- og Programmørbiblioteke**r skal selv:

1. aktivere modulerne og konfigurere dem, når de får besked af DBC om at superpinkoden er indsat: Aktivér modulet “Ding gatewayf” under /admin/modules.
2. Sørg endvidere for at deaktivere modulet “Ding Wayf” (modulet skal ikke længere anvendes).

Konfiguration af "Opret bruger": se fremgangsmåden herunder.

#### Konfigurering af ”Opret bruger”

Forudsætter at processen under "Aktivering for FBS biblioteker" er gennemført.

1. Aktivér modulet “Ding gatewayf registration” under /admin/modules. Vær opmærksom på at “Ding gatewayf registration" kræver at “Ding gatewayf” er aktiveret.
2. Åbn “Indstillinger -> Adgangsplatform -> Registration" (Under afsnittet “DING”)“ (Sti: /admin/config/ding/adgangsplatformen/registration).
3. Feltet "Age limit" under "NY BRUGER - NEMID" er som standard udfyldt med "18". Denne indstilling bør som udgangspunkt ikke ændres. (Unge i alderen 15-17 år kan godt have en NemiD, men når man er under 18 år er man ikke myndig, og oprettelsesflowet understøtter ikke at forældre/værge først skal godkende en brugeroprettelse for deres umyndig(e) barn/børn)
4. Sektionen "INFORMATION PAGE" indeholder den tekst, der vises til brugeren, når han/hun klikker på "Opret bruger via NemID.
   NB. Der er tale om den default tekst som skal tilpasses så den passer til lokale forhold.
5. Indsæt SELV et link i teksten til den side på sitet, der indeholder bibliotekets reglement.
6. Sektionen "ACCEPTANCE PAGE" indeholder den tekst, der vises til brugeren ud for "Acceptér" checkboksen i oprettelsesforløbet. Som standard er det: _Jeg accepterer bibliotekets reglement_
7. Sektionen "SUCCESSFUL REGISTRATION PAGE" indeholder den tekst, der vises til brugeren når han/hun er oprettet. Som standard er det: _Du er nu oprettet som bruger._
8. Test at “Opret bruger” fungerer på sitet.

### Rediger tekst i grænsefladen “Gebyr for SMS”

Lånerprofilen i DDB CMS indeholder et felt, hvor det er muligt at indtaste et mobilnummer, som bl.a. kan bruges til at sende låneren SMS notifikationer ang. materiale til afhentning og lignende. Under feltet vises der som udgangspunkt følgende hjælpetekst: “Vær opmærksom på, at der er et gebyr på SMS”. Det er muligt at redigere eller helt fjerne teksten. Sidstnævnte er naturligvis relevant, hvis man ikke har gebyr for SMS-notifikationer.

Sådan gør du:

1. Åbn “Indstillinger -> Kontoindstillinger” (Sti: admin/config/people/accounts)
2. Rediger teksten (evt. fjern teksten helt) i feltet “Fee for SMS”.
3. Klik på knappen “Gem indstillinger”.

Bemærk at de øvrige felter og fanebladene “Håndtér felter” og “Håndtér visning” ikke er tiltænkt at skulle bruges, da det kan have uforudsete konsekvenser for systemet.

#### Blacklist interne afdelinger (branches)

Mange biblioteker har afdelinger/brances som ikke er åbne for publikumsbetjening.

Det er muligt at blackliste disse brances, så de ikke påvirker:

1. Søgning (Søgeresultat)
2. Availabillity (Søgeresultat, Værk- og Materialevisning)
3. Beholdning (Materialevisning)
4. Afhentningsbibliotek (Brugerprofil og Lånerstatus)

Det kræver tre konfigurationsmuligheder i backend for henholdsvis:

* 1\. Søgning
* 2\. Availability og 3. Beholdning
* 4\. Afhentningsbibliotek

Konfigurationen foretages under /admin/config/ding/provider/fbs

Betaling af mellemværende med DIBS betalingsservice
-----------------------------------------------------

Når DIBS-integrationen i DDB CMS er konfigureret, kan brugerne betale deres mellemværender / bøder / gebyrer / erstatninger via hjemmesiden. Personalet har desuden mulighed for at kontrollere hvilke transaktionerne, der er foretaget under (URL: admin/config/payment/ding\_dibs/reports).

Integrationen forudsætter:

* SSL certifikat.
* Aftale med DIBS.
* Aftale med NETS for at understøtte dankort (URL: http://tech.dibspayment.com/starter\_guide ) - ”Some cards are only available through specific acquirers (for example Dankort through Nets/Teller)”.

### Rapporter for betaling af mellemværende i DIBS

Det er i DDB CMS muligt at se om brugernes betalinger er gået igennem til betaling via “Indstillinger -> Ding DIBS settings -> DING DIBS REPORTS” (Sti: admin/config/payment/ding\_dibs/reports)

BrugerID, som findes i kolonnen "Bruger" på (Sti: admin/config/payment/ding\_dibs/reports), kan du anvende til at finde navn og email ved at:

1. Logge ind og gå til (URL: https://\[bibliotekets\_domæne\].dk/user/\[BRUGERID\]/edit), hvor \[BRUGERID\] er brugerid'et
2. Skifte til fanebladet Brugerprofil, hvor du kan se de oplysninger brugeren har i DDB CMS.

### Cleared, Paid, Captured:

I rapporten for betaling af mellemværende figurerer en række kolonner: Cleared, Paid og Captured. De betyder følgende:

* Cleared: Låneren har indtastet kreditkortoplysninger og disse er godkendt.
* Paid: Betalingen gennemført i bibliotekssystemet.
* Captured: Pengene hævet på lånerens kort.

### Fejlsøgning, herunder mulighed for at administrator kan få tilsendt en mail i tilfælde af DIBS fejl

![](/system/rich/rich_files/rich_files/000/000/392/original/Udklip.PNG)

Dibsrapporten admin/config/payment/ding\_dibs/reports indeholder oplysninger for godkendte/betalte regninger og regninger med fejl.

I forbindelse med fejlsøgning er der behov at kunne finde de regninger/transaktioner der en gang mellem fejler.
Det er muligt at konfigurere DDB CMS så der sendes en mail i disse tilfælde:

Gå ind under /admin/config/payment/ding\_dibs/emails
I SET THE DAILY HOUR TO RUN THIS CRON indstillet hvor ofte dibstransaktionerne skal løbes igennem

i **Input emails that should be notified if something unusual happens with a payment.** angiver man den emailadresse fejl-transaktionerne skal sendes til.

### Verifikation af transaktioner i bibliotekssystemet og DIBS

I FBS kan regningsnumrene og brugerID fra DIBS-rapporterne i DDB CMS bruges til at fremsøge regningerne.

I DIBS admin (https://payment.architrade.com/admin/) kan regningsnumrene også bruges til at fremsøge regningerne.

1. Brugerid findes i kolonnen "Bruger", kan du bruge i DDB CMS til at finde navn og email ved at:
2. Regningsnumrene findes i kolonnen "Tekst" og starter med "Payment of library dues: ....."

### Indstillinger biblioteket selv skal konfigurere:

**Udfyld transaktionsnummer:**

1. Åbn “Indstillinger -> DIBS-indstillinger -> Ding DIBS debts payment (klik på redigér) (Sti: admin/config/payment/dibs/edit/ding\_dibs/1).
2. Indsæt transaktionsnummer i feltet “Næste ordre ID” under afsnittet “INDSTILLINGER FOR ORDRE ID”. Tallet skal være højere end det antal transaktioner, der allerede er foretaget i bibliotekets DIBS-løsning.
3. Klik på knappen “Gem indstillinger”.

**Indsæt tekst omkring brugsbetingelser for betalingstjenesten:**#Åbn “Indstillinger -> Ding DIBS settings” (Sti: admin/config/payment/ding\_dibs)

1. Udfyld felterne “Terms of sale (english)” og “Terms of sale (danish)” med tekst, der beskriver vilkår for betaling. Se eksempel på tekst nedenfor.
2. Klik på knappen “Gem indstillinger”.

### Eksempel på tekst for vilkår for betaling:

“ _Du sendes videre til betalingsvindue hos DIBS._

_Betalingen foregår i danske kroner, DKK og den kan ikke fortrydes._

_Du kan betale med følgende kort:_
_Dankort/VISA-Dankort, Mastercard, Maestro, Visa, Visa Electron, American Express og JCB._

_Aarhus Kommunes Biblioteker_
_Møllegade 1_
_8000 Aarhus C,_

_Tlf: 89409200_
_CVR: 55133018”_

### Kreditkort: Hvilke kort kan der betales med.

1. Åbn “Indstillinger -> Ding DIBS settings” (Sti: admin/config/payment/ding\_dibs).
2. Marker de kreditkort, eller andre betalingsløsninger f. eks. MobilePay, som biblioteket ønsker at understøtte i forbindelse med online betaling. (Læs i øvrigt om MobilePay længere nede i dette afsnit).
3. Klik på knappen “Gem indstillinger”.

![](/system/rich/rich_files/rich_files/000/000/393/original/Udklip.PNG)

### Udfyld DIBS automatic capture URL

**Vigtigt - dette felt skal være udfyldt for, at betalingsprocessen bliver gennemført**

1. Åbn “Indstillinger -> Ding DIBS settings” (Sti: admin/config/payment/ding\_dibs).
2. Udfyld feltet “DIBS automatic capture URL” med URL’en: https://payment.architrade.com/cgi-bin/capture.cgi.
3. Klik på knappen “Gem indstillinger”.

### Indstillinger der er konfigureret på forhånd:

En række indstillinger under “Indstillinger -> DIBS-indstillinger -> redigér (Ding DIBS debts payment)” (Sti: admin/config/payment/dibs/edit/ding\_dibs/1) vil være konfigureret på forhånd. Der benyttes følgende værdier i felterne under de forskellige afsnit:

Afsnittet “Generelle indstillinger for DIBS”:

* Merchant ID: Merchant ID er som udgangspunkt det brugernavn, der er tilknyttet din DIBS-konto og kan finde i DIBS’ administrationsgrænseflade.
* Konto: skal ikke udfyldes.
* Testtilstand: Vælg “Nej”.
* Windows type: Vælg “Flex window”.
* Order id handling after cancel: Vælg “Generate new order ID”.
* Udfør MD5-kontrol: Vælg “Ja”.
* MD5-nøgle 1: (kan være udfyldt hvis I har leveret konfigurationsoplysningerne til DDB inden etablering af produktionsmiløjet i uge 26 2014).
* MD5-nøgle 2: (kan være udfyldt hvis I har leveret konfigurationsoplysningerne til DDB inden etablering af produktionsmiløjet i uge 26 2014).
* Sprog: Vælg “Danish”.
* Valuta: Vælg “Danske kroner (DKK)”.

Afsnittet “Indstillinger for betalingsvindue”:

* Farvetema: Giver mulighed for at vælge imellem: sand, grå eller blå.

Afsnittet “Indstillinger for flex windo”:

* Farvetema: Vælg i mellem sand, grå eller blå.
* Decorator: Vælg “Tilpasset”
* Kupon: Vælg “Nej”

Afsnittet “Indstillinger for ordre ID”:\*Næste ordre ID: Indsæt et tal, der er højere end det antal transaktioner, der allerede er foretaget i Bibliotekets DIBS løsning.\*Order ID prefix: Indsæt biblioteksnummer (ISIL/Agency)

* Order ID suffix: Skal ikke udfyldes.

Afsnittet “Callback URL’s”:

* Accept URL: Indsæt “payment/dibs/accept”.
* Cancel URL: Indsæt “payment/dibs/cancel”.
* OK URL: Indsæt “payment/dibs/callbackok”.

Avancerede indstillinger:

* Calc fee: Vælg “Nej”.
* Capture now: Vælg “Nej”.
* Unique order ID: Vælg “Ja”.

### Strong Customer Authentication

NETS har siden September 14, 2019 stillet krav om Strong Customer Authentication (SCA) eller 3D Secure i forbindelse med VISA eller MasterCard.

DDB CMS gemmer ikke brugernes kreditkort og anvender kun guest checkout, så det er "kun" et spørgsmål om at aktivere funktionen i DIBS og altså ikke noget der skal ændres i DDB CMS.

Følg nedenstående trin:

1. Tag kontakt til DIBS via support@dibspayment.com og oplys merchant-ID og CVR-nummer. Merchant-ID kan findes i DIBS-kontrolpanel eller man kan også se hvad man har indtastet i CMS under /admin/config/payment/dibs/edit/ding\_dibs/1. 
   Det er også en god ide at nævne, at man kun vil have det aktiveret for aftaler, der er tilknyttet ens Merchant-ID. Hvis man f.eks. deler CVR med kommunen kan der være andre aftaler.
2. Hvis man har udenlandske kort vil DIBS bede om forretningsnummer på disse aftaler. 
   Her skal man kigge i de mails, man har modtaget da man lavede aftale med indløser, eller tage kontakt til indløser.
3. Når DIBS har modtaget det de skal bruge, aktiveres de krævede sikkerhedsforanstaltninger (som f.eks. "Dankort Secured by Nets" og "3D secure" for udenlandske kort) på ens aftaler.
4. Det er en god ide at tjekke DIBS administrationen på https://payment.architrade.com efter aktivering og sikrer at alt stadig kører igennem som det skal, og at transaktionerne er blevet sikret i oversigten eller under detaljevisning. 
   Der kan fx stå "PBS (SECURED)" ved dankort og "PBS (3D)" ved udenlandske kort.

### MobilePay

Vil I tilbyde betaling med MobilePay på hjemmesiden, kræver det en tillægsaftale med DIBS. Også selv om, I tilbyder betaling med MobilePay i appen.

Tillægsaftalen hedder MobilePay Online, og den koster 49 kr. om måneden og 1 kr. per transaktion.

DIBS skal kontaktes på mail eller telefon, for at man komme i gang, og kontaktinfo findes i linket under ved overskriften: "Kom i gang med MobilePay Online."
[dibs.dk/mobilepay](https://www.dibs.dk/mobilepay)

De vil sandsynligvis bede om følgende info:

* Eksisterende DIBS Merchant ID
* Virksomhedsnavn
* CVR nummer
* Adresse
* Postnr.
* By
* URL-adresse

Visning af mellemværender fra både ØiR og DIBS
-------------------------------------------------

Betalings-modulet gør det muligt at vise brugerne alle deres mellemværender / bøder / gebyrer / erstatninger ér sted, hvadenten de er oprettet i ØiR eller i DIBS.
For at den nedenfor beskrevne konfiguration skal fungere, forudsætter det at konfigurationen af [betaling af mellemværende med DIBS betalingsservice](https://platform.dandigbib.org/projects/ddb-cms/wiki/Ddb-cms-manual_konfiguration#Betaling-af-mellemv%C3%A6rende-medDIBS-betalingsservice) er foretaget korrekt (som beskrevet ovenfor).

### Økonomi i Rammearkitekturen (ØiR)

Økonomi i Rammearkitekturen (ØiR) er et centralt kommunalt økonomistyrings-redskab, der gør det muligt for borgerne at se al deres gæld til kommunerne ét sted.
Dette er besluttet centralt i KOMBIT.
Læs mere om ØiR her: https://kombit.dk/oeir og her: https://share-komm.kombit.dk/P0142/FBS%20Dokumenter/Forms/Implementering.aspx

Derfor skal bibliotekernes hjemmesider også integreres med ØiR.

Bibliotekerne vælger selv, hvornår de overgår til ØiR, så det bliver ikke samtidig.
Desuden vil der for det enkelte bibliotek være en overgangsperiode, hvor brugerne kan have gæld begge steder. Det betyder, at gæld, der er oprettet før den dato, det pågældende bibliotek er gået over, fortsat skal findes og betales i det gamle DIBS system, mens gæld, som er oprettet efter denne skæringsdato skal findes og afvikles i ØiR.

### Overgangsperioden

Denne overgangsperiode vil vare indtil al gæld, som er oprettet inden skæringsdatoen er enten afviklet eller afskrevet
I denne overgangsperiode er det nødvendigt at vise begge systemer på lånerstatus under mellemværender.
En bruger, som både har gæld, som er oprettet før og efter sit biblioteks skæringsdato, kan derfor opleve at se sine mellemværender se sådan ud:

![](/system/rich/rich_files/rich_files/000/001/657/original/Begge%20slags%20mellemv%C3%A6rende.jpg)

### Bemærk i forhold til betalings-modulet

BEMÆRK at integrationen til ØiR ikke er i optimal på følgende tre punkter:

1. Når brugeren trykker på knappen som i det ovenfor viste eksempel hedder "Mit betalingsoverblik" i DDB CMS og overføres til et eksternt site, hvorfra betaling kan ske i ØiR, er det nødvendigt at logge ind igen med NemID.
2. Når en betaling er gennemført på det eksterne betalingssite (fx "Mit betalingsoverblik") redirectes låneren ikke automatisk tilbage til DDB CMS.
3. Når en betaling er gennemført på det eksterne betalingssite opdateres oplysningerne ikke nødvendigvis øjeblikkeligt i FBS hvor DDB CMS for oplysningerne til Mellemværender siden fra, så låneren vil opleve at der kan gå estimeret op til 72 timer før listen med mellemværender er up-to-date.

Især punkt nummer tre er det formentlig en fordel som biblioteksmedarbejder at være opmærksom på. Det skyldes, at data kun overføres til FBS om aftenen/natten på de fem hverdage. Så betaling lavet tidligt lørdag vil først kunne ses i FBS tirsdag morgen.
Dette gøres brugeren IKKE opmærksom på ved betaling - men det fremgår under 'Mellemværende':
![](/system/rich/rich_files/rich_files/000/001/679/original/24%20timer.jpg)
Brugeren vil således blive præsenteret for meddelelsen umiddelbart inden klik på knappen som i det ovenfor viste eksempel hedder "Mit betalingsoverblik", og igen, hvis han ser at mellemværendet stadig figurerer på hans oversigt.

### Konfigurering af betalings-modulet

Når dit bibliotek overgår til ØiR skal betalings-modulet konfigureres. Det sker under /admin/config/ding/payment

Allerøverst er der mulighed for at tilføje en introtekst, som kan benyttes til at informere brugerne om forskellen på gæld, der er tilskrevet før og efter jeres skæringsdato, fx:

Dannevang Biblioteker er overgået til et nyt betalingssystem, ”Mit betalingsoverblik”, fra d. XX/XX. Mellemværender, der er oprettet inden denne dato bliver dog ikke overført til det nye system, og findes øverst på denne side. Mellemværender, der er oprettet efter denne dato findes nederst på denne side.

Ønskes ingen introtekst, fjernes flueben i ”Show introtekst”:
BEMÆRK! En fejl gør, at fjernelse af fluebenet ikke altid gør, at teksten fjernes for slutbrugeren. Er dette tilfældet, skal man sætte fluebenet igen, trykke "Gem", fjerne fluebenet igen, og så trykke "Gem" igen, så virker det

![](/system/rich/rich_files/rich_files/000/001/658/original/Introtekst.jpg)

Øverst på siden vises mellemværender, der er oprettet inden skæringsdatoen.
Ønskes disse ikke vist, fjernes flueben i ”Show list”.
Overskriften på disse kan passende være ”Mellemværender oprettet før XX/XX, betales her”

![](/system/rich/rich_files/rich_files/000/001/659/original/Payable%20on%20site.jpg)

Flueben i ”Show payment button” forudsætter korrekt konfiguration under /admin/config/payment/dibs/, læs mere her: https://platform.dandigbib.org/projects/ddb-cms/wiki/Ddb-cms-manual\_konfiguration#Betaling-af-mellemv%C3%A6rende-medDIBS-betalingsservice

Herunder vises mellemværender, der er oprettet efter skæringsdatoen.
Ønskes disse ikke vist, fjernes flueben i ”Show list”.
Overskriften på disse kan passende være ”Mellemværender oprettet efter XX/XX, betales på \[_navnet på det eksterne site, hvorfra betaling kan ske i ØiR, fx 'Mit Betalingsoverblik'_\]”
![](/system/rich/rich_files/rich_files/000/001/660/original/Payable%20off%20site.jpg)

Derpå vælges, hvilken tekst der skal stå på knappen (fx. “Mit betalingsoverblik”)
Og der indsættes URL'en til det eksterne site, hvorfra betaling kan ske i ØiR:
![](/system/rich/rich_files/rich_files/000/001/672/original/Payment%20button.jpg)

Indstillinger for reservering
-----------------------------

### Interesseperiode for reserveret materiale

Når man reserverer et materiale via DDB CMS, vil reserveringen blive tildelt en interesseperiode. Du har mulighed for at vælge en default interesseperiode på 1, 2, 3, 6 eller 12 måned/måneder. Hvis låneren ikke selv har valgt en interesseperiode, bruges som udgangspunkt default-værdien. Du kan deaktivere interesseperioden i brugerprofilen ved at sætte flueben i "Disable interest period", hvorved du fratager lånerne muligheden for at ændre deres default interesseperiode selv (gælder ikke FBS hvor dette er standard).

**Ændre default interesseperiode**

I FBS er det pt. ikke muligt at sætte default interessedato på brugerprofilen.

### Tillad/afvis sletning af reserveringer

I DDB CMS skal du bestemme, om lånerne skal kunne slette reserveringer (incl. opfyldte reserveringer) fra hjemmesiden. {background:yellow}.

DDB CMS er fra start indstillet til at tillade sletning af reserveringer. Vil du ændre på dette gøres det på følgende måde.

#### **Konfigurér tillad eller afvis sletning af reserveringer**

1. Gå til “Indstillinger -> Ding provider -> FBS Provider” (Sti: admin/config/ding/provider/fbs).
2. Sæt flueben i checkboksen “Enable reservation deletion” hvis lånerne skal have mulighed for at slette reservationer.
3. Klik på knappen “Gem indstillinger”.

### Sæt reserveringer på pause

Under brugerprofilen findes muligheden for at sætte reserveringer på pause. Herunder vises denn hjælpetekst:

Hvis du vælger en startdato der er tidligere end 5 dage fra nu, risikerer du at reserveringer når at blive opfyldt alligevel. Læs mere <a href="/ferieservice">her</a>"

Linket under "Læs mere her" virker kun, hvis der er oprettet en side med oplysninger om at sætte reserveringer på pause.
Hvis der ikke er det, så gå på /node/add/ding-page og opret én.
Benyt fx denne tekst:

Sæt dine reserveringer på pause

Her kan du finde en vejledning til, hvordan du kan sætte dine reserveringer på pause i en selvvalgt periode.

Du kan sætte dine reserveringer på pause i en periode, så du ikke skal hente reserverede materialer, hvis du er bortrejst. Når dine reserveringer er sat på pause, mister du heller ikke din plads i køen.

TIP: Vær opmærksom på, at hvis din reservation allerede er undervejs, inden din pause begynder, vil den ikke kunne stoppes i at nå frem. For at undgå det, kan du sætte din fraværsperiode til at begynde 7 dage tidligere.

Begynder din ferie f.eks. den 9. juli, skal din fraværsperiode starte den 2. juli.

Skulle det alligevel ske, at du modtager en reservation, mens du er væk, er der ikke andet at gøre end at reservere materialet igen. 

Sådan sætter du dine reserveringer på pause:

1. Log ind på "Min konto"
2. Ret din brugerprofil
3. Vælg en pauseperiode

Særligt om fjernlån:

Fjernlån kan du ikke sætte på pause i ferien, så du kan være nødt til at genbestille materialer efter din ferie.

Når siden er oprettet, tilføjes en URL-omdirigering, så linket i hjælpeteksten virker.

Dette gøres ved at klikke på ”Tilføj URL-redirect til denne indholdselement” under fanen ”URL-omdirigeringer” nederst.

![](/system/rich/rich_files/rich_files/000/001/667/original/urlomdirigering1.jpg)

Omdirigeringen skal være fra /ferieservice for at virke:

![](/system/rich/rich_files/rich_files/000/001/668/original/urlomdirigering2.jpg)

Søgning i Databrønden
-----------------------

### Brøndprofiler i VIP basen

Før det er muligt at fremsøge materialer i DDB CMS, skal du igennem to trin:

1. Oprette og konfigurere en brøndprofil i VIP-basen (URL: http://vip.dbc.dk)
2. Indstille en søgeprofil i DDB CMS, som benytter brøndprofilen

**Opret og konfigurer en brøndprofil:**

1. Fra forsiden af VIP basen: Under “J. Brøndprofiler” klik på “2. OpenSearch 3.x, 4x”.
2. Klik på “Tilføj profil”.
3. I feltet ”Navn” skal stå ”opac”.
4. Sæt flueben ved de kilder, du ønsker skal være tilgængelige gennem profilen. Vælg som minimum kilden “Bibliotekets katalog” for at søge i de bibliografiske poster.
5. Tryk “Gem”.

Det er ikke tilladt at kalde sin brøndprofil andet end “opac”, da listeservicen ellers ikke vil virke. Desuden er DDB CMS som udgangspunkt konfigureret med dette profilnavn.

Se desuden DBC's side om brøndprofiler på http://www.danbib.dk/index.php?doc=broend3\_kilder

### Indstilling af søgeprofil i DDB CMS.

Hvis du har valgt navnet “opac” til søgeprofilen, er det ikke nødvendigt, du foretager dig yderligere. Har du valgt et andet navn i VIP-basen skal du indsætte navnet som søgeprofil under “Indstillinger -> Ting -> Search profile” (Sti: admin/config/ting/settings).

### Konfiguration DDB CMS for søgning i Databrønden via Opensearch webservicen

Opensearch er den eksterne søgeservice, DDB CMS sender forespørgsler til, når der skal hentes bibliografiske poster i databrønden.

Som udgangspunkt er DDB CMS konfigureret, så hjemmesiden peger mod den seneste udgave af søgeservicen. I forbindelse med at nye versioner af opensearch frigives, er det muligt lokalt at pege på den nye version af Opensearch servicen.

**Konfigurer integration til opensearch og databrønden.**

1. Åbn “Indstillinger -> Opensearch -> Provider settings (Sti: admin/config/opensearch/settings).
2. Udfyld felterne på følgende måde:
   Bibliotekskode: \[biblioteksnummeret\]
   Search service URL: https://opensearch.addi.dk/b3.5\_5.0/
   Recommendation service URL: http://openadhl.addi.dk/1.1/
   Search profile: \[Indsæt navnet på den søgeprofil biblioteket har konfigureret i VIP basen\]
   Infomedia web service URL: https://useraccessinfomedia.addi.dk/1.4
   Enable logging: \[Udfyldes ikke\]
   Cache lifetime: 15 minutter.
3. Klik på knappen “Gem indstillinger”.

### Søgeresultater: konfigurer indstillinger for visning.

I DDB CMS er det muligt at konfigurere visningen af søgeresultater på forskellig vis.. F.eks. hvor mange søgeresultater, der skal vises pr. side og antallet af termer ved facetter. Konfiguration af søgeresultater kontrolleres fra siden “Søgeindstillinger”:

**Konfigurer indstillinger for visning af søgeresultater:**

1. Gå til “Indstillinger -> Materialer -> Søgeindstillinger” (Sti: admin/config/ting/search).
2. Konfigurer indstillinger (de forskellige valgmuligheder gennemgås nedenunder).
3. Klik på knappen “Gem indstillinger”.

**Gennemgang af konfigurationsmuligheder under “Søgeindstillinger”**

* Default results per page: Feltet definerer antallet af søgeresultater per side (paginering). Som udgangspunkt vises 10 søgeresultater.
* Number of facets: Feltet definerer antallet af termer, der hentes fra brønden per facet. Som udgangspunkt hentes 10 termer. Ved at sætte tallet højere vises en "Vis flere" og "Vis færre" valgmulighed når man folder en facetgruppe ud.
* Series title: Feltet definerer hvilket indeks, der benyttes ved klik på serietitler. Feltet er på forhånd være udfyldt med “phrase.titleSeries="@serietitle" ”, som er det eneste indeks, der kan anvendes.
* Default sorting: Dropdownmenuen giver mulighed for at vælge hvilke sorteringskriterier, der som udgangspunkt skal anvendes på søgeresultaterne. Der kan vælges mellem syv sorteringer, bl.a. efter alfabetisk orden på titler og forfatter. Som udgangspunkt er valg "Sorter efter Bedste match". Det er nødvendigt at vælge "Sorter efter Bedste match" hvis du ønsker at anvende "rank\_frequency" ellers vil sorteringen slå over på "rank\_general" (se afsnittet "Rankering og Boost").
* Search form style (Søgeprofiler - mulighed med modulet ting\_field\_search, også kaldet Vejle-modulet): Valgmulighederne er Normal, Extended og Extended with profiles

### Søgefelt: normalt, udvidet eller udvidet med profiler

Der er tre måder søgefeltet kan se ud: normal, udvidet og udvidet med profiler.

Hvilken måde søgefeltet ser ud, rettes under Indstillinger -> Materialer -> Søgeindstillinger (Sti: /admin/config/ting/search)

NB! Ryd cachen efter indstillingerne er rettet, for at rettelserne bliver vist.

![](/system/rich/rich_files/rich_files/000/000/023/original/search_dump4.PNG)

#### Normal visning - billedet til højre viser, hvordan søgefeltet udvider sig, når bruger skriver i felet

![](/system/rich/rich_files/rich_files/000/000/021/original/search_dump1.PNG) ![](/system/rich/rich_files/rich_files/000/000/020/original/search_dump2.PNG)

#### Udvidet (extended)

![](/system/rich/rich_files/rich_files/000/000/024/original/search_dump5.PNG)

#### Udvidet med profiler (extended with profiles)

[Vejledning i at konfigurere profilerne](https://platform.dandigbib.org/projects/ddb-cms/wiki/Ddb-cms-manual_konfiguration_next-version#S%C3%B8geprofiler-ting_field_search).

![](/system/rich/rich_files/rich_files/000/000/022/original/search_dump3.PNG)

### Sprogangivelse på udenlandske boglige materialer

Det er muligt at tilføje sprog efter titlen på et udenlandsk bogligt materiale.

Eksempel: "Fru Inés (Norsk)"

![](/system/rich/rich_files/rich_files/000/001/180/original/2019-12-10%2014_38_21-Search%20Ting%20_%20phrase.subject=_sk_%20and%20term.language=_norsk_%20_%20%E2%80%93%20Google%20Chrome.png)

Funktionen konfigureres under Configuration -> TING -> Language (Sti: /admin/config/ting/language)

1. Default language: "Dansk".
2. Markér alle boglige materialer under "Title suffix".
3. Gem

### Visning af beholdningsoplysninger (sektionen "Se alle eksemplarer)

Det er muligt at vælge om sektionen med beholdningsoplysninger som udgangspunkt skal være udfoldet på de enkelte materialeposter eller lukket så brugeren aktivt skal klikke på sektionen for at folde den ud. Som udgangspunkt er sektionen med beholdningsoplysninger lukket. Visningen kontrolleres på følgende måde:

1. Åben "Indstillinger > Ting/Materialer > Ting/Materialer > Local settings" eller tilgå siden direkte ved at indsætte admin/config/ting/settings/local\_config efter bibliotekets domæne i browseren.
   ![](/system/rich/rich_files/rich_files/000/000/374/original/Udklip.PNG)
2. Vælg fra dropdownmenuen "Group holdings available" mellem indstillingerne "Default (don't change)" (defaultværdi - dvs. lukket), "Open" (Åben uden mulighed for at lukke), "Collapsed" (lukket), "Collapsible" (Åben, med mulighed for at lukke).
3. Klik på knappen "Gem indstillinger".

### Facetbrowser

Facetbrowseren er navnet på de forskellige muligheder for afgrænsning, man finder i venstre side i forbindelse med materialesøgninger. Afgrænsningerne kan f.eks. være på materialetype, forfatter og emne. Disse forskellige typer af afgrænsninger kaldes facetgrupper.

I DDB CMS er det muligt at konfigurere opsætningen af facetbrowseren og bl.a. styre hvilke facetgrupper, der vises, rækkefølgen af disse, hvor mange facetter, der vises under de enkelte facetgrupper og lignende. Som udgangspunkt er facetbrowseren konfigureret med facetgrupperne “Materialetype”, “Forfatter”, “Emne”, “Sprog”, “Målgruppe”, “Årstal” og “Kilde”.

Facetgrupperne i facetbrowseren opbygges ud fra de facet-indekser der findes på https://opensearch.addi.dk/b3.5\_4.5/?showCqlFile&repository=prod&cql=opensearch\_cql.xml#facet.

**Tilføj facetgruppe**Under “Ting facets” er det muligt tilføje nye facetter.

1. Åbn “Indstillinger -> Ting facets (Under afsnittet “Ting”)” (Sti: https://bibliotekets-hjemmesideadresse.dk/admin/config/ting/facets).
2. Tilføj en ny facet ved at udfylde “Facet ID” og “Titel” og vælg hvilken sortering, der skal anvendes for den enkelte facet. Du kan finde en tabel over tilgængelige facetgrupper på https://opensearch.addi.dk/b3.5\_4.5/?showCqlFile&repository=prod&cql=opensearch\_cql.xml#facet. Find “Facet” i kolonnen “Namespace” i tabellen. \*
3. Klik på knappen “Gem ændringer”.

**Muligheder under “Ting facets”**Nedenfor er en kort beskrivelse af andre vigtige felter og konfigurationsmuligheder under “Ting facets”:

* “Visible facets amount": Dropdownmenuen giver mulighed for at bestemme, hvor mange facetgrupper, der som udgangspunkt skal være åbne i grænsefladen. Det betyder at brugerne kan se indholdet af facetgruppen, uden først at åbne den. Der kan vælges fra 1 til 15 åbne facetgrupper. Det anbefales ikke at have en lang liste med åbne facetgrupper, da siden kan blive meget lang og i sidste ende svær at overskue for brugerne.
* "Number of terms" angiver antallet af synlige facetter i hver facetgruppe. Antallet af termer, der hentes, er som default 10. Bemærk at antallet af facetter afhænger af hvor mange termer, der er tilgængelige i brønden. Selvom der står “10” i “Number of terms” vil der kun blive vist fem facetter, hvis der kun er fem termer i brønden.
* Skift rækkefølgen af facetgrupper ved at klikke og trække på korspilen yderst til venstre ud for en facetgruppe.

### Knapper på online materiale: Konfigurer tekst på knapper.

Under “Online types and URL labes” er det muligt at tilpasse teksten på knapper på online materialer.

1. Åbn “Indstillinger -> “Online types and URL labels” (URL: admin/config/ting/online\_types)
2. Tryk på knappen opdatér. Alle materialetyper, som er repræsenteret i bibliotekets kilder hentes nu fra brønden.
3. Tryk på "Online types" for at folde listen med materialetyper ud.
4. Marker de materialetyper, der skal kunne tilgås online.
5. Tryk på "Type specific labels” for at folde listen med materialetyper ud, hvor teksten på knapper kan ændres.
6. Find f.eks. "film (net)" på listen og skriv f.eks. "Se filmen" i feltet
7. Tryk på knappen "Gem indstillinger" nederst på siden.

Materialetyper der med fordel kan tildeles knappen "Se online" (har relationen hasOnlineAccess). Se http://osswiki.dbc.dk/bin/view/Databroend/KilderBroend3 for overblik over kilder med relationen hasOnlineAccess.

Bemærk at en kildes materialetyper kan fremsøges via følgende søgning: term.acSource="KILDENS NAVN", hvor de er synlige i søgeresultatet, hvis facetgruppen facet.type er aktiveret.

### Beholdningsoplysninger på materiale.

Under “Provider availability holdings” kan du angive hvilke materialer, der skal tildeles beholdningsoplysninger.

1. Åbn “Indstillinger -> Provider availability holdings” (Sti: admin/config/ting/holdings)
2. Tryk på knappen opdatér. Alle materialetyper som er repræsenteret i de bibliografiske poster hentes nu fra brønden.
3. Marker de materialetyper, der skal tildeles beholdningsoplysninger.
4. Tryk på knappen "Gem indstillinger" nederst på siden.

Vær opmærksom på at materialetyperne med årgange/numre, dvs. Tidsskrift, Årbog og Periodikum ikke må markeres, da beholdningsoplysninger for disse materialetyper ikke kan indsættes på pif-posten, men på årgange/numre.

### Beholdningsoplysninger - Opstilling

Under Indstillinger > Ding > Ding Provider > FBS Provider > HOLDINGS SUFFIX (Sti: /admin/config/ding/provider/fbs) kan man tilpasse opstillingssignaturen.

Beholdningsvisningen kan bestå af forskellige niveauer for opstilling der kan konfigureres så det afspejler lokal praksis.

Følgende fire niveauer vises altid: Branch > Department > Location > Sublocation

Derudover kan man vælge at få vist:

* Material group description - Materialegruppe
* Simple - DK5 Klassemærke + Inverteret forfatternavn
* Shelfmark - Hyldemærke

Man kan lave følgende kombinationer:

**Simple** (Default konfiguration)
Greve Bibliotek > Børn > 77.693 > Revenson, Judy

**Simple + Material group description**
Greve Bibliotek > Børn > Bog > 77.693 > Revenson, Judy

**Shelf mark** (simulerer DDELibras opstilling med differentieret visning for f. eks. skøn- og faglitteratur)
Greve Bibliotek > Børn > Enestående

**Shelf mark + Material group description**
Greve Bibliotek > Børn > Bog > Enestående

##### Beskrivelse af shelfmark

1. **Hvis felt 652 delfelt m = sk** - Vises 1. ord (efter evt. soltegn) i felt 100 delfelt a
   1. Hvis felt 100 mangler vises:
      1. Første ord (efter evt. soltegn) i 110 delfelt a
   2. Hvis felt 100 og felt 110 mangler vises:
      1. Første ord (efter evt. soltegn) i 245 delfelt a
2. **Hvis felt 652 delfelt m ikke = sk** og posten indeholder felt 039 - Vises indholdet i felt 039 delfelterne a + b (bogstavskoderne oversættes, se herunder) **efterfulgt af**
   1. Hvis felt 100 vises:
      1. Første ord (efter evt. soltegn) i 100 delfelt a
   2. Hvis felt 100 mangler vises:
      1. Første ord (efter evt. soltegn) i 110 delfelt a
   3. Hvis felt 100 og felt 110 mangler vises:
      1. Første ord (efter evt. soltegn) i 239 delfelt a
   4. Hvis felt 100, felt 110 og felt 239 mangler vises
      1. Første ord (efter evt. soltegn) i 245 delfelt a
3. **Hvis felt 652 delfelt m ikke = sk og der ikke er et felt 039** - Vises indhold af felt 652 delfelt m (DK5-koden) + indhold i delfelt b
   1. Hvis felt 652 delfelt b ikke findes vises:
      1. indhold i delfelt a + delfelt h (kommasepareret)
         (Forklarende tekst til 652 m vises ikke)
         **efterfulgt af** (ligesom ovenfor)
   2. Hvis felt 100 vises:
      1. Første ord (efter evt. soltegn) i 100 delfelt a
   3. Hvis felt 100 mangler vises:
      1. Første ord (efter evt. soltegn) i 110 delfelt a
   4. Hvis felt 100 og felt 110 mangler vises:
      1. Første ord (efter evt. soltegn) i 245 delfelt a

### Materialer til reservation: tildeling af knap.

Under “Reservable Ting object” er det muligt at bestemme hvilke materialer, der skal tildeles en knap til reservering.

1. Åbn “Indstillinger -> Reservable Ting objects” (URL: admin/config/ting/reservable)
2. Tryk på “Opdatér”. Alle materialetyper som er repræsenteret i de bibliografiske poster hentes nu fra brønden.
3. Marker de kilder (typisk kun "bibliotekskatalog"), hvis poster skal kunne tildeles en Reservér knap.
4. Marker de Typer der skal tildeles en Reservér knap.
5. Tryk på knappen "Gem indstillinger" nederst på siden.

Vær opmærksom på at materialetypen Tidsskrift IKKE må markeres da Reservérknapper for tidsskrifter ikke indsættes på pif-posten, men på årgange/numre.

### Ting digital article service ("Guldknappen")

Modulet Ting digital article service (ting\_das) gør det muligt for brugerne at bestille artikler via Digital Artikelservice direkte gennem DDB CMS.
Det er ikke muligt at aktivere modulet uden at indgå en forudgående aftale med Det Kongelige Bibliotek. Læs mere om Digital Artikelservice og tegn abonnement her: https://forbiblioteker.kb.dk/services/digital-artikelservice?
Hvis I vælger at tegne et abonnement, vil I modtage et brugernavn + password fra Det Kongelige Bibliotek, uden hvilket modulet ikke kan konfigureres.
Det vil derpå være nødvendigt at aktivere modulet. Hvis I er webmastere eller programmører, gøres det under /admin/modules søg på ’das’, og I vil fremfinde det:
![](/system/rich/rich_files/rich_files/000/001/661/original/Aktiver%20modul.jpg)

Hvis I er redaktørbibliotek, kan I ikke selv aktivere modulet. I skal da oprette en sag hos Kunderservice hos DBC https://kundeservice.dbc.dk/ og bede om at få det aktiveret.

Når det så er aktiveret, skal det konfigureres.

#### Konfigurering af Ting digital article service ("Guldknappen")

Konfigurering af Ting digital article service sker under /admin/config/ting/das og under /admin/config/ting/das/credentials

Knappen til bestilling via Digital Artikelservice virker sådan, at den bliver vist på udvalgte materialetyper, når der ikke er en ”Se online” knap.
Det kan konfigureres under /admin/config/ting/das under ”Data Well Types” hvilke materialetyper, knappen skal vises på. Som default er kun materialetypen ”tidsskriftsartikel” valgt, hvilket også er den anbefalede konfiguration:
![](/system/rich/rich_files/rich_files/000/001/719/original/Data%20well%20types.jpg)
Det betyder også, at knappen kun bliver vist, hvis de kilder hvori de(n) pågældende materialetype(r) forekommer uden onlineadgang, er aktiveret i jeres brøndprofiler. 
Med materialetypen ”tidsskriftsartikel” betyder det at kilden ”Artikelbasens tidsskriftsartikler” skal være aktiveret i jeres brøndprofiler:
![](/system/rich/rich_files/rich_files/000/001/720/original/Tidsskriftsartikler%20i%20VIP'en.jpg)
Husk på, at efter man har ændret i sin brøndprofil, går der gerne nogle timer, inden ændringen slår igennem.

Under /admin/config/ting/das skrives de tekster, der skal vises til brugeren ved klik på ”Bestil digital kopi” under en artikel.
Denne tekst udfyldes her:
![](/system/rich/rich_files/rich_files/000/001/662/original/Tekst%20f%C3%B8r.jpg)
 

Og her:
![](/system/rich/rich_files/rich_files/000/001/663/original/Tekst%20efter.jpg)

Slutbrugeren vil møde disse tekster efter klik på "Bestil digital kopi" sådan her:
![](/system/rich/rich_files/rich_files/000/001/664/original/Tekst%20til%20bruger.jpg)
Når brugeren også bedes opgive afhentningsbibliotek, skyldes det at i de meget få tilfælde, hvor en artikel ikke kan leveres digitalt, konverteres bestillingen til et almindeligt fjernlån.

Under /admin/config/ting/das/credentials skal der også konfigureres, før modulet virker:
![](/system/rich/rich_files/rich_files/000/001/665/original/Credentials.jpg)
Under ”End point” skal der stå https://webservice.statsbiblioteket.dk/elba-webservices/services/placecopyrequest
Under ”Username” og ”Password” udfyldes det brugernavn + adgangskode, som I har modtaget fra Det Kongelige Bibliotek i forbindelse med at i tegnede abonnementet.

### Søgeprofiler (ting\_field\_search)

Når der vælges udvidet søgefelt med profilerne, så kan man under Indstillinger -> Materialer -> Ting Field Search Profiles ændre, tilføje og slette profilerne.

Som minimum skal profilen have en titel og en prædefineret forespørgsel. Prøv at tilføje en profil - eks. med titel "Slægtsforskning".![](ting-field-search_dump1.png)

I feltet "Forespørgsel" er der tilføjet et dk5-nr. for slægtsforskning, og mere kræves ikke. Forespørgslen kunne være mere avanceret, eller der kunne eks. også afgrænses for, hvor gamle materialer der ønskes fremsøgt i feltet "New materials".

Under fanen "Søgeresultat" i menuen til venstre, kan man også ændre nogle parametre for, hvor mange resultater der vises pr. side eller hvilken sortering der ønskes. Og for den avancerede bruger, så er det også muligt under fanen "Facets", at ændre på hvilke facetter der vises til venstre i søgeresultatet.![](ting-field-search_dump2.png)

OBS: Hvis man retter i en af default søgeprofilerne så bliver rettelsen overskrevet næste gang en ny version af DDB CMS udrulles. Dette kan omgås ved at deaktivere default søgeprofilen![](https://platform.dandigbib.org/projects/ddb-cms/wiki/ting-field-search_dump2.png) og lave en ny der passer til bibliotekets behov, men dermed får man heller ikke glæde af eventuelle senere rettelser til den deaktiverede søgeprofil.

NB. Hvis man vælger at klone en søgeprofil skal man ændre maskinnavnet så det er unikt.

### Rankering og Boost

Rankering i forhold til søgninger handler om i hvilken rækkefølge søgeresultaterne vises.

Overordnet set bestemmes rankeringen/rækkefølgen af søgeresultaterne, ved at felterne i de forskellige værker tildeles en værdi på baggrund af en række kriterier. Jo højere værdi et værk samlet set tildeles, jo højere vil det figurere i søgeresultaterne. Nedenfor ses et udsnit af værket “Hypnotiseret” og et udsnit af de felter, der definerer den pågældende post i brønden. I forbindelse med evt. rankering vil disse felter blive tildelt en værdi, som bestemmer postens placering i det søgeresultat, der vises for brugerne.

Et eksempel er, at brugeren laver en søgning på “Hypnotisøren”. Herefter undersøger opensearch om søgestrengen findes i et eller flere af felterne/indekserne på de søgbare poster. På den baggrund tildeles de enkelte poster en vægtning, som definerer rækkefølgen af de enkelte poster i søgeresultatet på DDB CMS. Hvordan værdien af de enkelte felter i et værk bestemmes afhænger af hvilken søgemetode, der anvendes.

I DDB CMS kan man som udgangspunkt vælge mellem to prædefinerede metoder til at bestemme rækkefølgen af søgeresultaterne: “Rank\_frequency” og “Rank\_general”. Alternativt kan man vælge “No rank” eller “Custom ranking”. I førstnævnte tilfælde vil søgeresultatet blive listet i den rækkefølge de enkelte poster er indekseret. Ved “Custom ranking” vælger du selv hvilke felter, der skal rankeres på og deres værdi. Som udgangspunkt anvendes metoden “Rank\_frequency” i DDB CMS.

#### Vælg prædefinerede rankeringmetode

Vælg rankeringsmetode på følgende måde:

1. Åben “Indstillinger ->Search result ranking (under afsnittet “Opensearch”)” (Sti: admin/config/opensearch/ranking)
2. Vælg rankeringsmetode under dropdownmenuen “Type”. Der kan vælges mellem “Best match” (er det samme som “Rank frequency”), General rank (er det samme som “Rank general”) eller “No rank”.
3. Tryk på knappen “Gem ændringer” nederst på siden.

#### Rank frequency.

“Rank frequency” anvendes som default rankering fra og med DDB CMS 2015 3. Nedenstående beskrivelse af "Rank frequency" kan findes i sin oprindelige form i magasinet "#DBC, nr.2, april 2015".

I forbindelse med at brugeren laver en søgning “gætter” “Rank frequency” på om brugeren søger efter titel, forfatter eller emne og vælger dernæst en måde at rankere resultaterne på, som er god til netop dén type søgninger.

Der er lavet tre forskellige rankeringsalgoritmer: én, der er egnet til titelsøgninger, én til forfattersøgninger og én til emnesøgninger. Når rankeringsalgoritmen skal vælge,
hvilke søgeresultater, der skal vises først, ser den blandt andet på, hvilke felter i posten, søgeordene optræder i. For eksempel giver Titel-algoritmen en højere placering til poster, hvor søgeordene optræder i feltet ’Hovedtitel’ frem for i andre titelfelter. Og hvis søgeordene ligefrem står ved siden af hinanden i Hovedtitel-feltet, bliver posten endnu højere placeret.

I 80% af tilfældene vælges den rigtige rankering. De søgninger, hvor det ikke er tilfældet, er typisk, når titelsøgninger består af navne – for eksempel, hvis man skriver ’Peter Pedal’. Heldigvis får man altid at vide, hvilken rankeringsform der er valgt, så man kan vælge en anden, hvis det er nødvendigt. På illustrationen nedenfor er der lavet en søgning på “Peter Pedal”. I infoboksen beskrives at “Søgeresultatet er sorteret efter forfatter”, mens dropdownmenuen giver mulighed for at vælge en anden søgning.![](Rank_frequency_dump1.png)

Rank\_frequency kan ikke anvendes sammen med rank/boost parametrene i “custom ranking fields” (se afsnittet “Custom ranking: tilpas rankering med egne parametre”).

![](/system/rich/rich_files/rich_files/000/001/310/original/Rank%20frequency.png)

#### Rank general.

Rankering af søgeresultatet udregnes ud fra den værdi felterne i posten tildeles, således at værket med den højeste værdi vises først. “Rank general” er karakteriseret, ved at den benytter en række standardværdier til felterne “Forfatter”, “Titel”, “Emne” og “default” i forbindelse med rankeringen af søgeresultater. Posten med den højeste værdi vil ligge først i søgeresultaterne. Nedenfor en beskrivelse af hvilke værdier “Rank general” tildeler de nævnte felter:

 

Forfatter

Titel

Emne

Default

Term (vægtning)

4

3

2

1

Frase (vægtning)

8

6

3

2

#### Custom ranking: Tilpas rankering med egne parametre

“Custom ranking” sorterer søgeresultatet efter de poster/værker hvor brugerens søgetermer optræder i de felter/indekser lokaladministrator har defineret skal prioriteres.Med “Custom ranking” kan du dermed selv vælge hvilke felter, der er vigtigst og som skal vægtes højest i forbindelse med rankeringen. F.eks. kan det være, at du ønsker at definere at titler er vigtigere end forfatternavne, der igen er vigtigere end emner.Bemærk at “Custom ranking” ikke kan anvendes sammen med “Rank frequency” eller “Rank general”. Har du aktiveret “Custom ranking” vil andre rankeringsmetoder blive slået fra.Nedenfor er en beskrivelse af hvordan “Custom ranking” konfigureres:

1. Åben “Indstillinger -> Opensearch -> Search result ranking” (Sti: /admin/config/opensearch/ranking).
2. Marker checkboksen “Enable Custom Ranking”
3. Vælg under “Custom Ranking Fields” hvilket felt der skal vægtes (feltnavn), værdien for den pågældende vægtning (vægt) og hvilken type søgninger vægtningen skal gælde for (type).
4. Tryk på knappen “Add another ranking field” hvis du ønsker at tilføje endnu et felt der skal rankeres på.
5. Tryk på knappen “Gem ændringer”.

#### Custom ranking: Beskrivelse af indstillingsmuligheder.

Nedenfor er en beskrivelse af de forskellige indstillingsmuligheder under “Custom ranking files”:

* Type: Feltet har to værdier: “Frase” og “Ord”. En frase består af to eller flere søgeord f.eks. “Klaus Rifbjerg” eller “kødædende plante”.
* Feltnavn: Det er muligt at vælge mellem følgende seks felter: “kilde”, “titel”, “forfatter”, “emne”, “publiseringsår” og “materialetype”.
* Værdi: Vælg en værdi fra 1 til 10. Højere vægt betyder højere placering i søgeresultaterne.

Rankering er et komplekst emne og der er ikke nogen endegyldig løsning. Undersøg konsekvenserne af tilpasningen grundigt med mange forskellige søgninger og emner. Ved at fremme rankeringen af nogle materialetyper resulterer det typisk i at andre nedprioriteres.

#### Boost - fremhæv specifikke søgeposter.

Boost sorterer søgeresultatet efter de poster/værker, som har bestemte felter/indekser med en bestemt værdi defineret af lokaladministrator. Her vælger du altså hvilke værdier i bestemte felter, der er vigtigst, som f. eks. materialetypen bog eller sproget dansk.

Opsætning af boost

1. Åben “Indstillinger ->Search result boost (under afsnittet “Opensearch”)” (Sti: /admin/config/opensearch/boost).
2. Opsæt forskellige felter med tilhørende værdier, der skal fremhæves i søgeresultaterne. Pt. kan der boostes på følgende otte felter: kilde, forfatter, udgivelsesår, sprog, materialetype, emneord, dk5 (til brug for dette anvendes facet.dk5 hvor der så ”kun” boostes på første forekomst ”hovedopstilling”) og ISBN. I feltet “Værdi” angives værdien for det felt, man ønsker at booste på. I feltet vægt angives værdien for den pågældende vægt. Ønskes negativ boost, angives en vægt mellem 0 og 1 - dette vil få materialer med den valgte værdi til at blive vist længere nede i søgerestulatet. Ved anvendelse af decimaler benyttes punktum, ikke komma, fx. "0.01", ikke "0,01"
3. Tryk på knappen “Gem ændringer”.

#### queryDebug

Via webklienten til opensearch http://opensearch.addi.dk/4.0.1/ er muligt at se hvilken vægt de enkelte søgeresultater tildeles ved at angive parameteren QueryDebug, som en del af forespørgslen. For at bruge webklienten forudsætter dog, at DBC har åbnet for kald fra den IP-adresse forespørgslen sendes fra. Alternativt er der fri adgang på DBC’s testbrønd http://oss-services.dbc.dk/opensearch/ som dog kun indeholder en delmængde af driftsbrønden.

Eksempel på en simple-search søgning på “Hypnotisøren” med rankeringsmetoden “Rank general” og “queryDebug” angivet så den udregnede vægt for søgeresultaterne vises.

Søgeresultatet returneres med angivelse af hvilken vægt de enkelte søgeresultater tildeles - se efter “” i søgeresultatet :

Se desuden en beskrivelse af øvrige parametre der kan anvendes i forbindelse med forespørgsler til opensearch på:https://opensource.dbc.dk/services/open-search-web-service

### Autofuldførsel med “Ortograf servicen”.

Når servicen “Ortograf” er slået til, vil lånerne i forbindelse med søgninger på DDB CMS få vist forslag til autofuldførelse af søgeord.

Servicen konfigureres på følgende måde:

1. Åbn “Indstillinger - > Opensearch -> Ting search autocomplete setting (Sti: admin/config/opensearch/autocomplete).
2. Udfyld felterne, som beskrevet nedenfor:
   1. Autocomplete URL: https://ortograf.dbc.dk/ortograf/suggest
   2. Max suggestions: 10
   3. Minimum string: 3
3. Klik på knappen “Gem indstillinger”.

Søg redaktionelt indhold på hjemmesiden
-----------------------------------------

Den tekniske understøttelse af søgning på hjemmesiden varetages af modulet **Search api**.

Under /admin/config/search/search\_api/index/default\_multiple\_index kan admin cleare indekset, samt sætte sitet til at genindeksere. Har man meget indhold på hjemmesiden skal man dog være opmærksom på at det tager tid at indeksere alt indholdet.

Clearing af index: klik på Clear all index data

Under /admin/config/search/search\_api/index/default\_multiple\_index/fields kan admin konfigurere hvilke felter der skal indekseres.

Søgning på arrangementer
--------------------------

![](/system/rich/rich_files/rich_files/000/000/109/original/arrangementer-soeg_dump1.PNG)

På undersiden for arrangementer, ofte kaldet Arrangementer eller Det sker, er det muligt at fremsøge specifikke arrangementer ved at søge på ord, eller afgræsne til bestemte datoer, og desuden filtrere ud fra nogle kategorier, eller hvor et materiale står placeret.

Som standard vises arrangementerne grupperet efter måneder, men under /admin/config/ding\_event/settings kan dette ændres til at man gruppere efter dato.

Smart Search
------------

Smart Search er et værktøj der forbedrer rankering, og ved omdirigering til alternativ søgestreng også selve søgningen.
Smart Search består af en manuel og en automatisk del.

### **Automatisk Smart Search**

Den automatiske del forbedrer rankeringen ved at placere op til 5 poster øverst i søgeresulatet. Disse udvælges ud fra statistiske data om, hvad andre brugere, der har foretaget samme søgning indenfor de sidste 365 dage, efterfølgende har klikket på. Jo flere af disse brugere, der har klikket på en post, jo højere op kommer den. Har tidligere brugere ikke klikket på tilstrækkeligt mange poster til at fylde alle 5 pladser, fyldes kun dem, som der er datagrundlag for.

De øvrige poster rankeres efter de første op til 5, som de ville være rankeret, hvis Smart Search ikke var aktiveret, dvs med den rankeringsmetode (rank\_frequency eller eventuel custom ranking), som er valgt på det pågældende bibliotek.
For at automatisk Smart Search skal fungere, skal den være konfigureret, læs [afsnittet om ”Indstillinger af Smart Search”](https://platform.dandigbib.org/projects/ddb-cms/wiki/Ddb-cms-manual_konfiguration_next-version#Smart-Search-indstillinger).

### **Manuel tilretning med Smart Search**

Manuel tilretning giver mulighed for at tilpasse den enkelte søgning, så den giver mere relevante resultater til brugerne.
Når en bruger med redaktør- eller administratorrettigheder foretager en søgning, kommer der en formular frem over søgeresultatet, som kan bruges til at tilpasse søgningen. Klik på pilen for at udfolde formularen.
![](/system/rich/rich_files/rich_files/000/001/372/original/1%20Foldet%20ind.jpg)

Udfoldet efter klik:
![](/system/rich/rich_files/rich_files/000/001/373/original/2%20Foldet%20ud.jpg)

#### Øverste del af formularen

Den øverste del af formularen indeholder data om søgningen:

![](/system/rich/rich_files/rich_files/000/001/374/original/3%20%C3%98verste%20del.jpg)

Der står hvilken søgestreng er blevet brugt (1), hvor mange gange den søgning er forekommet nationalt i løbet af det sidste år (2), og hvor mange gange i løbet af det sidste 30 dage (3). Der er også muligt at vælge hvilken status Smart Search tilretning har for den pågældende søgestreng (4). Som default er den ”Inaktiv”. Den skal sættes til status ”Aktiv”, hvis du ønsker at den skal fungere på den pågældende søgestreng.

**Vigtigt! En tilretning slår først i gennem når den gives status Aktiv.
Hvis du oplever at den tilretning, du har lavet ikke har nogen effekt, tjek da hvilken status den har.**
 

Man kan også vælge at tildele sin tilretning status ”Behandlet”, hvis man ønsker at indikere at man har set på den pågældende søgning og besluttet, at den ikke skulle tilrettes. Endelig er det muligt at vælge status ”Planlagt” som giver mulighed for sætte en tilretning på i en periode. F.eks. kan søgning på bagning op til jul giver juleopskrifter, eller i måneden op til et forfatter-foredrag på biblioteket kan dennes værker promoveres. Når ”Planlagt” vælges kommer der følgende felter frem:

![](/system/rich/rich_files/rich_files/000/001/375/original/4%20Periode.jpg)

Her kan der indsættes datoer for hvornår tilretningen træder i kraft og hvornår den stopper igen.

#### Alternativ søgestreng

Der kan angives en alternativ søgestreng, som bedre matcher brugernes hensigt med en given søgning. Et eksempel: Søgningen ”lydbøger” giver meget få resultater, hvoraf kun et fåtal er lydbøger. Derfor tilrettes søgningen ved tilføjelsen af ”term.type=lydbog\*”, så materialetypen lydbog tilføjes. Det er en god konvention altid at tilføje et ”or \[den oprindelige søgestreng\]”, når søgestrengen ændres, i dette tilfælde ”or lydbøger”. 

![](/system/rich/rich_files/rich_files/000/001/376/original/5%20alt%20s%C3%B8gestreng.jpg)
Denne tilretning kunne fx kombineres med en sortering med nyeste først, eller med boost på materialetypen lydbøger (men ikke begge dele, da tvungen sortering ikke kan kombineres med boost).

### Fremhæv og boost

#### Fremhævede materialer

Der er muligt at placere op til 5 specifikke materialer øverst i søgeresultatet. Det kan være materialer, som vi ved at brugerne efterspørger, når de laver en specifik søgning, f.eks. den første bog i Harry Potter-serien, når de søger efter Harry Potter.

Det gøres ved at indtaste postens faustnummer direkte ind i feltet. Dette findes nemmest ved at fremsøge posten og derpå kopiere den sidste del af url’en (adresselinjen). Posten kan tilføjes både som almindeligt faustnummer, eller med formerne: 870970-basis%3A53214169 eller 870970-basis:A53214169. Modulet kan håndtere alle tre former.
![](/system/rich/rich_files/rich_files/000/001/377/original/6%20Promoted.jpg)

Når der er valgt en række materialer, kan rækkefølgen ændres ved at trække rundt på dem. Posterne kan også slettes fra fremhævede materialer ved at trykke på (x) knappen til højre.
Kun poster som allerede er i søgeresultatet kan fremhæves. Hvis du ønsker at fremhæve en post som ikke findes i søgeresultatet på den pågældende søgning, skal søgestrengen tilrettes først.

#### Boost værdier

Der er også muligt at tilpasse boost på specifikke søgestrenge. Som et eksempel søgningen ”film” giver et blandet resultat af film og andre materialetyper. Vi ved, at brugerne først og fremmest efterspørger fim her, så derfor kan der boostes materialetyperne DVD, blu-ray og film (net).
![](/system/rich/rich_files/rich_files/000/001/378/original/7%20custom%20boost.jpg)

Ønsker du at tilrette en søgning vha boost, skal du starte med at klikke på ”Add Custom boost values” og derpå i ”Feltnavn”, hvorunder du vælger hvilket felt du gerne vil booste. Derpå udfyldes værdien, som skal boostes, og til sidst hvilken vægt, den skal boostes med.

![](/system/rich/rich_files/rich_files/000/001/379/original/8%20Boost%20felter.jpg)

Når feltet ”Værdi” skal udfyldes er det vigtigt at skrive dem præcis på samme måde som de står i facetterne, fx ”dvd”, ”film (net)” eller ”blu-ray”:
![](/system/rich/rich_files/rich_files/000/001/380/original/9%20Facet-v%C3%A6rdier.JPG)
Derpå angives en boostens vægt. Vægten skal være tal der er større end 0, erfaringsmæssigt er en vægt mellem 20 – 100 som regel passende, idet mindre tal ikke har ret meget effekt, mens større tal let skævvrider et søgeresultat.

Ønskes der at tilføje flere boosts trykkes der på knappen ” Add custom boost values”.

### Sortering

Søgetrenge kan også tilrettes med tvungen sortering af søgeresultatet, f.eks. på ”Udgivelsesår – nyeste først”. Bemærk, at hvis der vælges en tvungen sortering, bliver tilretninger for boost og fremhævelse af materialer sat ud af kraft.

### ![](/system/rich/rich_files/rich_files/000/001/381/original/10%20Sorterint.jpg)

Ved klik i sorteringsfeltet kommer en drop-down:

![](/system/rich/rich_files/rich_files/000/001/382/original/11%20Sortering%202.jpg)

### Gem

![](/system/rich/rich_files/rich_files/000/001/383/original/12%20Gem.jpg)

Nederst er der en gem knap.
**Vigtigt! Hvis du laver en tilretning og trykker på gem men det ikke sker noget, er det som regel fordi konfigurationen stadigvæk har status ”Inaktiv”. Den skal sættes til status ”Aktiv” før der sker noget.**
 

### Gå til oversigt

Nederst i formen er der knap ”Gå til oversigt” Når du klikker på den, ser du en oversigt over de 5000 hyppigste søgninger, samt de søgninger som er blevet manuelt tilrettet.

![](/system/rich/rich_files/rich_files/000/001/384/original/13%20Oversigt.jpg)

Oversigten findes på /admin/structure/entity-type/ting\_type/smart\_search\_string/list og viser de 5000 søgninger, der på landsplan er foretaget flest gange de sidste 365 dage, samt alle søgninger som er blevet tilrettet manuelt. Oversigten opdateres en gang om ugen. Hensigten med oversigten er at vise, hvilke søgninger, det vil give størst effekt at foretage en manuel tilretning af.

![](/system/rich/rich_files/rich_files/000/001/385/original/14%20Oversigt%20filtreret.jpg)

Oversigten kan filtreres ved at skrive begyndelsen på den søgestreng der søges efter. Der kan også filtreres på status. Oversigten kan også sorteres på forskellige måder ved at klikke på linket med kolonne-overskriften.
Oversigten kan også filtreres ved at vælge en status. Vælges status ”Aktiv” vises kun manuelle tilretninger.
Der kan vælges et antal søgestrenge og udføres handlinger på dem, enten sletning eller redigering.
 

### Smart Search indstillinger

Indstillingerne findes under Indstillinger -> Ding -> Ting Smart Search /admin/config/ding/ting\_smart\_search. Det kræver administrator-rettigheder at ændre disse indstillinger.

Ønsker du ikke at automatisk Smart Search skal være aktiveret, kan den deaktiveres her ved fjernelse af flueben i ”Activate automatic smart search”.
For at Smart Search skal fungere, skal der her angives links til hvor datafilen skal hentes fra, samt til hvor data omkring de mest brugte søgninger skal hentes fra.
Under ”Master server for automatic smart search” skal der stå "https://smartsearch.dandigbib.org/data/autodata.txt"; og under ”Webtrekk statistics feed” skal der stå "https://smartsearch.dandigbib.org/data/searchdata.csv":
![](/system/rich/rich_files/rich_files/000/001/642/original/15%20Settings.jpg)

### Eksport/import

Der er herfra også muligt at eksportere alle de manuelle tilretninger af søgninger som er foretaget på dit bibliotek. Vil du se en oversigt over alle dine tilretninger inden du eksporterer dem, klik da på ”View local smart search records”, hvilket fører dig til oversigten, som beskrevet ovenfor. Filtrer på status ”Aktiv” for at se alle aktive manuelle tilretninger.

![](/system/rich/rich_files/rich_files/000/001/387/original/16%20View%20local%20records%20export.jpg)

Klik da på ”Export smart search records” for at eksportere. Dette resulterer i at en datafil i JSON-format gemmes på computeren. Alle de tilretninger som har status aktiv bliver eksporteret. Denne fil kan sendes til andre biblioteker, som kan importere den ved hjælp af feltet ”IMPORT SMART SEARCH RECORDS” nedenunder, ligesom du på samme måde kan hente andre bibliotekers tilretninger.
**Bemærk! Hvis du importerer et sæt af tilretninger, vil de overskrive dem, du selv har foretaget, hvis der er tilretninger af samme søgestrenge.**

Det betyder, at hvis du gerne vil sikre, at dine egne tilretninger bevares, skal du gemme dem lokalt på din egen computer, inden du importerer tilretninger fra et andet bibliotek. På den måde kan du efter import af andres tilretninger overskrive dem, der er gengangere fra dine egen, med import af din egen fil, hvorved dine egne tilretninger bevares.

Upload service til Cover service

---

Funktionen gør det muligt for hjemmesidens administratorer, lokal administratorer og lokale redaktører at tilføje nye forsider til materialer direkte fra hjemmesiden.

Det er vigtigt at være opmærksom på, at alle forsider, der uploades, straks vil blive tilgængelige på alle bibliotekshjemmesider. Dermed bliver dit lokale arbejde til gavn for alle dine kolleger i hele landet. Det forpligter til gengæld også, og derfor er det ikke tilladt at uploade forsider, før mab har læst brugsbetingelserne. 

[Læs brugsbetingelserne her](http://detdigitalefolkebibliotek.dk/sites/default/files/ddb_cover_service_-_brugsbetingelser_1.pdf).

[Læs mere om Cover service her.](http://www.danskernesdigitalebibliotek.dk/loesninger-og-projekter/i-brug-paa-biblioteket/cover-service/)

Log ind som administrator, lokal administratorer eller lokal redaktør

**Trin 1 - find materialet** 
Fremsøg det materiale, du vil uploade en forside til, og klik på knappen "Upload forside" på enten værk- eller materialevisningssiden

_eller_

Åben “Indstillinger ->Materialer ” (Sti: /admin/config/ting/ddb\_cover\_upload) og fremsøg det materiale, du vil uploade en forside til.
Klik på knappen "preview" for at få vist de bibliografiske oplysninger om materialet,så du kan sikre det, det er det rigtige materiale, du har søgt frem. "Preview" viser endvidere om der allerede er et forsidebillede på materialet. Klik på knappen "Næste"

**Trin 2  - find forsidebilledet på din pc**
Klik på lmappen "Upload new image" og find filen på dit lokale drev. Klik på "Åbn" Herefter vises den forside, du vil uploade, så du kan verificere, at der er tale om det rigtige billede.
Klik en gang til på knappen "Upload new image" OBS! Når du først har klikket vil billedet blive uploaded til Cover service og derefter straks være tilgængelig på alle bibliotekshjemmesider.

**Trin 3 - bekræftelse**
Viser at billedet bliver uploaded, samt bekræftelse på, når det er sket. 

**Vis uploadede forsider**
Under fanebladet "List uploaded covers" (sti: /admin/config/ting/ddb\_cover\_upload/list) vises en oversigt over alle de forsidebilleder, dit bibliotek har lagt op. 

**Slet uploadede forsider**
I oversigten "List uploaded covers"  under fanebladet af samme navn (sti: /admin/config/ting/ddb\_cover\_upload/list) er der ud for hvert forsidebillede et link til at slette billedet fra Cover service igen. Vær opmærksom på at de enkelte hjemmesider casher billedet, så der kan gå en rum tid, før det er er væk i brugergrændefladerne.

 

Subsearch
---------

Subsearch-modulerne er 3 funktioner, der giver jeres brugere hjælp, hvis de ikke er tilfredse med resultaterne fra deres søgning: 

1. Mente-du (subsearch\_suggestions)
2. Forslag fra bibliotek.dk (subsearch\_bibdk)e
3. Oversatte forslag (subsearch\_translate)

### **De enktelte moduler**

#### ”mente-du” (subsearch\_suggestions)

Modulet ”mente-du” sammenligner søgetermen fra brugerens søgning med ord fra ortograf-servicen - og hvis der er noget, der ligger sprogligt tæt på, som giver et bedre søgeresultat, foreslås dette for brugeren.

Eksempel:
![](/system/rich/rich_files/rich_files/000/001/595/original/didyoumean%20hobitten.jpg)

I tilfælde af, at brugerens søgning giver 0 hits, udføres den sekundære søgning blot, uden at brugeren spørges, såfremt de øvrige triggers er opfyldt.

Eksempel:
![](/system/rich/rich_files/rich_files/000/001/597/original/didyoumeanredirect.jpg)
 

#### ”Forslag fra bibliotek.dk” (subsearch\_bibliotek.dk)

I dette modul foretages brugerens søgning i bibliotek.dk samtidig med at den foretages på den lokale hjemmeside. Hvis kriterierne opfyldes præsenteres brugeren for et antal resultater fra bibliotek.dk.

Eksempel:
![](/system/rich/rich_files/rich_files/000/001/491/original/Forslag%20fra%20bibliotek.dk.jpg)

#### "Oversatte forslag" (subsearch\_translate)

Oversætter brugerens søgning til engelsk vha. google translate, og foreslår dette,  hvis kriterierne er opfyldt.
Biblioteker, der hverken abonnerer på Masterfile eller nogle Gale-baser har nok ikke samme glæde af ”Oversatte forslag”, som dem der har.

Eksempel:
![](/system/rich/rich_files/rich_files/000/001/492/original/Oversatte%20forslag.jpg)

### Konfiguration af Subsearch

Når man konfigurerer subsearch-modulerne, gælder det om at finde en balance, så brugerne hverken vises forslag for ofte eller for sjældent – og det vil variere alt efter bibliotekets katalog og brøndprofil. Et biblioteker med relativt få fysiske materialer, og som ikke har ret mange kilder slået til i brønden, skal vælge værdier, der udløser forslag oftere, end relativt større biblioteker.

Udfyld felterne i subsearch-moduler på /admin/config/ding/subsearch, som beskrevet nedenfor.I kan finde anbefalede konfigurationer i skemaet på baggrund af to faktorer:

1. Størrelsen på jeres katalog
2. Om I har Masterfile aktiveret eller ej

Foretag denne søgning for at afklare det første spørgsmål:

term.title=\* not term.acsource=masterfile

En lille katalog er under 500.000 resultater, en mellemstor er mellem 0,5 og 1,5 million, og en stor er over 1,5 millioner.
Dermed kan I finde de anbefalede konfigurationer i skemaet herunder:

Modul

Konfiguration

Uden Masterfile

Med Masterfile

 

 

Stor

Mellem

Lille

Stor

Mellem

Lille

mente-du (subsearch\_suggestions)

Levenshtein-afstand

3

3

3

3

3

3

Højeste antal resultater, der udløser sekundær søgning

18

15

12

18

15

12

Faktoren mellem antallet af resultater fra den primære og den sekundære søgning

1.1

1.1

1.1

1.1

1.1

1.1

Forslag fra bibliotek.dk (subsearch\_bibdk)

Højeste antal resultater fra primær-søgningen for at vise forslag

200

250

250

200

250

250

Faktoren mellem nonfiktion og fiktion.

1.5

1.5

1.5

1

1

1

Laveste antal resultater fra sekundær-søgning

4

4

4

4

4

4

Faktoren mellem antallet af resultater fra primær-søgningen og fra sekundær-søgningen

1.4

1.2

1

1.7

1.5

1.4

Oversatte forslag (subsearch\_translate)

Faktoren mellem nonfiktion og fiktion.

1

1

1

2.5

2.5

2.5

Faktoren mellem antallet af resultater fra primær-søgningen og fra sekundær-søgningen.

1

1

1

2

2

2

BEMÆRK: Dette er kun anbefalede konfigurationer; I opfordres til at eksperimentere med det selv, læs meget mere her: https://platform.dandigbib.org/projects/ddb-cms/wiki/Vejledning\_i\_subsearch
BEMÆRK: Konfiguration foretages på /admin/config/ding/subsearch
BEMÆRK: Husk at benytte punktum, ikke komma, når du skal indsætte decimaltal.
BEMÆRK: For at Mente-du (subsearch\_suggestions) kan fungere, skal ortograf-servicen være aktiveret. Det betyder, at feltet Autocomplete URL skal være udfyldt med https://ortograf.dbc.dk/ortograf/suggest under “Indstillinger » Opensearch » Opensearch search autocomplete settings" (Sti: admin/config/opensearch/autocomplete), jf https://platform.dandigbib.org/projects/ddb-cms/wiki/Ddb-cms-manual\_grundl%C3%A6ggende-ops%C3%A6tning\_next-version#Autofuldf%C3%B8rsel-med-Ortograf-servicen

### Google Cloud Translation API URL og Google Cloud Translation API key

Gå ind under /admin/config/ding/subsearch/translate

I feltet “Google Cloud Translation API URL” skal der blot stå https://www.googleapis.com/language/translate/v2

For at udfylde feltet ”Google Cloud Translation API key”, skal du have en nøgle, og for at få sådan en, skal du oprette en google-konto med et betalingskort tilknyttet. Udgiften vil variere alt efter brugen af modulet, men eftersom der afregnes med 20 USD pr million karakterer, og eftersom den gennemsnitlige søgestreng er på 13 karakterer, og der i gennemsnit foretages omkring 25.000.000 søgninger årligt på landsplan, så vil den gennemsnitlige årlige udgift pr kommune være på knap 400 kroner – men det er så kun under forudsætning af at alle søgninger oversættes, hvilket jo langtfra er tilfældet, da antallet at hits fra primærsøgningen tjekkes mod konfigurationen, inden søgestrengen overhovedet oversættes. Det vil derfor under alle omstændigheder være helt ubetydeligt - men der skal tilknyttes et betalingskort.

Følgende beskrivelse er udført med det forbehold, at fremgangsmåden kan ændre sig; allerede i det år, projektet omkring subsearch\_translate har været i gang, har det været nødvendigt at opdatere vejledningen 2 gange, idet Google har ændret den måde, man skal generere en nøgle på.

Det kan derfor ikke udelukkes, at nedenstående atter er forældet, når du læser det - i så fald anbefales du at forsøge at google dig til en nyere vejledning. Alternativt kan du kontakte Det Digitale Folkebibliotek, så vil vi naturligvis også gerne forsøge at hjælpe dig.
 

1.    Mens du er logget ind på en konto med et betalingskort tilknyttet, gå til https://console.cloud.google.com/getting-started 
2.    Klik ja til ”Terms and Conditions”
3.    Klik på “Billing” til højre
4.    Klik på ”Add Billing Account”
5.    Klik ja til ”Terms and Conditions”
6.    Klik på “Start my free trial”
7.    Derpå skal du bekræfte at du er dig, metoden varierer alt efter betalingskortet
8.    Du har nu accepteret, at Google må trække penge på kortet
9.    Gå derpå til https://cloud.google.com/translate/
10.    Scroll ned til ”Enable the API” og klik på dén
11.    Øverst er der en dropdown med ”Select a project” – vælg ”My first project”
12.    Vælg også ”My first project” i dropdown’en lige nedenunder
13.    Øverst til højre står der noget med ”Free trial status” og en knap med ”Activate”. Klik på den.
14.    Bekræft at du vil opgradere
15.    Klik ”Go to credentials”
16.    Under “Find out what kind of credentials you need” står der “If you wish you can skip this step and create an API key, client ID, or service account”. Klik på “API key”
17.    Klik på “Create” nederst
18.    Så kommer du til en skærm, hvor der er en afdeling med API Keys, og herunder finder du din nye nøgle. Klik på symbolet ![](/system/rich/rich_files/rich_files/000/001/593/original/Kopiersymbol.jpg) for at kopiere den.
19.    Indsæt den i feltet ”Google Cloud Translation API key” under /admin/config/ding/subsearch/translate

Hvis du har brug for at fejlsøge, og du gerne vil tjekke om din nøgle overhovedet virker, kan du prøve dette link, hvor du erstatter \[INDSÆT NØGLE HER\]  med din nøgle: https://www.googleapis.com/language/translate/v2?key=\[INDSÆT\_NØGLE\_HER\]&source=da&target=en&q=krystaller 

Hvis din nøgle virker, skal den returnere _"translatedText": "crystals"_

Oversættelser
--------------

De fleste tekster i grænsefladen i DDB CMS kan oversættes ved at bruge den indbyggede oversættelsesfunktion.

### Oversæt tekst i grænsefladen.

1. Åbn “Indstillinger - > Oversættelser (under afsnittet “Region og sprog” (Sti: https://bibliotekets-hjemmesideadresse.dk/admin/config/regional/translate/translate).
2. Vælg fanebladet “Oversæt”.
3. Fremsøg den tekststreng du ønsker at oversætte. Bemærk at du får forskellige søgeresultater afhængig af, om du skriver store eller små bogstaver i søgningen.
4. Vælg “Rediger” ud for den tekststreng, der ønsker at oversætte.
5. Indsæt din oversættelse.
6. Klik på knappen “Gem oversættelser”.

Lokale oversættelser overskrives ikke ved opdatering af den samme tekststreng i senere versioner af DDB CMS.

### Import og eksport af oversættelsesfiler

Det er muligt at eksportere oversættelserne fra DDB CMS med henblik på backup eller gennemgang af oversættelserne i eksterne værktøjer, der er særligt egnede til det job. Man kan f.eks. bruge POedit (http://poedit.net/) eller et lignende tekstbehandlingsprogram til at redigere oversættelsesfilerne. Når man eksportere oversættelserne i Drupal gemmes de i filformatet PO, deraf navnet POedit.

DDB CMS har to grupper af oversættelser repræsenteret ved "Indbygget grænseflade" og "Felter". Begge skal enten eksporteres eller importeres efter hinanden.

Oversættelsen er inkluderet i DDB CMS, men løbende opdateringer af master oversættelsen kan hentes fra:
[DDB CMS indbygget grænseflade](https://www.dropbox.com/s/sa6stp287nltoph/DDB%20CMS%20built-in%20interface.po?dl=0)
[DDB CMS felter](https://www.dropbox.com/s/9rey21t6fi4xwz9/DDB%20CMS%20fields.po?dl=0)
[DDB CMS metatags](https://www.dropbox.com/s/xs70bkn0qgtxrlg/DDB%20CMS%20metatags.po?dl=0)

### Eksporter oversættelser.

1. Åbn “Indstillinger - > Oversættelser -> Eksportér” (Sti: admin/config/regional/translate/export).
2. Vælg “Indbygget grænseflade” eller “Felter” under “Eksportér oversættelse”.
3. Tryk på knappen “Eksportér”.

### Importer oversættelser.

1. Åbn “Indstillinger - > Oversættelser -> Importér” (Sti: admin/config/regional/translate/import)
2. Vælg under feltet “Sprogfil” den PO-fil for “Indbygget grænseflade” eller “Felter”, der skal importeres.
3. Vælg “Indbygget grænseflade” eller “Fields” afhængig af hvilken gruppe af oversættelser, du ønsker at importere.
4. Vælg under “Tilstand” radioknappen "Eksisterende strenge og flertals-formatet bevares, kun nye strenge tilføjes." for at undgå at overskrive eksisterende lokale tilpasninger af oversættelserne. Bemærk at nye oversættelser overskriver eksisterende oversættelser hvis du vælger radioknappen "Tekststrenge i den uploadede fil erstatter de eksisterende, mens nye tilføjes. Flertalsformatet opdateres."
5. Tryk på knappen “Importér”.

Eksport og udstilling af redaktionelt indhold til eksterne systemer
-------------------------------------------------------------------

### Nyheder arrangementer og karuseller til APP'en

APP'en Biblioteket trækker nyheder, arrangementer og information om forsidekarusellen direkte fra DDB CMS.

Det gør den fra "Ding app content rss" og "Ding app variables" modulerne som begge er aktiverede og ikke kræver konfiguration.

De to moduler kan testes under.

* Arrangementer: \[jeres staging-site URL\] /ding-redia-rss/event
* Nyheder: \[jeres staging-site URL\] /ding-redia-rss/news
* Materialekarruseller: \[jeres staging-site URL\] /ding/variables

### CMS Content til Mobilesearch (ding\_mobilesearch)

Biblioteker på Redaktørhostingplanen får automatisk modulet aktiveret og konfigureret.

Biblioteker på Webmaster- og Programmørhostingplanen skal:

1. kontakte DBC via https://kundeservice.dbc.dk og bede om API nøglen
2. Logge ind med en administrator og indsætte https://cmscontent.dbc.dk/ i feltet "WS URL" og API nøglen i feltet "Nøgle" under Indstillinger > Ding > Content export > plugins (Sti: /admin/config/ding/mobilesearch/content-export/plugin).
3. ændre WS URL til https://cmscontent-stg.dbc.dk/ for oprettelse af indhold under tekst på development- og stagingmiljøer.

![](/system/rich/rich_files/rich_files/000/000/104/original/2017-10-05%2013_05_12-Content%20export%20_%20%E2%80%93%20Google%20Chrome.png)

Manglende konfiguration af modulet vil resultere i fejlmeddelelsen "Problem connecting to the REST service. We have unchecked your "Push to Mongo" flag. Please check your [indstillinger](https://hvidovre-dev.ddbcms.dk/admin/config/ding/mobilesearch/content-export/plugin)." eller på dansk "DDB CMS kunne ikke få forbindelse til CMS Content servicen. Markeringen ved Send til CMS Content er fjernet. Undersøg venligst modulets indstillinger."

Nye nyheder, arrangementer og åbningstider overføres automatisk til den fælles app via CMS Content servicen.

Man kan fravælge at en nyhed eller et arrangement vises i app'en, ved under fanen Flag i bunden af siden, at fjerne fluebenet i "Send til CMS Content".

NB. Ding\_mobile search modulet benyttes til at udstille indhold via Open platform CMS endpointet.

### Services modulet

Services modulet gør det muligt at udstille indhold, hvilket pt. omfatter nyheder og arrangementer, fra DDB CMS som en web service.

Når følgende moduler skal aktiveres:

1. Ding\_services\_news; Ding\_services\_events (Medvirker aktivering af modulerne #Services" og "Services Views")
2. rest\_server (Medvirker aktivering af modulet "Services")

Følgende endpoints eksponerer indholdet:

* /services/news\_list
* /services/event\_list

NB. Services modulet benyttes ikke pt. aktivt.

E-resursemodul
--------------

### Opret brugernes adgangsmuligheder for de enkelte resurser.

* Klik på Administration\_Struktur-Taksonomi
* Klik på E-resource availability![](e-resursemodul_dump2.png)
* Tilføj ord. F. eks.
  * Adgang fra biblioteket
  * Adgang hjemmefra
  * Fri adgang![](e-resursemodul_dump3.png)

### Opret kategorier for ressourcerne

* Klik på Administration\_Struktur-Taksonomi
* Klik på E-resource category
* Tilføj ord. F. eks.
  * Aviser
  * Film
  * Magasiner![](e-resursemodul_dump4.png)

### Opret den enkelte resurse

* Klik på tilføj indhold og vælg E-resource som indholdstype![](e-resursemodul_dump5.png)
* Tilføj indhold til de obligatoriske felter![](e-resursemodul_dump7.png)

Logoer i beskåret tilstand kan findes på [https://centralbibliotek.dk/post/nye-logo-st%C3%B8rrelser-p%C3%A5-ddb-cms-e-resursemodulet](https://centralbibliotek.dk/post/nye-logo-st%C3%B8rrelser-p%C3%A5-ddb-cms-e-resursemodulet) (udarbejdet udført af Rosa Andersen).

Oversigtsvisning af resurserne https://upgrade-fbs.ddbcms.dk/e-materialer![](e-resursemodul_dump8.png)

Visning af den enkelte resurse (“læs mere”) inkl. relateret materiale![](e-resursemodul_dump9.png)

### Forankring af e-resursemodulet i (hoved)menustrukturen

* Klik på Hjem » Administration » Struktur » Menuer » Hovedmenu
* Klik på tilføj link
* Vælg titel, eks.: E-resurser
* I feltet Sti, skrives: e-materialer

### Ændring af teksten på e-resurse oversigtsvisningssiden

Defaultteksten på /e-materialer siden kan ændres under Indstillinger > Ding > eresurser (Sti: /admin/config/ding/eresource)

Som låner ved Mariagerfjord Bibliotekerne har du fri adgang til en række digitale tjenester som e-bøger, lydbøger, magasiner, temasider og film.
De fleste tjenester kan anvendes hjemmefra. For nogle af dem kræves, at du er bosat i Mariagerfjord Kommune, er oprettet som låner på biblioteket og har en pinkode.

![](e-resursemodul_dump10.png)

Webstatistik
------------

### Mapp (tidl. WebTrekk)

Mapp er folkebibliotekernes fælles løsning til opsamling og analyse af webstatistik. Mapp giver dels mulighed for lokalt at tilgå egne statistiske data, dels leverer systemet statistik til Danmarks Biblioteksindeks: http://danmarksbiblioteksindex.dk/, som samler udvalgte webstatiske nøgletal fra folkebiblioteker i hele Danmark.

For at data fra hjemmesiden sendes til Mapp forudsættes konfiguration af Webtrekkmodulet i DDB CMS. Det er hensigtsmæssigt at konfigurere Webtrekkmodulet før hjemmesiden sættes i drift, så det er muligt at se brugerstatistik fra hjemmesiden fra starten.

For de flestes vedkommende er dette sat op automatisk, men det er en god ide at kontrollere om opsætningen er korrekt alligevel.

Indstillingen af modulet sker under “Indstillinger -> DING -> WebTrekk” (/admin/config/ding/webtrekk )

De forskellige felter herunder skal udfyldes på følgende måde:

* Tracking domæne: responder.wt-safetag.com
* Tracking ID: 476651662471322

Arrangementer
-------------

### Arrangementer: Konfigurér om prisen skal være i euro i stedet for kroner.

1. Åbn “Indstillinger -> sektionen “Begivenheder” -> Ding event settings
2. Marker checkboksen “€”.
3. Klik på knappen “Gem indstillinger”.
   Ved oprettelse af en begivenhed (aka arrangement) er det muligt at angive en pris. Prisen er som udgangspunkt i kroner. Ønsker du at ændre møntfoden til euro, gøres følgende:
4. Åbn “Indstillinger -> Event currency (under afsnittet “Begivenheder”)
5. Marker checkboksen “€”.
6. Klik på knappen “Gem indstillinger”.

### Arrangementer: Konfigurér antal arrangementer på forsiden

Det er muligt at konfigurere hvor mange arrangementer der maksimalt skal vises på forsiden. (kræver rollen admin eller lokaladmin)

1. Gå til /admin/config/ding\_event/settings eller Åbn “Indstillinger -> sektionen “Begivenheder” -> Ding event settings
2. Skriv det ønskede tal i "Maximum number of events on the frontpage"
3. Klik på knappen “Gem indstillinger”.

### Billetbestilling til arrangementer med Place2book

_[Læs også om Place2book i manualen Struktur og indhold.](https://platform.dandigbib.org/projects/ddb-cms/wiki/Ddb-cms-manual_struktur-og-indhold_next-version#Place2Book-Send-en-begivenhed-arrangement-til-Place2Book)_

Place2book er et eksternt online billetsystem, der anvendes af mange biblioteker til at modtage tilmeldinger- og sælge billetter til arrangementer. Desuden er det via Place2Book muligt at eksportere oprettede arrangementer til www.kultunaut.dk.

Place2Book opkræver i forbindelse med salg af billetter via tjenesten et mindre billetgebyr, der som udgangspunkt betales af køberen. Der vil desuden figurere reklamer på billetterne. Til gengæld er det for arrangøren som udgangspunkt gratis at anvende tjenesten. Information om andre prismodeller og aktuelle priser findes på place2book.com.

DDB CMS indeholder et Place2Book-modul, som giver mulighed for at integrere til tjenesten. For at integrere til Place2Book forudsættes, at du har oprettet en arrangørprofil på place2book.com. Når der oprettes begivenheder i DDB CMS, der kræver tilmelding/betaling, fungerer integrationen til Place2Book ved at der automatisk bliver oprettet et tilsvarende arrangement i Place2Book. På den pågældende begivenhed på DDB CMS linkes der videre til arrangementet på Place2Book, hvor tilmelding og evt. betaling håndteres.

For at aktivere Place2book-modulet skal biblioteker, der er tilmeldt redaktørhostingplanen oprette en sag på opgaven hos DBC via http://kundeservice.dbc.dk. Webmasterbiblioteker sørger selv for at aktivere og konfigurere modulet. Fremgangsmåden for grundlæggende konfiguration er beskrevet nedenunder:

### Konfigurér Place2book

1. Åbn “Indstillinger > Place2book (under afsnittet “Ding”)” (Sti: admin/config/ding/place2book).
2. I skal kontakte Place2book på bibliotek@place2book.com og bede om en API nøgle.
3. Indtast jeres unikke nøgle til Place2Book i feltet “Place2Book authorisation token” under fanen “PLACE2BOOK INDSTILLINGER”. Den fungerer som unik identifikator for den pågældende konto.
4. Klik på knappen "Gem indstillinger".
5. Naviger til fanen STANDARDER (Sti: /admin/config/ding/place2book/defaults)
6. Indstil Default event maker, som er den filial der skal vælges som default ved oprettelse af nye arrangementer (typisk hovedbiblioteket).
7. Markér Vedligehold kopi hvis begivenheder som default skal overføres til Place2book
8. Markér Kultunaut eksport, hvis begivenheder som default skal overføres til Kultunaut
9. Markér Passivt arrangement, hvis begivenheder som default ikke skal påføres en knap til billetsalg, f. eks. mhp. at sende begivenheder til Kultunaut uden at benytte Place2book, eller for at holde regnskab.
10. Angiv det maksimale antal deltagere til begivenheder, der som default skal indsættes på nye begivenheder.
11. Oplys navnet på den billettype der som default skal indsættes på nye begivenheder f. eks. Adgang, Børn eller Voksne.
12. Naviger til fanen MAPPINGS (Sti: /admin/config/ding/place2book/mappings)
13. Vælg for hver filial den tilsvarende event maker som er oprettet i Place2book administrationsgrænsefladen.
14. Vælg for hver event target taksonomi term (Se /admin/structure/taxonomy/event\_target) den tilsvarende Kultunaut age group.
15. Vælg for hver event category taksonomi term (Se /admin/structure/taxonomy/event\_category) den tilsvarende Kultunaut export category.

### Migrering af arrangementer til nyt API (kun relevant for release 31)

1. Redaktørbiblioteker skal have en API nøgle af DBC når I kontakter dem for at aftale et tidspunkt for opgraderingen. Webmaster- og programmørbiblioteker skal henvende sig til Place2Book på [api@place2book.com](mailto:api@place2book.com) og få udleveret den nye API-nøgle
2. Naviger til /admin/config/ding/place2book og indstil API key til nyt API\*.
3. Naviger til /admin/config/ding/place2book/defaults og indstil Default event maker.
4. Naviger til /admin/config/ding/place2book/mappings og lav event maker mapping og kultunaut kategori/målgruppe mapping.
5. Når ovenstående er gennemført, foretager man migrering: Klik på  knappen “Start migration” under /admin/config/ding/place2book/migrate.
6. Når migreringen er foretaget, skal I tjekke, at jeres arrangementers billetlink-statusser er korrekte. Skulle der være arrangementer, der ikke er blevet migreret, vil de fremgå af en oversigt inde på /admin/config/ding/place2book/migrate. Det kan f.eks. være tilfældet såfremt et arrangement er slettet ovre i Place2Book, men ikke er blevet slettet i Jeres DDB CMS.
7. For at godkende migreringen endeligt klikker I på “Approve migration. Når først I har klikket på approve, er der ingen vej tilbage. Gamle Place2Book data bliver slettet og man kan ikke migrere længere.

Spørg Biblioteksvagten
-----------------------

Med "Spørg Biblioteksvagten" kan lånerne sende spørgsmål til
Biblioteksvagten via en spørgeformular på hjemmesiden. Biblioteksvagten besvarer herefter spørgsmålet eller videresender det til lokal besvarelse. Besvarelsen kan foregå via chat, sms eller e-mail. Spørgeformularen vises i et overlay på hjemmesiden:

Alle biblioteker kan benytte Biblioteksvagtens spørgefunktion uden vederlag.

Brugerne kan aktivere spørgefunktonen fra enten en knap ”Spørg Biblioteksvagten”, der vises nederst i DDB CMS vinduet eller fra et link i tekster eller billeder på sitet.

På http://biblioteksvagten.dk/om.asp?artid=21 findes bannere og knapper, der kan bruges som henvisning til Biblioteksvagten.

Har du spørgsmål som vejledningen nedenunder ikke besvarer, kan du kontakte Biblioteksvagtens webmaster Anders Nielsen, bibani@herning.dk.

### Aktivér spørgefunktionen

Du skal igennem følgende trin for at aktivere spørgefunktionen:

* Biblioteker, der er tilmeldt redaktørhostingplanen skal kontakte http://kundeservice.dbc.dk for at få aktiveret Biblioteksvagten (ask\_vopros) modulet.
* Send identifikationsnummer (se afsnittet “Muligheder under Biblioteksvagten/Ask Vopros” nedenunder) sammen med biblioteksnavn til Anders Nielsen, bibani@herning.dk. Biblioteksvagtenen vil herefter godkende, at der modtages spørgsmål fra den pågældende hjemmeside.
* Konfigurér spørgefunktionen i DDB CMS (se nedenunder). For at kunne foretage indstillingerne skal du være logget ind som administrator.

### Konfigurér spørgefunktionen i DDB CMS:

* Åbn ”Indstillinger > Ask Vopros” (Sti: admin/config/services/ask\_vopros)
* Udfyld de forskellige felter efter behov (se beskrivelse af de enkelte felter i afsnittet “Muligheder under “Biblioteksvagten/Ask Vopros” nedenunder).
* Klik på knappen “Gem indstillinger”.

### Muligheder under “Biblioteksvagten/Ask Vopros”:

Nedenfor er en kort beskrivelse af felter og konfigurationsmuligheder under “Biblioteksvagten/Ask Vopros”:

**Identifikationsnummer:** Feltet er udfyldt på forhånd. Identifikationsnummeret består af landekode og biblioteksnummer og skal opgives i forbindelse med aktivering af Biblioteksvagten på det pågældende site.

**Vopros URL:**
Feltet er udfyldt på forhånd og skal ikke ændres. Når lånerne stiller et spørgsmål til Biblioteksvagten sendes spørgsmålene til denne adresse.

**Lokal e-mail:**
“Lokal e-mail” skal udfyldes med bibliotekets primære e-mailadresse. Det er den adresse Biblioteksvagten vil bruge til at sende spørgsmål videre til, hvis det er et spørgsmål, der kun eller bedst kan besvares lokalt.

**Override tab color:**
Farven på fanebladet kan ændres. Den valgte farve overskriver den grønne standardfarve. Farven skal angive som HEX-værdi.

**Definér højre margin:**
“Definér høre margin” udfyldes, hvis knappen nederst på siden skal flyttes i forhold til højre margin af browservinduet. Det kan være hvis knappen netop er i vejen for et lokalt telefonnummer el. lign. Vær opmærksom på at tjekke at den valgte indstilling også fungerer, når siden tilgås fra en mobil.

**Standardmetode til besvarelse:**
Du vælger selv om spørgeformularen skal åbnes med chat, e-mail eller SMS som foretrukken spørge/svar-form. Biblioteksvagten anbefaler, at I vælger ”E-mail”.

**Vis blok på bestemte sider:**
Her kan du vælge hvor spørgeknappen skal vises.
Hvis du vælger ”Alle sider undtagen de nævnte” bliver knappen vist på alle sider.
I de fleste tilfælde vil det være hensigtsmæssigt at ekskludere siderne: media/browser\* da spørgeknappen her ikke har nogen funktion og ofte vil genere.
Hvis I vælger ”Kun de viste sider” skal I angive, hvilke sider eller grupper af sider, der skal vise spørgeknappen.

Nederst på indstillingssiden er angivet jeres specifikke URL, der skal anvendes, hvis I vil åbne spørgeboksen fra et link på en tekst eller et billede. Linket indeholder de nødvendige oplysninger til Biblioteksvagten, så det fremgår, hvor spørgsmålet kommer fra og den lokale kontakt-e-mail.

eKurser
-------

EKurser.nu er et site, som tilbyder et bredt udvalg af e-læringsforløb produceret på danske folkebiblioteker. De kurser, du finder på eKurser.nu handler om emner som folkebibliotekerne traditionelt vejleder i på it-området. Det vil sige kurser i selvbetjeningsløsninger fra det offentlige, bibliotekernes egne nettjenester, brug af computer, søgning på internettet og andre muligheder på internettet, som kan have almen interesse.

Det er muligt at få vist kurser fra eKurser.nu direkte i DDB CMS via søgninger og relationer på materialer og på en samlet kursusoversigter.

Nedenfor ses illustration af hvordan et kursus vises direkte på biblioteksposten. Kursusindholdet vises under afsnittet "Materialets Indhold". Bemærk at knappen "Se online" på posten stadig linker til kurset på ekurser.nu.

![](/system/rich/rich_files/rich_files/000/001/312/original/ekurser_materialevisning.png)

Nedenfor ses illustration af kursusoversigten:

![](/system/rich/rich_files/rich_files/000/001/311/original/ekurser.png)

### Konfiguration af eKurser for Webmaster- og programmørbiblioteker

Fremgangsmåden for at få vist kursusoversigten er for webmaster- og programmørbiblioteker følgende. Bemærk at biblioteker med redaktørhostingplanen skal følge vejledningen nedenunder.

1. Aktivér kilden eKurser som "søgning" (og evt. som "Relationer") i VIP (se evt. afsnittet “Opret og konfigurer en brøndprofil” for mere info om VIP-konfiguration og brøndprofiler).
2. Aktiver modulet "Ding eKurser".
3. Gå ind på (Sti: https://bibliotekets-hjemmesideadresse.dk/ekurser) og bekræft at kursusoversigten er tilgængelig.
4. Opret evt. et menupunkt der linker til kursusoversigten ved at følge vejledningen under http://platform.dandigbib.org/projects/ddb-cms/wiki/Manual\_til\_DDB\_CMS#Sådan-tilføjer-du-et-menupunkt-til-hovedmenuen

Fremgangsmåde for at få vist et kursus direkte på biblioteksposten er for webmaster- og programmørbiblioteker følgende:

1. Aktivér kilden eKurser som "søgning" (og evt. som "Relationer") i VIP (se evt. afsnittet “Opret og konfigurer en brøndprofil” for mere info om VIP-konfiguration og brøndprofiler).
2. Aktivér modulerne "Add oEmbed support to Ting objects", "oEmbed", "oEmbed Embed.ly" og "oEmbed Provider"

### Konfiguration af eKurser for redaktørbiblioteker

Fremgangsmåden for at få vist kursusoversigten på (Sti: https://bibliotekets-hjemmesideadresse.dk/ekurser) er følgende:

1. Aktivér kilden eKurser som "søgning" (og evt. som "Relationer") i VIP (se evt. afsnittet “Opret og konfigurer en brøndprofil” for mere info om VIP-konfiguration og brøndprofiler).
2. Opret et menupunkt der linker til kursusoversigten ved at følge vejledningen under http://platform.dandigbib.org/projects/ddb-cms/wiki/Manual\_til\_DDB\_CMS#Sådan-tilføjer-du-et-menupunkt-til-hovedmenuen
3. Gå ind på (Sti: https://bibliotekets-hjemmesideadresse.dk/ekurser) og bekræft at kursusoversigten er tilgængelig.

Fremgangsmåden for at aktivere visning af eKurser direkte i biblioteksposterne er følgende:

1. Aktivér kilden eKurser som “Søgning” (og evt. som “Relationer”) i VIP under korrekt brøndprofil (se evt. afsnittet “Opret og konfigurer en brøndprofil” for mere info om VIP-konfiguration og brøndprofiler).
2. Lav en prøvesøgning på tilgængelige e-kurser og tjek at kurserne vises direkte i posten.

Artikler fra Infomedia
----------------------

For deaktivering af Infomedia modulet skal feltet ting\_infomedia slettes fra admin/structure/ting\_object/fields. NB. det kræver administratorrettigheder, hvilket for Redaktørhosrtingplansbiblioteker betyder at man skal kontakte DBC via https://kundeservice.dbc.dk.

Administration
--------------

### Tilpas "siden blev ikke fundet".

Når brugeren sender en forespørgsel på en webside til DDB CMS, som ikke eksisterer, vil brugeren automatisk blive omdirigeret til en side, der fortæller, at den forespurgte side ikke findes.

Som udgangspunkt henviser DDB CMS i disse tilfælde til følgende side (sti: https://bibliotekets-hjemmesideadresse.dk/siden-blev-ikke-fundet) med systemstien (sti: https://bibliotekets-hjemmesideadresse.dk/node/1). Denne side er defineret som “Standard 404-side (ikke fundet)” under (Sti: admin/config/system/site-information).

Teksten på “Siden blev ikke fundet” skal tilrettes så den passer til dit bibliotek (bl.a. henvises der som udgangspunkt til Odense Centralbibliotek). Da siden er en helt almindelige side-indholdstype, kan du redigere den på sædvanlig vis, når du er logget ind som administrator.

Skift kodeordet til lokaladministrator
--------------------------------------

Skift kodeord:

1. Log ind med din ladmin-bruger (lokaladministrator) og tryk på “Hej ladmin” øverst til højre i administrationsmenuen.
2. Tryk på fanebladet “Redigér brugerprofil”.
3. Indtast dit nuværende password i feltet ”Nuværende adgangskode”.
4. Indtast din nye adgangskode i feltet ”Adgangskode” og gentag det i feltet ”Bekræft adgangskode”.
5. Tryk på knappen "Gem" nederst på siden.

Glemt kodeord

1. Opret en sag i http://kundeservice.dbc.dk, og medsend den e-mail-adresse du bruger i DDB CMS. Du får herefter tilsendt et link, som giver dig adgang til at nulstille dit kodeord.

Bibliotekets Tekniske kontaktperson for DDB CMS har modtaget bruger og pinkode til den primære lokaladministrator. De øvrige redaktører opretter biblioteket selv.

Konfigurer fjernadgang med proxy til de licensbelagte elektroniske ressourcer.
==============================================================================

Fjernadgangsproxy sørger for adgangskontrollen til udvalgte licensbelagte ressource.
Se [Fjernadgang med proxy manualen](https://platform.dandigbib.org/projects/ddb-cms/wiki/Proxyvejledning) for yderligere information om hvordan DDB CMS kan konfigureres for at give brugerne adgang til de licensbelagte elektroniske ressourcer.

**Cookie- og privatlivspolitik**
================================

Vi vil gerne tilbyde vores brugere en overskuelig og brugervenlig hjemmeside. For at sikre os, at indholdet på siden er relevant og til at finde rundt i, benytter vi os af cookies. Cookies giver os vigtige informationer om, hvordan vores side bliver brugt, hvilke sider der bliver set mest, hvor længe vores brugere bliver på siderne osv.

Hvad er en cookie?
------------------

En cookie er en lille tekstfil, der lagres i din browser for at kunne genkende din computer ved tilbagevendende besøg. Cookies er ikke aktive filer; de kan altså ikke udvikle virus eller spore indhold på din computer. Det eneste, de gør, er at sende anonyme oplysninger tilbage til os om fx besøgstidspunkt, -varighed osv.

På denne hjemmeside bruger vi cookies til følgende formål:

Statistik: Vi bruger Mapp (tidl. Webtrekk) til at føre statistik over trafikken på siden, sådan at vi bedst muligt kan tilpasse den brugernes behov. Vi får blandt andet oplysninger om antal besøg, gennemsnitlig besøgsvarighed og færden rundt på siden.

Login: Når du logger ind for at se lånerstatus, reservere m.m. sættes en sessions-cookie. Denne cookie forsvinder når du lukker browseren.

Hvis du ikke vil tillade cookies
--------------------------------

Hvis du ikke vil tillade brugen af cookies på din computer, kan du ændre i indstillingerne i din browser, så den husker det fremover. Du kan også slette cookies, der allerede er lagret.
Se vejledning og læs mere om cookies på http://minecookies.org/cookiehandtering.
Vær opmærksom på, at du ved at spærre for cookies besværliggør brugen af hjemmesiden.

Brug af personoplysninger
-------------------------

Personoplysninger bliver på intet tidspunkt videregivet eller solgt til tredjepart, og vi indsamler ikke personoplysninger, uden du selv har givet os disse.

For at tilbyde en bedre brugeroplevelse kan du dele indhold fra vores hjemmeside på sociale medier, som Facebook og Twitter. Når du deler indholdet, kan du forvente tredjeparts-cookies.

Hvad er tredjeparts-cookies?
----------------------------

Tredjeparts-cookies afsættes på din computer af en tredjepart, som har elementer på vores hjemmeside. Tredjeparts-cookies sættes på din computer til markedsførings- og statistikformål for de respektive leverandørers hjemmeside. Hvis tredjeparts-cookies bekymrer dig, kan disse deaktiveres i din browser.\_

Rettelse af cookie-tekst til brugerne
-------------------------------------

Default tekst samt knaptekster kan rettes under /admin/config/system/eu-cookie-compliance
På grund af en fejl er det ikke muligt at gemme rettelsen, hvis feltet "Thank you banner message" er tomt. Det er derfor nødvendigt at skrive noget i dette felt, inden man gemmer, da rettelsen ellers ikke vil slå igennem. Så længe man ikke sætter flueben i "Enable thank you banner", vises denne tekst ikke til brugerne, så det er uden betydning, hvad man skriver, blot feltet ikke er tomt.


