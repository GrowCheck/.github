# GrowCheck

GrowCheck ist ein innovatives System, das entwickelt wurde, um die Gesundheit und das Wachstum Ihrer Pflanzen zu Hause zu überwachen. Unser Sensor erfasst verschiedene Umweltparameter und sendet diese Informationen an unseren Server, wo sie visualisiert und analysiert werden können. 

## Funktionen

GrowCheck verwendet hochentwickelte Sensoren, um die folgenden Informationen zu erfassen:

### 1. Soil Fertility Detection
**Beschreibung:** Misst den Nährstoffgehalt des Bodens.
**Nutzen:** Hilft festzustellen, ob der Boden genügend Nährstoffe enthält, um das Pflanzenwachstum zu unterstützen.

### 2. Soil Moisture Detection
**Beschreibung:** Erfasst den Feuchtigkeitsgehalt im Boden.
**Nutzen:** Ermöglicht die Optimierung der Bewässerung, um sicherzustellen, dass Pflanzen weder austrocknen noch ertrinken.

### 3. Light Intensity Detection
**Beschreibung:** Misst die Intensität des einfallenden Lichts.
**Nutzen:** Hilft festzustellen, ob Pflanzen ausreichend Licht erhalten, was für die Photosynthese entscheidend ist.

### 4. Ambient Temperature and Humidity
**Beschreibung:** Misst die Umgebungstemperatur und Luftfeuchtigkeit.
**Nutzen:** Ermöglicht die Überwachung der klimatischen Bedingungen, die das Wachstum und die Gesundheit der Pflanzen beeinflussen.

## Systemarchitektur

### Sensor-Kommunikation
Die Sensoren kommunizieren über Zigbee mit dem Gateway. Zigbee ist ein energieeffizientes, drahtloses Mesh-Netzwerkprotokoll, das für die Kommunikation zwischen Geräten in einem Nahbereich verwendet wird.

### Gateway
Das Gateway empfängt die Daten von den Sensoren und überträgt sie über WLAN an den Router. Es fungiert als Brücke zwischen den Zigbee-Sensoren und dem Heimnetzwerk.

**Vorteile eines Gateways:**
- **Weniger Traffic:** Reduziert die Belastung des Hauptnetzwerks durch lokale Datenaggregation.
- **Einfache Paarung:** Erleichtert die Verbindung und Verwaltung von Sensoren.

**Nachteile eines Gateways:**
- **Mehr Geräte:** Erfordert zusätzliche Hardware im Netzwerk.
- **Mehr Kosten:** Zusätzliche Anschaffungskosten für das Gateway.
- **Mehr Strom:** Erhöhter Energieverbrauch durch das zusätzliche Gerät.

### Router
Der Router verbindet das Gateway mit dem Internet und ermöglicht die Kommunikation mit dem MQTT-Message-Broker. WLAN (Wi-Fi) ist ein Standard für die drahtlose Verbindung von Geräten innerhalb eines lokalen Netzwerks.

### MQTT-Message-Broker
MQTT (Message Queuing Telemetry Transport) ist ein leichtgewichtiges Publish-Subscribe-Netzwerkprotokoll, das ideal für die Übertragung von Sensordaten in IoT-Anwendungen geeignet ist. Der MQTT-Message-Broker empfängt die Sensordaten und stellt sie zur weiteren Verarbeitung und Visualisierung bereit.

## Installation

1. Verbinden Sie die Sensoren mit dem Zigbee-Gateway.
2. Stellen Sie das Gateway in der Nähe der Sensoren auf.
3. Verbinden Sie das Gateway über WLAN mit Ihrem Router
4. Greifen Sie über das Dashboard auf die visualisierten Sensordaten zu.

## Visualisierung und Analyse
Nach der Einrichtung können Sie die Daten über unser benutzerfreundliches Dashboard visualisieren. Die Visualisierung hilft Ihnen, Trends zu erkennen und fundierte Entscheidungen zur Pflanzenpflege zu treffen.

---

**GrowCheck**
****
