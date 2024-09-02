### Variable specification for data file `frictionless_data_schema_Notaufnahme_Aufenthaltsdauer`

| Variable       | Typ     | Ausprägungen                | Beschreibung                                                                                              |
|:---------------|:--------|:----------------------------|:----------------------------------------------------------------------------------------------------------|
| date           | date    | Format: `%Y-W%W`            | Berichtswoche der Daten der Aufenthaltsdauer im ISO-8106 Format                                           |
| ed_count       | integer | Minimum: 11                 | Anzahl meldender Notaufnahmen in der Berichtswoche                                                        |
| visit_mean     | number  | Minimum: 1                  | Durchschnittliche Anzahl Vorstellungen in der Berichtswoche pro Notaufnahme, gerundet auf ganze Zahlen    |
| los_mean       | number  | Minimum: 1                  | Gewichtete durchschnittliche Aufenthaltsdauer in der Berichtswoche in Minuten                             |
| los_reference  | number  | Minimum: 1                  | Gewichteter Mittelwert der Aufenthaltsdauer, berechnet aus Daten der Jahre 2017 bis 2019                  |
| los_difference | number  |                             | Abweichung der los_mean von der los_reference                                                             |
| change         | string  | Werte: `Zunahme`, `Abnahme` | Interpretation der Variable „los_difference“. Wenn los_difference < 0, dann Abnahme, andernfalls Zunahme. |


