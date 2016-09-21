# baufi
Vergleich von verschiedenen Baufinanzierungen. Bereitstellungszinsen sind nicht im effektiven Jahreszins inbegriffen. Die Bereitstellungszinsen werden oft vernachlässigt, obwohl der Bereitstellungszins mit 3% p.a. höher ist als der eigentliche Sollzins.

Die Bereitstellungszinsfreie Zeit sowie die Höhe des Zins variiert von Bank zu Bank. Besonders relevant wird das, wenn man eine Immobilie baut, wobei nach Baufortschritt bezahlt wird.

# Input

## Bauvorhaben
Das Bauvorhaben besteht aus Ratenzahlungen an den Bauträger. Jede Rate ist ein Tupel aus Datum und Betrag der Rate.

## Finanzierung
Die Finanzierung besteht aus einer Liste von Krediten.

### Kredit
Ein Kredit ist definiert durch:
- Betrag (Euro)
- Sollzinssatz (%)
- Beginn (Datum)
- Tilgungssatz (%)
- Tilgungsbeginn (Datum)
- Bereitstellungszinssatz (%)
- Bereitstellungszinsbeginn (Datum)
- Sollzinsbindung (Jahre)

# Output
Der Finanzierungsverlauf wird ausgegeben, so dass die monatliche Belastung inklusive Bereitstellungszins dargestellt wird. Ebenso wird die Gesamtsumme / Gesamtkosten des Kreditvertrags angezeigt.
