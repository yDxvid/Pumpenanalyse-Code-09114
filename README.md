# Pumpenanalyse mit CSV-Messdaten Code: 09114

## Fünfstelliger Code

Fünfstelliger Code für die Bewertung: 09114

---

## Kurs

Kurs: TMB23PT DHBW Karlsruhe

---

## Projektbeschreibung

Dieses Projekt analysiert den Betrieb einer Wasserpumpe anhand von Messdaten aus einer CSV-Datei.  
Die Messwerte enthalten den Volumenstrom der Pumpe über die Zeit. Mithilfe einer vorgegebenen Pumpenkennlinie werden daraus Förderhöhe, Leistung, Wirkungsgrad und Energieverbrauch bestimmt.

Die Auswertung erfolgt mit Python und wird in einem Jupyter Notebook visualisiert.

---

## Verwendete Technologien

- Python
- Jupyter Notebook
- pandas
- numpy
- matplotlib

---

## Vorgehensweise

1. Einlesen der CSV-Messdaten
2. Umrechnung und Aufbereitung der Messwerte
3. Interpolation der Pumpenkennlinie
4. Bestimmung von:
   - Förderhöhe
   - hydraulischer Leistung
   - elektrischer Leistung
   - Pumpenwirkungsgrad
   - Gesamtwirkungsgrad
   - Energieverbrauch
5. Glättung der Messwerte zur besseren Darstellung
6. Visualisierung der Ergebnisse in Diagrammen

---

## Verwendete Grundlagen

Für die Berechnung der hydraulischen Leistung wird folgende Formel verwendet:

P_hyd = rho * g * V * H

mit:

- rho = Dichte von Wasser
- g = Erdbeschleunigung
- V = Volumenstrom
- H = Förderhöhe

Zusätzlich wird der Motorwirkungsgrad berücksichtigt.

---

## Ergebnisse und Diagramme

### 1. Pumpenkennlinie und Betriebspunkt

Das Diagramm zeigt die verwendete 269-mm-Kennlinie der Pumpe sowie den markierten Betriebspunkt.  
Die markierte Fläche stellt die hydraulische Leistung dar.

Aussage:
- Zusammenhang zwischen Volumenstrom und Förderhöhe
- Darstellung des gewählten Arbeitspunktes der Pumpe

---

### 2. Geglätteter Volumenstrom

Darstellung des zeitlichen Verlaufs des Volumenstroms.

Aussage:
- Schwankungen des Förderstroms im Betrieb
- Erkennung von Laständerungen

---

### 3. Geglättete Leistungen

Vergleich zwischen:
- aufgenommener Pumpenleistung
- hydraulischer Nutzleistung

Aussage:
- Unterschied zwischen eingesetzter und nutzbarer Leistung
- Sichtbare Energieverluste

---

### 4. Wirkungsgrad über der Zeit

Darstellung des geglätteten Pumpenwirkungsgrades.

Aussage:
- Bewertung der Effizienz der Pumpe
- Erkennung effizienter und ineffizienter Betriebsbereiche

---

### 5. Histogramm des Volumenstroms

Zeigt die Häufigkeitsverteilung des Volumenstroms.

Aussage:
- In welchen Betriebsbereichen die Pumpe am häufigsten arbeitet

---

### 6. Heatmap der Betriebspunkte

Darstellung der Häufigkeit verschiedener Betriebspunkte.

Aussage:
- Häufig genutzte Kombinationen aus Volumenstrom und Förderhöhe
- Analyse typischer Betriebszustände

---

### 7. Kumulierter Energieverbrauch

Darstellung des gesamten elektrischen Energieverbrauchs über die Zeit.

Aussage:
- Entwicklung des Energieverbrauchs im Messzeitraum
- Gesamtverbrauch der Anlage

---

### 8. Histogramm des Pumpenwirkungsgrades

Zeigt die Verteilung der Wirkungsgrade.

Aussage:
- Häufigkeit effizienter und ineffizienter Betriebszustände

---

### 9. Verlustleistung über der Zeit

Darstellung der nicht hydraulisch genutzten Leistung.

Aussage:
- Analyse von Energieverlusten
- Bewertung der Betriebseffizienz

---

## Dateien

- `Strömungsmaschinen_Zusatzaufgabe.py` → Python Code
- `Strömungsmaschinen_Zusatzaufgabe.ipynb` → Jupyter Notebook mit Code und Ergebnissen
- `volume_flow_data.csv` → Messdaten
- `README.md` → Projektbeschreibung

---
