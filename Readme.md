Datensatzdokumentation
# AKTIN - Daten zur Aufenthaltsdauer in Notaufnahmen  

**[AKTIN-Notaufnahmeregister](http://aktin.org)**  
*<sup>1</sup> AKTIN-Geschäftsstelle und TDAC*  
c/o Otto-von-Guericke Universität Magdeburg  
Universitätsklinik für Unfallchirurgie  
Leipziger Straße 44  
39120 Magdeburg  

*<sup>2</sup> AKTIN-IT*  
c/o Institut für medizinische Informatik  
Uniklinik RWTH Aachen  
Pauwelsstraße 30  
52057 Aachen  
  
**[Robert Koch-Institut | RKI](http://www.rki.de)**  
*<sup>3</sup> Fachgebiet 32 | Surveillance und elektronisches Melde- und Informationssystem (DEMIS) | ÖGD Kontaktstelle*  
*<sup>4</sup> Fachgebiet MF4 | Informations- und Forschungsdatenmanagement*  
Nordufer 20  
13353 Berlin  


**Beitragende Personen**  

Susanne Drynda<sup>1</sup>, Ronny Otto<sup>1</sup>, Wiebke Schirrmeister<sup>1</sup>, Jonas Bienzeisler<sup>2</sup>, Alexander Kombeiz<sup>2</sup>, [Madlen Schranz](https://orcid.org/0000-0002-2426-5770)<sup>3</sup>, [Theresa Kocher](https://orcid.org/0000-0002-9300-6625)<sup>4</sup>

-----
**Zitieren**

AKTIN-Notaufnahmeregister und Robert Koch-Institut (2023): AKTIN – Daten zur Aufenthaltsdauer in Notaufnahmen, Berlin: Zenodo. DOI: [10.5281/zenodo.7711112](https://doi.org/10.5281/zenodo.7711112)  

## Einleitung  

Die Belastung von Notaufnahmen hängt von verschiedenen Faktoren ab, wie z.B. der Anzahl der Patienti:innen , der Schwere ihrer Fälle, der Personalsituation und der Kapazität der Intensivbetten. Die durchschnittliche Aufenthaltsdauer in der Notaufnahme kann als Indikator für die Belastungssituation herangezogen werden.  
Der Datensatz „AKTIN - Daten zur Aufenthaltsdauer in Notaufnahmen“ enthält aggregierte Daten der Routinedokumentation aus einer Auswahl deutscher Notaufnahmen aus dem AKTIN-Notaufnahmeregister. Zur Erfassung der speziellen Belastungssituation während der COVID-19-Pandemie werden im vorliegenden Datensatz Daten zur durchschnittliche Aufenthaltsdauer von Patienti:innen in den Notaufnahmen bereitgestellt und mit den Werten vor der Pandemie verglichen.

## Informationen zum Datensatz und Entstehungskontext  

Um die Belastungssituation in Notaufnahmen abzubilden, kann die durchschnittliche Aufenthaltsdauer in der Notaufnahme innerhalb der letzten Woche als „Surrogatparameter“ herangezogen werden. In die Berechnung der Aufenthaltsdauer (length of stay, LOS) fließt der erste dokumentierte Kontakt in der Notaufnahme (in der Regel der Zeitpunkt der administrativen Aufnahme) und der Zeitpunkt der Entlassung aus der Notaufnahme ein. Um die spezielle Belastungssituation während der COVID-19-Pandemie abzubilden, wird die durchschnittliche Aufenthaltsdauer der jeweils letzten Wochen mit der durchschnittlichen Aufenthaltsdauer vor der Pandemie ins Verhältnis gesetzt. Dazu wird ein gewichteter Mittelwert mit Daten aus den Jahren 2017 bis 2019 berechnet. Eine längere Aufenthaltsdauer (im Vergleich zum gewichteten vor-pandemischen Mittelwert) weist auf eine höhere Belastung und eine kürzere auf eine geringere Belastung hin. 

### Administrative und organisatorische Angaben  

Die Verarbeitung, Aufbereitung und Veröffentlichung der Daten erfolgen durch das [Fachgebiet MF 4 | Informations- und Forschungsdatenmanagement](https://www.rki.de/DE/Content/Institut/OrgEinheiten/MF/MF4/mf4_node.html). Fragen zum Datenmanagement und zur Publikationsinfrastruktur können an das Open Data-Team des Fachgebiets MF4 unter [OpenData@rki.de](mailto:opendata@rki.de) gerichtet werden. Das Monitoring der Notaufnahme-spezifischen Datenqualität und etwaige Abstimmungen mit den Notaufnahmen erfolgt im AKTIN Trusted Data Analyzing Center (TDAC). Für den Kontakt und Koordination der teilnehmenden Notaufnahmen ist das AKTIN-Office verantwortlich. Bei Fragen kann sich an [office@aktin.org](mailto:office@aktin.org) gewendet wenden.

## Datenerhebung und Datenverarbeitung  

Die zugrundeliegenden Daten aus der Routinedokumentation von Notaufnahmen werden im Rahmen des AKTIN-Notaufnahmeregisters erhoben ([Brammen et al. 2020](https://doi.org/10.1007/s00063-020-00764-2)) und anschließend dem RKI als tägliche Datenlieferungen über eine SFTP-Server-API täglich bereitgestellt. 

> Brammen, D., Greiner, F., Kulla, M. et al. Das AKTIN-Notaufnahmeregister – kontinuierlich aktuelle Daten aus der Akutmedizin. Med Klin Intensivmed Notfmed 117, 24–33 (2022). DOI: [10.1007/s00063-020-00764-2](https://doi.org/10.1007/s00063-020-00764-2) 

### Datengrundlage und Datenqualität

Die Auswahl der Notaufnahmen basiert auf der individuellen Bereitschaft zur Teilnahme.

Unplausible Werte werden aus der Berechnung ausgeschlossen (LOS < 1 min, >24 h). Notaufnahmen, bei denen die dokumentierten Zeitpunkte nicht plausibel sind oder eine fehlende Dokumentation der für die Berechnung erforderlichen Zeitpunkte von mehr als 20% aufweisen, werden ebenfalls ausgeschlossen.

## Inhalt und Aufbau des Datensatzes  

Der Datensatz enthält aggregierte Daten aus der Routinedokumentation aus einer Auswahl deutscher Notaufnahmen. Im Datensatz enthalten sind:

- Aggregierte Daten zur Aufenthaltsdauer von Patienti:innen in teilnehmenden Notaufnahmen  
- Datensatzdokumentation in deutscher Sprache  
- Lizenzdatei mit Daten-Nutzungsbedingungen  
- Metadaten zum Datensatz  

Die Daten werden wöchentlich Donnerstags aktualisiert und enthalten alle zum Berichtsdatum verfügbaren Informationen der vorherigen Berichtswoche.

### Aufenthaltsdauer in teilnehmenden Notaufnahmen  

Die Datei "Notaufnahme_Aufenthaltsdauer.csv" enthält die Daten zur durchschnittlichen Aufenthaltsdauer aller teilnehmenden Notaufnahmen. 

> [Notaufnahme_Aufenthaltsdauer.csv](/Notaufnahme_Aufenthaltsdauer.csv)

#### Variablen und Variablenausprägungen

Die Daten enthalten folgende Variablen mit ihren entsprechenden Ausprägungen:  

|Variable|Typ|Ausprägung|Erläuterung|
| - | - | - | - |
|date|Datum|`yyyy-Www`|Berichtswoche der Daten der Aufenthaltsdauer im ISO-8106 Format|
|ed_count|Ganze Zahl|`>10`|Anzahl meldender Notaufnahmen in der Berichtswoche|
|los_mean|Dezimalzahl||Durchschnittliche Aufenthaltsdauer in der Berichtswoche, in Minuten.|
|los_reference|Dezimalzahl||Gewichteter Mittelwert der Aufenthaltsdauer, berechnet aus Daten der Jahre 2017 bis 2019.|
|los_difference|Dezimalzahl||Differnez der durchschnittlichen Aufenthaltsdauer in der Berichtswoche zum gewichteten Mittelwert, in Minuten.|
|change|Text|`Zunahme`, `Abnahme`|Interpretation der Variable „los_difference“. Wenn los_difference < 0, dann Abnahme, andernfalls Zunahme.|

#### Formatierung der Daten  

Die Notaufnahmesurveillance-Daten sind im Datensatz als kommaseparierte .csv-Datei enthalten. Der verwendete Zeichensatz der .csv-Datei ist UTF-8. Trennzeichen der einzelnen Werte ist ein Komma ",". Datumsangaben sind im ISO-8601-Standard formatiert.  

- Zeichensatz: UTF-8  
- Datumsformat: ISO 8601  
- .csv-Trennzeichen: Komma ","  


### Metadaten  

Zur Erhöhung der Auffindbarkeit sind die bereitgestellten Daten mit Metadaten beschrieben. Über GitHub Actions werden Metadaten an die entsprechenden Plattformen verteilt. Für jede Plattform existiert eine spezifische Metadatendatei, diese sind im Metadatenordner hinterlegt:

> [Metadaten/](/Metadaten/)  

Versionierung und DOI-Vergabe erfolgt über [Zenodo.org](https://zenodo.org). Die für den Import in Zenodo bereitgestellten Metadaten sind in der [zenodo.json](/Metadaten/zenodo.json) hinterlegt. Die Dokumentation der einzelnen Metadatenvariablen ist unter https://developers.zenodo.org/#representation nachlesbar.   

> [Metadaten/zenodo.json](/Metadaten/zenodo.json)  

## Hinweise zur Nachnutzung der Daten  

Offene Forschungsdaten des RKI werden auf [GitHub.com](http://GitHub.com/), [Zenodo.org](http://Zenodo.org/) und [Edoc.rki.de](http://Edoc.rki.de/) bereitgestellt:

- [https://github.com/robert-koch-institut](https://github.com/robert-koch-institut)  
- [https://zenodo.org/communities/robertkochinstitut](https://zenodo.org/communities/robertkochinstitut)  
- [https://edoc.rki.de](https://edoc.rki.de/)  

### Lizenz  

Der Datensatz "AKTIN - Daten zur Aufenthaltsdauer in Notaufnahmen" ist lizenziert unter der [Creative Commons Namensnennung 4.0 International Public License | CC-BY 4.0 International](https://creativecommons.org/licenses/by/4.0/deed.de).  

Die im Datensatz bereitgestellten Daten sind, unter Bedingung der Namensnennung der Quelle, frei verfügbar. Das bedeutet, jede Person hat das Recht die Daten zu verarbeiten und zu verändern, Derivate des Datensatzes zu erstellen und sie für kommerzielle und nicht kommerzielle Zwecke zu nutzen. Weitere Informationen zur Lizenz finden sich in der [LICENSE](/LICENSE) bzw. [LIZENZ](/LIZENZ) Datei des Datensatzes.  
