# Datensatz: Smartphone
### Beschreibt ein Smartphone im Warenkorb.

## Felder  
`Smartphonename` (Text)- Name des Smartphones  
`Preis in Euro` (Zahl)- Preis des Smarphones  
`Auf Lager` (Wahrheitswert) - aktell verfügbar?  
`Farben` (Liste von Text) - welche Farben gibt es?  
`Kategorie` (Text)  - zu welcher Kategorie zählt der Artikel?  
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

# Reflexion  
Das Format das mir am schwertsten viel war XML, da mann immer darauf achten muss,  
dass man die Tags paarweise andwendet. Also eines zu Öffnen und eines zum Abschließen.
Außerdem ist es ein wenig mühsam, dass man bei YML sehr penibel bei den Leerzeichen sein muss.  

Bei CVS habe ich die verschachtelte Liste einfach in eine Spalte geschrieben und mit | getrennt.  
Für den Menschen ist es zwar eindeutig lesbar, dass es sich hier um zwei verfügbare Farben handelt,  
für einen Computer ist es aber nicht ersichtlich, dass es sich dabei um zwei verschiedene Listenelmenete handelt.   

Bei dem verschachteltem Objekt hat man ein ähnliches Problem, hier habe ich zwar "Bildpunkte in Höhe" und   
"Bildpunkte in Breite" in zwei verschiedenen Spalten definiert, jedoch geht so die Überschrift  
"Bildschirmauflösung in Pixel" verloren. Ein Computer würde nicht erkenne, dass es sich hier um "echte Unterfelder" handelt.   

Ein XSD Schema wäre bei der Übermittlung der XML Datei hilfreich.  
ISD Schemen legt fest, welche Datentypen, Elemente und Reihenfolgen erlabt sind. Also zB. dass der Preis in EUR sein muss.   
Bei der Zusammebarbeit von zwei verschiedenen Firmen sind solche "Regeln" sehr wertvoll


