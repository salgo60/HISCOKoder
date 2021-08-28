# HISCOKoder - Historiska yrken #

Kan vi Digitalt koppla ihop historiska yrken i Sverige **"same as"**? Och enkelt hitta i alla databaser alla personer/beskrivningar av exempelvis [isutkörare](https://sv.wikipedia.org/wiki/Iskarl) (ett av Sveriges vanligaste yrken)...Känns som en lågt hängande frukt... utmaningen är nog att börja jobba ihop och ha [publika backlogs](https://www.youtube.com/watch?v=502ILHjX9EE) och föra en dialog på exempelvis GITHUB ....

Projekt SWEPOP har skapat [Principles of Coding Swedish Historic Occupations](https://swedpop.se/wp-content/uploads/2021/06/Principles-of-Coding-Swedish-Historic-Occupations.pdf) tanken är att se om vi kan föra över det till Wikidata och se om andra aktörer rör sig åt samma håll då det gäller att digitalisera datat och röra sig mot HISCO istället för textsträngar.

Tanken
* starta dela planer --> [diskussion](https://github.com/salgo60/HISCOKoder/discussions) eller [issues](https://github.com/salgo60/HISCOKoder/issues) kan fungera som en start eller varför inte [Clubhouse](https://www.clubhouse.com/room/m2XWQAzx) - [linked data needs linked people](https://twitter.com/hashtag/LinkedDataNeedsLinkedPeople?src=hash)
* starta fundera på olikheter mellan olika yrken i maskinläsbar form
  * att bara ha textsträngar blir lätt som att ange en textsträng **Stockholm** och sedan låta läsaren gissa om det är
    *  Stockholm = [Q94385](https://www.wikidata.org/wiki/Q94385?uselang=sv), Stockholm = [Q506250](https://www.wikidata.org/wiki/Q506250?uselang=sv), Stockholm = [Q922489](https://www.wikidata.org/wiki/Q922489?uselang=sv), Stockholm = [Q876775](https://www.wikidata.org/wiki/Q876775?uselang=sv), Stockholm = [Q3233188](https://www.wikidata.org/wiki/Q3233188)..... för många mer betydelser se [Stockholm olika betydelser](https://sv.wikipedia.org/wiki/Stockholm_(olika_betydelser))
  * beskriv hur det implementeras av olika institutioner jmf hur Wikidata idag använder [ShEx](https://shex.io/) för att beskriva olika informationsmängder se exempel [E134 Riksdagsman](https://www.wikidata.org/wiki/EntitySchema:E134), [E283 Svensk församling](https://www.wikidata.org/wiki/EntitySchema:E283), [E260 Fredmans epistel](https://www.wikidata.org/wiki/EntitySchema:E260), [E250 svensk kommun](https://www.wikidata.org/wiki/EntitySchema:E250), [E271 offentlig konst Umeå](https://www.wikidata.org/wiki/EntitySchema:E271), [E99 staty](https://www.wikidata.org/wiki/EntitySchema:E99)    
    * [Wikidata:WikiProject Schemas](https://www.wikidata.org/wiki/Wikidata:WikiProject_Schemas)
* kan Wikidata vara en enabler? 
  * Min feedback från [LD4](https://sites.google.com/stanford.edu/ld4-community-site/home) är att aktörer som Stanford University Libraries, USA:s kongressbibliotek, Columbia University, Harvard Library gör detta se deras senaste konferans [LD4 schedule](https://ld42021.sched.com/) /  Youtube lista "[2021 LD4 Conference Videos](https://www.youtube.com/watch?v=ludJFf06w94&list=PLx2ZluWEZtICVGpkAIzRW4P17r2jFSOiY)" där jag pratade om publika identifierare i svenska boken Bautil från 1750 [artikel](https://meta.wikimedia.org/wiki/Structured_data_for_GLAM-Wiki/Roundtripping/KMB)/[video](https://youtu.be/GeDXzInR_mA?t=974) 
  * vad behövs i Wikidata för att vi skall starta i Sverige!!! Vilka är intresserade och vilka byggstenar har ni? 
     * API ex. [SKBL](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBL%20yrken%20JSON.ipynb)
     * dokumentation ex. [SWEPOP](https://swedpop.se/wp-content/uploads/2021/06/Principles-of-Coding-Swedish-Historic-Occupations.pdf)
     * att skapa en mer avancerad modell för yrken och kopplingen till person se [JSON filen](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBL%20yrken%20JSON.ipynb) från SKBL mer beskriven nedan där man anger när en person jobbar med ett visst yrke och var....
     * att ha en modell för vilka egenskaper som behövs för att beskriva ett yrke se Wikidata spretiga försök med 
        * kvinnlig form [P2521](https://www.wikidata.org/wiki/Property:P2521)
        * manlig form [P3321](https://www.wikidata.org/wiki/Property:P3321)
        * egenskaper för denna objekttyp [Property:P1963](https://www.wikidata.org/wiki/Property:P1963)
          * exempel forskare [Q901](https://www.wikidata.org/wiki/Q901) _egenskap för denna objekttyp_ utbildad vid [P69](https://www.wikidata.org/wiki/Property:P69)
        * verksamhetsområde [P425](https://www.wikidata.org/wiki/Property:P425)
          * exempel skulptör [Q1281618](https://www.wikidata.org/wiki/Q1281618) _verksamhetsområde_ bildhuggeri [Q11634](https://www.wikidata.org/wiki/Q11634)
        * beskriven av källa [P1343](https://www.wikidata.org/wiki/Property:P1343)
        * föremål eller koncept som används av subjektet [P2283](https://www.wikidata.org/wiki/Property:P2283)....
     * ?!?!?

## Yrkesklassificering - HISCOkoder ##
Status vad vi ser

#### Har HISCOkoder
* Mats Hayen har ett projekt [Tidigmoderna konkurser!](http://www.tidigmodernakonkurser.se/) som har HISCOkoder se ["Titelklassificering"](http://www.tidigmodernakonkurser.se/index.php/page/3)
  * [Titelklassificering](http://www.tidigmodernakonkurser.se/index.php/page/3) / [Undergrupp i Hisco](http://www.tidigmodernakonkurser.se/index.php/extended/subject) 
* Swepop - [swedpop.se](https://swedpop.se/)...
  * [HISCO codes and description](https://swedpop.se/wp-content/uploads/2021/06/HISCO-codes-and-description.pdf) Version: June 28, 2021
* ...

#### Andra aktörer som verkar sakna bra strukturerad data och koppling HISCO "utan kör eget"
* Alvin [Wikidata P6821](https://www.wikidata.org/wiki/Property_talk:P6821) har > [34 500 personer, platser ...](https://w.wiki/3yEt) kopplade till Wikidata
  * [yrken i WD för i personer kopplade till Alvin](https://w.wiki/3u2w)
  * [samma fråga men visa om Wikidata har en bild](https://w.wiki/3uCW) eller bildkatalog  
    * samma fråga men [yrken som saknar bild i Wikidata](https://w.wiki/3vJb)
  * samma fråga men där yrkena också har en artikel på [svenska wikipedia](https://w.wiki/3uEV) / [engelska](https://w.wiki/3uEi) / [tyska](https://w.wiki/3uEa) / [kinesiska](https://w.wiki/3uEs) / saknar [svensk Wikipedia artikel](https://w.wiki/3uJE)
     * vilka egenskaper har dessa yrken i Wikidata idag (behövs nog en hel del jobb för att få ordning på detta)
       * av typ [Authority control properties ](https://w.wiki/3uT2)
       * alla [externa egenskaper](https://w.wiki/3uSx) 
       * [alla Wikidata egenskaperna](https://w.wiki/3uSq) / samma som bubble chart

![](https://github.com/salgo60/HISCOKoder/blob/main/img/WD%20egenskaper%20yrken.png)
![](https://github.com/salgo60/HISCOKoder/blob/main/img/WD%20egenskaper%20yrken%20bubble.png)
  * [Notepad](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Alvin%20yrken.ipynb) kör igenom alla poster i Wikidata kopplade till Uppsala universitetsbibliotek Alvin plattform > 28000 kopplingar där vi försöker identifiera yrkena i html sidan hos Alvin se även [T225522](https://phabricator.wikimedia.org/T225522) 
    * [csv fil](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Alvin_yrken_value_counts.csv) > 3000 yrken  
![](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Alvin_yrken_alla.png)
* Arken [Wikidata P8899](https://www.wikidata.org/wiki/Property_talk:P8899) har > [3 390](https://w.wiki/3yEs) personer kopplade till Wikidata
  * [yrken i Wikidata för personer kopplade till Arken](https://w.wiki/3wEf)/[lista](https://w.wiki/3wEd)
  * har lite struktur men inga kopplingar HISCOkoder finns ett schema ej åtkomligt https://arken.kb.se/Actor-occupations
    * exempel 
      * SKOS [Diplomater](https://arken.kb.se/Diplomater;skos)   
        * finns stöd för flerspråkighet 
      * SKOS [Författare](https://arken.kb.se/F%C3%B6rfattare;skos)  
      * SKOS [filmproducenter](https://arken.kb.se/filmproducenter)
        * finns stöd BT (Broader term), NT (Narrow term)  
        * har även udda term **skos:note** för koppling https://id.kb.se/term/sao/Diplomater borde vara **samma som**
![](https://github.com/salgo60/HISCOKoder/blob/main/img/SKOSArken.png)      
  * [Notepad](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Arken%20yrken.ipynb) webscrapar Arken efter yrken / [csv](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Arken_yrken_value_counts.csv)  - [alla](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Arken_yrken.csv)
![](https://github.com/salgo60/HISCOKoder/blob/main/img/Arken_yrken.png)    
* Digitaltmuseum [Wikidata P7847](https://www.wikidata.org/wiki/Property_talk:P7847) - P7846 används för bilder - P1248 har > [18000](https://w.wiki/3yEq) kopplingar till Wikidata
  * har dataset [Life roles (KulturIT AS [no])](https://kulturnav.org/23c7080c-6752-4691-8c8a-ce0d65623c51) -  [Notepad](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/kulturnav%20dataset%20liferoll.ipynb) / [csv](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/kulturnav_liferoll.csv)
  * [yrken i Wikidata för personer i kulturnav P1248](https://w.wiki/3u2s) - [P1248](https://www.wikidata.org/wiki/Property_talk:P1248)
    * [WD egenskaper för yrken kopplade till dessa personer](https://w.wiki/3wgt)
  * kulturnav.org: August Strindberg vars [RDF](https://kulturnav.org/291ad5e4-1169-4f50-8fb3-6a82308c4ff6.json-ld) har Liferole som pekar på ex. [JSON författare](https://kulturnav.org/5ffd9b2f-a555-466e-886b-2185d95f4a83.json-ld) som
    * har **exactMatch** 
      * [metadataregistry.org](http://metadataregistry.org/schemaprop/show/id/121.html) 
      * [Getty Vocabularies](http://vocab.getty.edu/aat/300025492)
      * [Library of congress](https://id.loc.gov/vocabulary/relators/aut.html)
![](https://github.com/salgo60/HISCOKoder/blob/main/img/StrindbergLiferole.png)
![](https://github.com/salgo60/HISCOKoder/blob/main/img/kulturnav_org_F%C3%B6rfattare.png)
    * har **[mads:see](https://id.loc.gov/ontologies/madsrdf/v1.html#see)** sv:Wikipedia [författare](https://sv.wikipedia.org/wiki/F%C3%B6rfattare)
![](https://github.com/salgo60/HISCOKoder/blob/main/img/Mads_see.png)    
* Historiska museet [Wikidata P9495](https://www.wikidata.org/wiki/Property_talk:P9495) har > [3 360](https://w.wiki/3yEv) personer kopplade till Wikidata
  * [yrken i Wikidata för personer kopplade till Historiska museer](https://w.wiki/3u2q)
  * planer finns se [tweet](https://twitter.com/linneakarlberg_/status/1427886596058198018) "Vi har interna identifierare för yrken och möjligheten finns att koppla dessa till externa, och lägga ut yrkena som egna poster på vårt onlinesök"
  * se [Historiska museet yrken #6](https://github.com/salgo60/HISCOKoder/issues/6)
* Kungliga biblioteket - LIBRISXL verkar ha **hasOccupation** med **label** utan språktag och utan koppling HISCOkod se [August Strindberg](https://libris.kb.se/tr574vdc33gk2cc/data.jsonld) - [yrken i WD för dessa personer](https://w.wiki/3u2k) - [yrken i Wikidata för personer kopplade till KB](https://w.wiki/3u2p)
![](https://github.com/salgo60/HISCOKoder/blob/main/img/LIBRISXL_has_occupation.png)
* Levande musikarv [Wikidata P4607](https://www.wikidata.org/wiki/Property_talk:P4607) - har > [6000](https://w.wiki/3yEx) personer/verk kopplade till Wikidata
  * [yrken i Wikidata för personer kopplade till Levande musikarv](https://w.wiki/3u2k)
* Litteraturbanken [Wikidata P5101](https://www.wikidata.org/wiki/Property_talk:P5101) - har > [2800](https://w.wiki/3yF4) personer kopplade till Wikidata
  * [yrken i Wikidata för personer kopplade till Litteraturbanken](https://w.wiki/3u2y)
  * här har vi kopplat böcker som [Bellman var där. En vägvisare till Bellmansmiljöer (1997)](https://litteraturbanken.se/f%C3%B6rfattare/Anders%C3%A9nML/titlar/BellmanVarD%C3%A4r/sida/3/faksimil?om-boken) till Wikidata se [karta](https://w.wiki/mMH)/[graf](https://w.wiki/mYV) och [Runstenar till böcker hos Litteraturbanken](https://w.wiki/3Fz9) se [karta](https://w.wiki/3Fz9) se längre artikel om [dataroundtripping](https://meta.wikimedia.org/wiki/Structured_data_for_GLAM-Wiki/Roundtripping/KMB) 
* Riksarkivet SBL [Wikidata P3217](https://www.wikidata.org/wiki/Property:P3217?uselang=sv) - har > [7000](https://w.wiki/3yF6) personer/släkter kopplade till Wikidata
  * [yrken i Wikidata för personer kopplade till SBL](https://w.wiki/3u2i)
  * har yrken men ingen koppling till HISCO koder [länk](https://sok.riksarkivet.se/sbl/YrkesSearch.aspx?fbclid=IwAR1CHuNsVj45vQyh9LTy-vJV7344qhMys421nlIY3Jq82h1KqcQZlH3B70o) 
  * se [csv fil](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SBLyrken.csv) och [Notebook](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Yrken%20SBL.ipynb)
  * jämförelse yrken hos SKBL och SBL - [Notebook](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/J%C3%A4mf%C3%B6r%20yrken%20SBL%20SKBL.ipynb) / [csv fil](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBL_SBL_yrken.csv)
    * både SBL och SKBL identifierar yrken med textsträngar vilket gör detta lite ohanterligt och hobbymässigt
    * yrken bör ha unika persistenta identifierare och en [kunskapsgraf](https://vimeo.com/36752317) där egenskaper beskriver yrket och har samma som ex. HISCOkoder  

![](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBLSBLyrken.png)        

* [Stadens ansikte](https://stockholmia.stockholm.se/forskning/projekt/stadens-ansikten/) ingen koppling idag till Wikidata 
  * se försök att öppna en dialog [T268374](https://phabricator.wikimedia.org/T268374) 
* Svenskt Kvinnobiografiskt lexikon [Wikidata P4963](https://www.wikidata.org/wiki/Property_talk:P4963) - har > [1900](https://w.wiki/3yFB) personer... kopplade till Wikidata
  * [yrken i Wikidata för personer kopplade till SKBL](https://w.wiki/3u2h) motsv. [partitillhörighet](https://w.wiki/3wPR) 
  * har vissa yrken som [nyckelord](https://skbl.se/sv/nyckelord)  
  * se [csv fil](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBLyrken.csv) och [Notebook](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Yrken%20SKBL.ipynb)
  * JSON strukturerad data --> yrken [SKBLyrken_valuecount.csv](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBLyrken_valuecount.csv)/[csv per person](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBLyrken_newListdf.csv) och [Notebook JSON](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBL%20yrken%20JSON.ipynb)
    * SKBL har ex. Kerstin Anneka Anderson [svenska](https://skbl.se/sv/artikel/KerstinAnnekaAnderson) [engelska](https://skbl.se/en/article/KerstinAnnekaAnderson) [json](https://skbl.se/sv/artikel/KerstinAnnekaAnderson.json) där yrket i JSON har struktur
       * occupation 
         * description 
         * detail - borde vara [Linked data](https://vimeo.com/36752317)  för kopplingar till arbegtsgivare etc...
         * from
           * comment / date - borde vara maskinläsbara datum, tidsperioder
         * place
           * är med koordinat och text sträng ej [Linked data](https://vimeo.com/36752317) 
         * to
         * type kan vara Yrke / Ideellt arbete  
![](https://github.com/salgo60/HISCOKoder/blob/main/img/SKBLJson.png)        
![](https://github.com/salgo60/HISCOKoder/blob/main/img/SKBL_yrken_json.png)        
![](https://github.com/salgo60/HISCOKoder/blob/main/img/SKBL_yrken_json2.png)
## Övrigt
* [ISCO–08](https://www.ilo.org/public/english/bureau/stat/isco/docs/publication08.pdf) "International Standard
Classification of Occupations Structure, group definitions and correspondence tables"
### SSYK Yrken
* SCB har [SSYK koder för "moderna" yrken](https://www.scb.se/dokumentation/klassifikationer-och-standarder/standard-for-svensk-yrkesklassificering-ssyk/)
  * diskussion jobtech [SSYK egenskap i Wikidata](https://forum.jobtechdev.se/t/ssyk-egenskap-i-wikidata/164/8)
  * Wikidata egenskap [P8654](https://www.wikidata.org/wiki/Property_talk:P8654) se  även task ["SSYK 2012"](https://phabricator.wikimedia.org/T263945) 
  * min tro är att dessa koder inte är funktionella för en datadriven arbetsmarknad ett nytt initiativ har startats upp se sr.se tyvärr svårt att förstå vad de gör och har för leverabler 
### Wikipedia
* historiska yrken 
  * [sv:Kategori:Historiska_yrken](https://sv.wikipedia.org/wiki/Kategori:Historiska_yrken)
  * [Category:Obsolete occupations](https://en.wikipedia.org/wiki/Category:Obsolete_occupations)
  * [Kategori:Historiske beskjeftigelser](https://no.wikipedia.org/wiki/Kategori:Historiske_beskjeftigelser)
  * [Kategorie:Historischer_Beruf](https://de.wikipedia.org/wiki/Kategorie:Historischer_Beruf)
* projekt [Wikidata:WikiProject Occupations and professions](https://www.wikidata.org/wiki/Wikidata:WikiProject_Occupations_and_professions) 
## Kontaktpersoner
* [Annika Westberg, CEDAR](https://www.umu.se/en/staff/annika-westberg/)


# Wikidata
* om [Wikidata](https://www.youtube.com/watch?v=m_9_23jXPoE) / ["Making feedback loops work for Wikidata"](https://www.youtube.com/watch?v=Xq1ss6WFjeE) / [Wikidata:Mismatch Finder](https://www.wikidata.org/wiki/Wikidata:Mismatch_Finder)
* [Svenska egenskaper i Wikidata](https://www.wikidata.org/wiki/Template:Sweden_properties)
![](https://github.com/salgo60/HISCOKoder/blob/main/img/Swedenprop.png)
* Saknas idag en egenskap för HISCOkoder -  [Q5629694](https://www.wikidata.org/wiki/Q5629694)
## Wikidata - mer än yrken
Intressant i denna ekvation där vi ovan ser hur svenska kulturinstitutioner lyckas trassla till något så trivialt som historiska yrken är hur mycket kopplingar en global databas som Wikidata innehåller till andra extern egenskaper ( se senaste skapade [WD egenskaper](https://w.wiki/AKq) > 9000, [externa](https://w.wiki/DYQ) > 6300) men även antal språk som stöds där svenska databaser oftast antar att dom bara skall leverera på svenska. 
* Alvin har ofta en rad om personen med namnet och yrket, i Engelsk Wikipedia finns det 31799 artiklar om personer i Alvin... **Varför länkar inte Alvin?** det finns artiklar på [301 språk](https://w.wiki/3yGM) för personer kopplade till Alvin, [lista med personer med flest artiklar](https://w.wiki/3yG4), [list med personer kopplade till Alvin men inte har en artikel på svenska Wikipedia](https://w.wiki/3yG7) men på annat språk = 9500...
![](https://github.com/salgo60/HISCOKoder/blob/main/img/AlvinWikiLang.png)
* Personer kopplade till Alvin > [34 500 personer, platser ...](https://w.wiki/3yEt) --> men dessa personer i Wikidata har kopplingar till [1300 externa egenskaper](https://w.wiki/3yFH) osv... det är ett enormt jobb att hålla detta vid liv och för att jobba med data skall man ha dom kunskaperna. Kan svenska kulturinstitutioner som pratar samma språk åker på samma konferenser, får bidrag ur samma "ficka" inte klara av att synka hur historiska yrken beskrivs så är att koppla sig till externa egenskaper i andra länder nog en omöjlighet om man inte byter ut hela laget....  
![](https://github.com/salgo60/HISCOKoder/blob/main/img/AlvinExternaEgenskaperB.png)
![](https://github.com/salgo60/HISCOKoder/blob/main/img/AlvinExternaEgenskaper.png)
