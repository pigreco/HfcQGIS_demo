---
theme : "black"
transition: "zoom"
highlightTheme: "darkula"
logoImg: "./doc/logo_RTD_def_2.png"
slideNumber: true
---

## HfcQGIS
Help funzioni calcolatore di campi di QGIS

©2019 CC-BY-SA Salvatore Fiandaca pigrecoinfinito@gmail.com

---

Presentazione **[#HfcQGIS](http://hfcqgis.opendatasicilia.it/it/latest/)**

al primo **QGIS Summer Camp** Padova 5/7 Luglio 2019

<p align="center"> <a href="http://hfcqgis.opendatasicilia.it/it/latest/" target="_blank"><img src="./doc/loc_HfcQGIS2.png" width="400" title="#HfcQGIS"></a>
</p>

---

Questa guida nasce per rispondere alle numerose richieste di aiuto sull’uso del **calcolatore di campi**, a integrazione - con esempi e molti screenshot - della guida ufficiale di **QGIS**

[Facebook](https://www.facebook.com/groups/GisItalia/permalink/10156495751381385/?comment_tracking=%7B%22tn%22%3A%22O%22%7D)

--

<p align="center"> <a href="http://hfcqgis.opendatasicilia.it/it/latest/" target="_blank"><img src="./doc/hfc003.png" width="600" title="#HfcQGIS"></a>
</p>

--

<p align="center"> <a href="http://hfcqgis.opendatasicilia.it/it/latest/" target="_blank"><img src="./doc/hfc002.png" width="600" title="#HfcQGIS"></a>
</p>

--

<p align="center"> <a href="http://hfcqgis.opendatasicilia.it/it/latest/" target="_blank"><img src="./doc/hfc001.png" width="600" title="#HfcQGIS"></a>
</p>

---

Questa versione in formato **[Read The Docs](https://docs.readthedocs.io/en/latest/index.html)** è stata realizzata dalla comunità [OpenDataSicilia](http://opendatasicilia.it), in particolare da: [Andrea Borruso](https://twitter.com/aborruso), [Totò Fiandaca](https://twitter.com/totofiandaca) e [Giovan Battista Vitrano](https://twitter.com/gbvitrano).
L'idea è stata di Giovan Battista, mentre la musa ispiratrice per la scelta di Read The Docs è [Ciro Spataro](https://twitter.com/cirospat).

<p align="center"> <a href="http://opendatasicilia.it/" target="_blank"><img src="./doc/face4ods.png" width="550" title="opendatasicilia.it"></a>
</p>

---

#### OpenDataSicilia fa scruscio
(«rumore» in siciliano) qui:

* mailing list https://groups.google.com/forum/#!forum/opendatasicilia;
* sito web http://opendatasicilia.it;
* gruppo facebook https://www.facebook.com/groups/opendatasicilia/;
* account twitter http://twitter.com/opendatasicilia;
* gruppo Telegram https://t.me/opendatasicilia.


<p align="center"> <a href="http://opendatasicilia.it/" target="_blank"><img src="./doc/ods_logo_esa.png" width="150" title="opendatasicilia.it"></a>
</p>

--

<p align="center"> <a href="http://ods16.opendatasicilia.it/" target="_blank"><img src="./doc/ods16ME.png" width="1550" title="opendatasicilia.it"></a>
</p>

[Google Photos Opendatasicilia - LODS1](https://photos.google.com/share/AF1QipOY9E7G5GnRmjyR-ylXVd5aG2PTIIQqOucUIgkzP7OGCWXC1urcyXhOGTN6q2pWqA?key=Z0tZZXpUOGp0SS00UlNmQlhEcTZFaXBsRFU4bzlB)

[Google Photos Opendatasicilia -LODS2](https://photos.google.com/share/AF1QipNP-Yu1f7OVetq6dRsDjPWhk7tLMBhL2fGk_aGGCAcjth1RSYZqlUI-7CfwYvNEdA?key=dUVxVEtZM0YtVnV6MlViZFk0OGJWRmR1a1BGNTd3)

---

## Che cosa è HfcQGIS
HfcQGIS è un manuale che spiega come usare il calcolatore di campi e le relative funzioni/espressioni; nasce per rispondere alle numerose richieste di aiuto sull’uso del calcolatore di campi e per colmare un vuoto sulla guida online di QGIS con esempi e molti screenshot.

---

## Come usarlo

<p align="center"> <a href="http://ods16.opendatasicilia.it/" target="_blank"><img src="./doc/pc_cell.png" width="500" title="opendatasicilia.it"></a>
</p>

--

### link

Short link di HfcQGIS

bit.ly/hfcqgis

condividi con #hfcqgis #qgis @opendatasicilia

---

## Come è organizzata

<p align="center"> <a href="http://hfcqgis.opendatasicilia.it/it/latest/index.html" target="_blank"><img src="./doc/home.png" width="900" title="#HfcQGIS"></a>
</p>

--

<p align="center"> <a href="http://hfcqgis.opendatasicilia.it/it/latest/index.html" target="_blank"><img src="./doc/home_cell.png" width="900" title="#HfcQGIS"></a>
</p>

---

### grazie per l'attenzione

<p align="center"> <a href="http://hfcqgis.opendatasicilia.it/it/latest/release/novita_38.html" target="_blank"><img src="./doc/fine.png" width="900" title="#HfcQGIS"></a>
</p>

---

### Perché è utile usare il field calc/espressioni

Il field calc agisce direttamente nella tabella attributi e NON crea altri layer

--

### Esempio1 - Spatial Join

Supponiamo di avere dei punti, uno per ogni regione italiana, e volessimo associare il relativo nome della regione in cui ricade:

<p align="center"> <a href="http://hfcqgis.opendatasicilia.it/it/latest/release/novita_38.html" target="_blank"><img src="./doc/esempi/sj_01.png" width="700" title="#HfcQGIS"></a>
</p>

--

## da Processing

Unisci attributi per posizione

<p align="center"> <a href="http://hfcqgis.opendatasicilia.it/it/latest/release/novita_38.html" target="_blank"><img src="./doc/esempi/sj_02.png" width="800" title="#HfcQGIS"></a>
</p>

**OTTENGO ALTRO LAYER**

--

## Usando il field calc

Aggiungo il campo nel layer (molto più utile, no??)

<p align="center"> <a href="http://hfcqgis.opendatasicilia.it/it/latest/release/novita_38.html" target="_blank"><img src="./doc/esempi/sj_03.png" width="800" title="#HfcQGIS"></a>
</p>

--

```
aggregate(
    layer:='regioni_g', 
    aggregate:='concatenate', 
    expression:=to_string("DEN_REG"), 
    filter:=contains( $geometry, geometry(@parent) )
        )
```

--

### Esempio2 - Spatial Join

Conta punti nel poligono:

<p align="center"> <a href="http://hfcqgis.opendatasicilia.it/it/latest/release/novita_38.html" target="_blank"><img src="./doc/esempi/sj_04.png" width="700" title="#HfcQGIS"></a>
</p>

--

```
aggregate(
    layer:='punti',
    aggregate:='count', 
    expression:="id", 
    filter:=intersects( $geometry, geometry(@parent))
        )
```
