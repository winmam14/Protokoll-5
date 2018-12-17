# Protokoll 5
## Thema: Thema: Schnittstellen und Feldbus
**Professor:** SX  
**Übungsdatum:** 11.12.2018  
**Author, KNr.:** Winter Matthias, 17  
**Anwesend:** Sarah Vezonik, Alois Vollmaier, Patrick Wegl, Mercedes Wesonig, Winter Matthias, Winter Thomas  

---

## Stundenübersicht
#### 1. Schnittstellen
##### 1.1 Echtzeitfähige Schnittstllen
##### 1.2 Nicht Echtzeitfähige Schnittstellen
#### 3. Feldbus
#### 4. Modbus-Protokoll

--- 

## 1. Schnittstellen
Eine Schnittstelle dient zur Komunikation verschiedener Systeme oder einzelner Komponenten. Der Austausch von Informationen erfolgt in Form von physikalischen oder logischen Größen (Daten) und kann analog oder digital erfolgen. Eine Schnittstelle wird durch eine Menge von Eigenschaften beschrieben. Wenn diese Eigenschaften mit einer anderen Schnittstelle übereinstimm kann man Komponenten und Module gegeneinander austauschen. Dafür gibt es mehrere verschiedene Standarts.

### 1.1 Echtzeitfähige Schnittstellen
Echtzeitfähigkeit bedeutet, dass die Übertragung von Daten immer verlässlich innerhalb einer festgelegten Zeit erfolgen kann.
Ein Beispiele für eine echtzeitfähige Schnittstelle ist **S485**.  

### 1.1.1 RS485
Die **RS485-Schnittstelle** ist eine aufwandsarme serielle Schnittstelle für die Datenkommunikation über große Entfernungen. Sie stellt ein bidirektional nutzbares Bussystem dar, das mit bis zu **128 Geräten** an einem Bus betrieben werden kann. Die Datenübertragung erfolgt symmetrisch, massefrei als Spannungsdifferenz (Differenz: < -0,3 V = H, > +0,3 V = L) zwischen den beiden Busleitungen A (invertierte Leitung) und B (nicht invertierte Leitung), so können sich Gleichtaktstörungen auf der Leitung nicht störend auswirken. Wichtig ist ein Abschluss der Leitung an jedem Ende des Busses mit einem Abschlusswiderstand von 120 Ω.
  ![alt text](https://files.elv.com/bilder/elvexpertenwissen/gross/rs485_bus01.jpg)

### 1.2 Nicht Echtzeitfähige Schnittstellen
Keine Echtzeitfähigkeit bedeutet, dass die Übertragung von Daten nicht immer verlässlich innerhalb einer festgelegten Zeit erfolgen kann. Ein Beispiel für eine Schnittstelle die nicht echtzeitfähig ist, ist **Ethernet**(kabelgebunden oder kabellos).

### 1.2.1 Ethernet
Ethernet finded verwendung wenn man sehr große Datenmengen hat die man übertrage muss, es jedoch nicht sehr schlimm ist wenn man keine Echtzeitfähigkeit hat. Ethernet kann aber mit ein paar Modifikationen echtzeitfähig gemacht werden. Hersteller die ihr eigens echtzeitfähiges Ethernet bereits entwickelt haben sind zum Beispiel B&R mit **"Power Link"** und Profinet.

## 3. Feldbus
Feldbus ist ein Bussystem welches zur Komunikation von Sensoren und Aktoren verwendet wird. Wenn mehrere Kommunikationsteilnehmer ihre Nachrichten über dieselbe Leitung senden, dann muss festgelegt sein, **wer** (Kennung), **was** (Messwert, Befehl), **wann** (Initiative), sagt. Hierfür gibt es normierte **Protokolle**.
![alt text]()

## 4. Modbus-Protokoll
