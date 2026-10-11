# Datensatz: Smartphone
### Beschreibt mein Smartphone.

## Felder  
`Smartphonename` (Text)- Name des Smartphones  
`Preis in Euro` (Zahl)- Preis des Smarphones  
`Auf Lager` (Wahrheitswert) - aktell verfügbar?  
`Farben` (Liste von Text) - welche Farben gibt es?  
`Kategorie` (Text)  
`Bildschirmauflösung` in Pixel (Objekt) - mit `Bildpunkte in Höhe` und `Breite`  

## Als JSON (`daten.jason`)    
```JSON
{
"Smartphone Name": "Samsung Galaxy S20",  
"Preis in EUR": 163,  
"Auf Lager": true,  
"Farben": [  
"Schwarz",  
"Weiß"  
],
"Kategorie": "Smartphone",  
"Bildschirmauflösung in Pixel":  
{  
"Bildpunkte in der Breite": 3200,  
"Bildpunkte in der Höhe": 1440  
}   
}  
``` 
  
## Als YML (`daten.yml`)  
```yaml
# Smartphone im Shop
Smartphone Name: Samsung Galaxy S20
Preis in Euro: 163
Auf Lager: true
Farben:
- Schwarz
- Weiß
  Kategorie: Smartphone
  Bildschirmauflösung in Pixel:
  Bildpunkte in der Breite: 3200
  Bildpunkte in der Höhe: 1440  
```




