Datensatzdokumentation
# AKTIN - Daten zur Aufenthaltsdauer in Notaufnahmen    

<br>
<br>
<br>

**[AKTIN-Notaufnahmeregister](http://aktin.org)**&sup1; und **[Robert Koch-Institut](http://www.rki.de)**

<br>

**Beteiligte**  
Susanne Drynda&sup1;, Ronny Otto&sup1;, Wiebke Schirrmeister&sup1;, Jonas Bienzeisler&sup2;, Alexander Kombeiz&sup2;, [Madlen Schranz](https://orcid.org/0000-0002-2426-5770)&sup3;, [Theresa Kocher](https://orcid.org/0000-0002-9300-6625)&#8308;

<br>

&emsp;&emsp;&sup1; Otto-von-Guericke Universität Magdeburg | Medizinische Fakultät  
&emsp;&emsp;&sup2; Universitätsklinik RWTH Aachen | Institut für medizinische Informatik   
&emsp;&emsp;&sup3; Robert Koch-Institut | Fachgebiet 32     
&emsp;&emsp;&#8308; Robert Koch-Institut | Fachgebiet MF2    

-----
**Zitieren**
<!-- CITATION_START: {"citation_style": "apa"} -->
AKTIN-Notaufnahmeregister, & Robert Koch-Institut. (2025). AKTIN - Daten zur Aufenthaltsdauer in Notaufnahmen [Data set]. Zenodo. [https://doi.org/10.5281/zenodo.15598286](https://doi.org/10.5281/zenodo.15598286)
<!-- CITATION_END -->


## Einleitung  

Die Belastung von Notaufnahmen hängt von verschiedenen Faktoren ab, wie z.B. der Anzahl der Patienti:innen , der Schwere ihrer Fälle, der Personalsituation und der Kapazität der Intensivbetten. Die durchschnittliche Aufenthaltsdauer in der Notaufnahme kann als Indikator für die Belastungssituation herangezogen werden.  
Der Datensatz „AKTIN - Daten zur Aufenthaltsdauer in Notaufnahmen“ enthält aggregierte Daten der Routinedokumentation aus einer Auswahl deutscher Notaufnahmen aus dem AKTIN-Notaufnahmeregister. Zur Erfassung der speziellen Belastungssituation während der COVID-19-Pandemie werden im vorliegenden Datensatz Daten zur durchschnittliche Aufenthaltsdauer von Patienti:innen in den Notaufnahmen bereitgestellt und mit den Werten vor der Pandemie verglichen.

## Informationen zum Datensatz und Entstehungskontext  

Um die Belastungssituation in Notaufnahmen abzubilden, kann die durchschnittliche Aufenthaltsdauer in der Notaufnahme innerhalb der letzten Woche als „Surrogatparameter“ herangezogen werden. In die Berechnung der Aufenthaltsdauer (length of stay, LOS) fließt der erste dokumentierte Kontakt in der Notaufnahme (in der Regel der Zeitpunkt der administrativen Aufnahme) und der Zeitpunkt der Entlassung aus der Notaufnahme ein. Um die spezielle Belastungssituation während der COVID-19-Pandemie abzubilden, wird die durchschnittliche Aufenthaltsdauer der jeweils letzten Wochen mit der durchschnittlichen Aufenthaltsdauer vor der Pandemie ins Verhältnis gesetzt. Dazu wird ein gewichteter Mittelwert mit Daten aus den Jahren 2017 bis 2019 berechnet. Eine längere Aufenthaltsdauer (im Vergleich zum gewichteten vor-pandemischen Mittelwert) weist auf eine höhere Belastung und eine kürzere auf eine geringere Belastung hin. 

### Administrative und organisatorische Angaben  

Die Verarbeitung, Aufbereitung und Veröffentlichung der Daten erfolgen durch das [Fachgebiet MF 4 | Informations- und Forschungsdatenmanagement](https://www.rki.de/DE/Institut/Organisation/Abteilungen/MFI/MF4/mf4-fach-und-forschungsdatenmanagement-node.html). Fragen zum Datenmanagement und zur Publikationsinfrastruktur können an das Open Data-Team des Fachgebiets MF4 unter [OpenData@rki.de](mailto:opendata@rki.de) gerichtet werden. Das Monitoring der Notaufnahme-spezifischen Datenqualität und etwaige Abstimmungen mit den Notaufnahmen erfolgt im AKTIN Trusted Data Analyzing Center (TDAC). Für den Kontakt und Koordination der teilnehmenden Notaufnahmen ist das AKTIN-Office verantwortlich. Bei Fragen kann sich an [office@aktin.org](mailto:office@aktin.org) gewendet wenden.

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

<!-- DATA_SCHEMA_SPECIFICATION_START: {"id": "Notaufnahme_Aufenthaltsdauer", "lang": "de"} -->

Die Datei [Notaufnahme_Aufenthaltsdauer.csv](https://github.com/robert-koch-institut/AKTIN_Daten_zur_Aufenthaltsdauer_in_Notaufnahmen/blob/main/Notaufnahme_Aufenthaltsdauer.csv) enthält die in der folgenden Tabelle abgebildeten Variablen und deren Ausprägungen. Ein maschinenlesbares Datenschema ist im [Data Package Standard](https://datapackage.org/) in [tableschema_Notaufnahme_Aufenthaltsdauer.json](https://github.com/robert-koch-institut/AKTIN_Daten_zur_Aufenthaltsdauer_in_Notaufnahmen/blob/main/Metadaten/schemas/tableschema_Notaufnahme_Aufenthaltsdauer.json) hinterlegt:
> [tableschema_Notaufnahme_Aufenthaltsdauer.json](https://github.com/robert-koch-institut/AKTIN_Daten_zur_Aufenthaltsdauer_in_Notaufnahmen/blob/main/Metadaten/schemas/tableschema_Notaufnahme_Aufenthaltsdauer.json)

<!-- DATA_SCHEMA_TABLE_START -->
| Variable       | Typ     | Ausprägungen                | Beschreibung                                                                                              |
|:---------------|:--------|:----------------------------|:----------------------------------------------------------------------------------------------------------|
| date           | date    | Format: `YYYY-Www`          | Berichtswoche der Daten der Aufenthaltsdauer im ISO-8106 Format                                           |
| ed_count       | integer | Werte: `≥11`                | Anzahl meldender Notaufnahmen in der Berichtswoche                                                        |
| visit_mean     | number  | Werte: `≥1`                 | Durchschnittliche Anzahl Vorstellungen in der Berichtswoche pro Notaufnahme, gerundet auf ganze Zahlen    |
| los_mean       | number  | Werte: `≥1`                 | Gewichtete durchschnittliche Aufenthaltsdauer in der Berichtswoche in Minuten                             |
| los_reference  | number  | Werte: `≥1`                 | Gewichteter Mittelwert der Aufenthaltsdauer, berechnet aus Daten der Jahre 2017 bis 2019                  |
| los_difference | number  |                             | Abweichung der los_mean von der los_reference                                                             |
| change         | string  | Werte: `Zunahme`, `Abnahme` | Interpretation der Variable „los_difference“. Wenn los_difference < 0, dann Abnahme, andernfalls Zunahme. |

<!-- DATA_SCHEMA_TABLE_END -->

<!-- DATA_SCHEMA_SPECIFICATION_END -->


#### Formatierung der Daten  

Die Notaufnahmesurveillance-Daten sind im Datensatz als kommaseparierte .csv-Datei enthalten. Der verwendete Zeichensatz der .csv-Datei ist UTF-8. Trennzeichen der einzelnen Werte ist ein Komma ",". Datumsangaben sind im ISO-8601-Standard formatiert.  

- Zeichensatz: UTF-8  
- Datumsformat: ISO 8601  
- .csv-Trennzeichen: Komma ","  

<!-- FOOTER_START: {"lang": "de"} -->



### Metadaten  

Zur Erhöhung der Auffindbarkeit sind die bereitgestellten Daten mit Metadaten beschrieben. Über GitHub Actions werden Metadaten an die entsprechenden Plattformen verteilt. Für jede Plattform existiert eine spezifische Metadatendatei, diese sind im Metadatenordner hinterlegt:  

> [Metadaten/](https://github.com/robert-koch-institut/AKTIN_Daten_zur_Aufenthaltsdauer_in_Notaufnahmen/tree/main/Metadaten/) 

Versionierung und DOI-Vergabe erfolgt über [Zenodo.org](https://zenodo.org). Die für den Import in Zenodo bereitgestellten Metadaten sind in der [zenodo.json](https://github.com/robert-koch-institut/AKTIN_Daten_zur_Aufenthaltsdauer_in_Notaufnahmen/blob/main/Metadaten/zenodo.json) hinterlegt. Die Dokumentation der einzelnen Metadatenvariablen ist unter https://developers.zenodo.org/#representation nachlesbar.
 
> [Metadaten/zenodo.json](https://github.com/robert-koch-institut/AKTIN_Daten_zur_Aufenthaltsdauer_in_Notaufnahmen/blob/main/Metadaten/zenodo.json)  

In der zenodo.json ist neben dem Publikationsdatum (`"publication_date"`) auch der Datenstand in folgendem Format enthalten (Beispiel):  

```
  "dates": [
    {
      "start": "2023-09-11T15:00:21+02:00",
      "end": "2023-09-11T15:00:21+02:00",
      "type": "Collected",
      "description": "Date when the Dataset was created"
    }
  ],
```    


Zusätzlich beschreiben wir tabellarische Daten mithilfe des [Data Package Standards](https://datapackage.org/).
Ein Data Package ist eine strukturierte Sammlung von Daten und zugehörigen Metadaten, die den Austausch und die Wiederverwendung von Daten erleichtert. Es besteht aus einer datapackage.json-Datei, die zentrale Informationen wie die enthaltenen Ressourcen, ihre Formate und Schema-Definitionen beschreibt.

Der Data Package Standard wird von der [Open Knowledge Foundation](https://okfn.org/) bereitgestellt und ist ein offenes Format, das eine einfache, maschinenlesbare Beschreibung von Datensätzen ermöglicht.

Die Liste der in diesem Repository enthaltenen Daten ist in folgender Datei hinterlegt:

> [datapackage.json](https://github.com/robert-koch-institut/AKTIN_Daten_zur_Aufenthaltsdauer_in_Notaufnahmen/tree/main/datapackage.json)

Für tabellarische Daten definieren wir zusätzlich ein [Table Schema](https://datapackage.org/standard/table-schema/), das die Struktur der Tabellen beschreibt, einschließlich Spaltennamen, Datentypen und Validierungsregeln. Diese Schema-Dateien finden sich unter:

> [Metadaten/schemas/](https://github.com/robert-koch-institut/AKTIN_Daten_zur_Aufenthaltsdauer_in_Notaufnahmen/tree/main/Metadaten/schemas) 



## Hinweise zur Nachnutzung der Daten  

Offene Forschungsdaten des RKI werden auf [Zenodo.org](http://Zenodo.org/), [GitHub.com](http://GitHub.com/), [OpenCoDE](https://gitlab.opencode.de) und [Edoc.rki.de](http://Edoc.rki.de/) bereitgestellt:  

- https://zenodo.org/communities/robertkochinstitut  
- https://github.com/robert-koch-institut  
- https://gitlab.opencode.de/robert-koch-institut  
- https://edoc.rki.de/  
 
### Lizenz  

Der Datensatz "AKTIN - Daten zur Aufenthaltsdauer in Notaufnahmen" ist lizenziert unter der [Creative Commons Namensnennung 4.0 International Public License | CC-BY 4.0 International](https://creativecommons.org/licenses/by/4.0/deed.de).  

Die im Datensatz bereitgestellten Daten sind, unter Bedingung der Namensnennung des Robert Koch-Instituts als Quelle, frei verfügbar. Das bedeutet, jede Person hat das Recht die Daten zu verarbeiten und zu verändern, Derivate des Datensatzes zu erstellen und sie für kommerzielle und nicht kommerzielle Zwecke zu nutzen. Weitere Informationen zur Lizenz finden sich in der [LICENSE](https://github.com/robert-koch-institut/AKTIN_Daten_zur_Aufenthaltsdauer_in_Notaufnahmen/blob/main/LICENSE) bzw. [LIZENZ](https://github.com/robert-koch-institut/AKTIN_Daten_zur_Aufenthaltsdauer_in_Notaufnahmen/blob/main/LIZENZ) Datei des Datensatzes.  
<!-- FOOTER_END -->
