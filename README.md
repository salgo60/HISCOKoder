# HISCOKoder - Historiska yrken #

Projekt SWEPOP har skapat [Principles of Coding Swedish Historic Occupations](https://swedpop.se/wp-content/uploads/2021/06/Principles-of-Coding-Swedish-Historic-Occupations.pdf?fbclid=IwAR11GjBmaQnBhqVgiI65bFh6YbvMpdoYN0IDHrKSS-Lc4DZcLXtZTc82hTo) tanken är att se om vi kan föra över det till Wikidata och se om andra aktörer rör sig åt samma håll då det gäller att digitalisera datat och röra sig mot HISCO istället för textsträngar.

## Yrkesklassificering - HISCOkoder ##
Status vad vi ser

#### Har HISCOkoder
* Mats Hayen har ett projekt [Tidigmoderna konkurser!](http://www.tidigmodernakonkurser.se/) som har HISCOkoder se ["Titelklassificering"](http://www.tidigmodernakonkurser.se/index.php/page/3)
  * [Titelklassificering](http://www.tidigmodernakonkurser.se/index.php/page/3) / [Undergrupp i Hisco](http://www.tidigmodernakonkurser.se/index.php/extended/subject) 
* Swepop - [swedpop.se](https://swedpop.se/)...
  * [HISCO codes and description](https://swedpop.se/wp-content/uploads/2021/06/HISCO-codes-and-description.pdf) Version: June 28, 2021
* ...

#### Andra aktörer som verkar sakna bra strukturerad data och koppling HISCO utan kör eget
* Alvin [Wikidata P6821](https://www.wikidata.org/wiki/Property_talk:P6821) - [yrken i WD för i personer kopplade till Alvin](https://w.wiki/3u2w)
  * [samma fråga men visa om Wikidata har en bild](https://w.wiki/3uCW) eller bildkatalog  
  * samma fråga men där yrkena har en artikel på [svenska wikipedia](https://w.wiki/3uEV) / [engelska](https://w.wiki/3uEi) / [tyska](https://w.wiki/3uEa) / [kinesiska](https://w.wiki/3uEs) / sanknar [svensk Wikipedia artikel](https://w.wiki/3uJE)
     * vilka [externa egenskaper har dessa yrken i Wikidata
       * av typ [Authority control properties ](https://w.wiki/3uT2)
       * alla [externa egenskaper](https://w.wiki/3uSx) 
       * [alla Wikidata egenskaperna](https://w.wiki/3uSq)
  * [Notepad](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Alvin%20yrken.ipynb) kör igenom alla poster kopplade till Wikidata > 28000 och försöker identifiera yrkena i html sidan hos Alvin se även [T225522](https://phabricator.wikimedia.org/T225522) 
    * [csv fil](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Alvin_yrken_value_counts.csv) > 3000 yrken  
![](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Alvin_yrken_alla.png)
* Digitaltmuseum [Wikidata P7847](https://www.wikidata.org/wiki/Property_talk:P7847) 
  * har dataset [Life roles (KulturIT AS [no])](https://kulturnav.org/23c7080c-6752-4691-8c8a-ce0d65623c51) men annars verkar det istrukturerat
  * [yrken i Wikidata för personer i kulturnav P1248](https://w.wiki/3u2s) - [P1248](https://www.wikidata.org/wiki/Property_talk:P1248)

* Historiska museet [Wikidata P9495](https://www.wikidata.org/wiki/Property_talk:P9495) - [yrken i Wikidata för dessa personer](https://w.wiki/3u2q)
* Kungliga biblioteket - LIBRISXL verkar bara vara textsträngar se [August Strindberg](https://libris.kb.se/tr574vdc33gk2cc/data.jsonld) - [yrken i WD för dessa personer](https://w.wiki/3u2k) - [yrken i Wikidata för dessa personer](https://w.wiki/3u2p)
* Levande musikarv [Wikidata P4607](https://www.wikidata.org/wiki/Property_talk:P4607) - [yrken i Wikidata för dessa personer](https://w.wiki/3u2k)
* Litteraturbanken [Wikidata P5101](https://www.wikidata.org/wiki/Property_talk:P5101)  - [yrken i Wikidata för dessa personer](https://w.wiki/3u2y)
* Riksarkivet SBL [Wikidata P3217](https://www.wikidata.org/wiki/Property:P3217?uselang=sv) - [yrken i Wikidata för dessa personer](https://w.wiki/3u2i)
  * har yrken men ingen koppling till HISCO koder [länk](https://sok.riksarkivet.se/sbl/YrkesSearch.aspx?fbclid=IwAR1CHuNsVj45vQyh9LTy-vJV7344qhMys421nlIY3Jq82h1KqcQZlH3B70o) 
  * se [csv fil](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SBLyrken.csv) och [Notebook](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Yrken%20SBL.ipynb)
  * jämförelse yrken hos SKBL och SBL - [Notebook](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/J%C3%A4mf%C3%B6r%20yrken%20SBL%20SKBL.ipynb) / [csv fil](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBL_SBL_yrken.csv)

![](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBLSBLyrken.png)        

* [Stadens ansikte](https://stockholmia.stockholm.se/forskning/projekt/stadens-ansikten/) ingen koppling idag till Wikidata 
  * se försök att öppna en dialog [T268374](https://phabricator.wikimedia.org/T268374) 
* Svenskt Kvinnobiografiskt lexikon [Wikidata P4963](https://www.wikidata.org/wiki/Property_talk:P4963) - [yrken i Wikidata för dessa personer](https://w.wiki/3u2h)
  * har vissa yrken som [nyckelord](https://skbl.se/sv/nyckelord)  
  * se [csv fil](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBLyrken.csv) och [Notebook](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/Yrken%20SKBL.ipynb)
  * JSON strukturerad data --> yrken [SKBLyrken_valuecount.csv](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBLyrken_valuecount.csv)/[csv per person](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBLyrken_newListdf.csv) och [Notebook JSON](https://github.com/salgo60/HISCOKoder/blob/main/Jupyter/SKBL%20yrken%20JSON.ipynb)
    * SKBL har ex. Kerstin Anneka Anderson [svenska](https://skbl.se/sv/artikel/KerstinAnnekaAnderson) [engelska](https://skbl.se/en/article/KerstinAnnekaAnderson) [json](https://skbl.se/sv/artikel/KerstinAnnekaAnderson.json) där yrket i JSON har struktur
       * occupation 
         * description
         * detail
         * from
           * comment / date
         * place
           * är med koordinat och text sträng ej [Linked data](https://vimeo.com/36752317) 
         * to
         * type kan vara Yrke / Ideellt arbete  
![](https://github.com/salgo60/HISCOKoder/blob/main/img/SKBLJson.png)        
![](https://github.com/salgo60/HISCOKoder/blob/main/img/SKBL_yrken_json.png)        

## Övrigt
### SSYK Yrken
* SCB har [SSYK koder för yrken](https://www.scb.se/dokumentation/klassifikationer-och-standarder/standard-for-svensk-yrkesklassificering-ssyk/)
  * diskussion jobtech [SSYK egenskap i Wikidata](https://forum.jobtechdev.se/t/ssyk-egenskap-i-wikidata/164/8)
  * Wikidata egenskap [P8654](https://www.wikidata.org/wiki/Property_talk:P8654) se  även task ["SSYK 2012"](https://phabricator.wikimedia.org/T263945)  
### Wikipedia
* historiska yrken 
  * [sv:Kategori:Historiska_yrken](https://sv.wikipedia.org/wiki/Kategori:Historiska_yrken)
  * [Category:Obsolete occupations](https://en.wikipedia.org/wiki/Category:Obsolete_occupations)
  * [Kategori:Historiske beskjeftigelser](https://no.wikipedia.org/wiki/Kategori:Historiske_beskjeftigelser)
  * [Kategorie:Historischer_Beruf](https://de.wikipedia.org/wiki/Kategorie:Historischer_Beruf)
* projekt [Wikidata:WikiProject Occupations and professions](https://www.wikidata.org/wiki/Wikidata:WikiProject_Occupations_and_professions) 
## Kontaktperson
* [Annika Westberg, CEDAR](https://www.umu.se/en/staff/annika-westberg/)


# Wikidata
* om [Wikidata](https://www.youtube.com/watch?v=m_9_23jXPoE) / ["Making feedback loops work for Wikidata"](https://www.youtube.com/watch?v=Xq1ss6WFjeE) / [Wikidata:Mismatch Finder]/(https://www.wikidata.org/wiki/Wikidata:Mismatch_Finder)
* [Svenska egenskaper i Wikidata](https://www.wikidata.org/wiki/Template:Sweden_properties)
![](https://github.com/salgo60/HISCOKoder/blob/main/img/Swedenprop.png)
* Saknas idag en egenskap för HISCOkoder -  [Q5629694](https://www.wikidata.org/wiki/Q5629694)
