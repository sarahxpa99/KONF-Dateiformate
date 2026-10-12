# Datensatz: Smartphone
### Beschreibt ein Smartphone im Warenkorb.

## Felder  
`Smartphonename` (Text)- Name des Smartphones  
`Preis in Euro` (Zahl)- Preis des Smarphones  
`Auf Lager` (Wahrheitswert) - aktell verfügbar?  
`Farben` (Liste von Text) - welche Farben gibt es?  
`Kategorie` (Text)  
`Bildschirmauflösung` in Pixel (Objekt) - mit `Bildpunkte in Höhe` und `Bildpunkte in Breite`  

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

## Als XML (`daten.xml`)  
```xml  
<?xml version="1.0" encoding="UTF-8"?>
<produkt>
    <SmartphoneName>Samsung Galaxy S20</SmartphoneName>
    <PreisinEur>163</PreisinEur>
    <AufLager>true</AufLager>
    <Farben>
        <Farbe>Schwarz</Farbe>
        <Farbe>Weiß</Farbe>
    </Farben>
    <BildschrimAuflösunginPixel>
        <BilpunkteBreite>3200</BilpunkteBreite>
        <BildpunkteHöhe>1440</BildpunkteHöhe>
    </BildschrimAuflösunginPixel>
</produkt>
```  
## Als CSV (`daten.csv`)  
```csv
Smartphone Name,Preis in EUR,Auf Lager,Farben,Kategorie,Bildpunkte Breite,Bildpunkte Höhe
Samsung Galaxy S20,163,True,Schwarz | Weiß,Smartphone,3200,1440
```