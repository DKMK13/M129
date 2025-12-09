# Host-Name / Gerätebezeichnung

## Einführung
Ein **Hostname** ist der eindeutige Name eines Geräts in einem Netzwerk.  
Er vereinfacht Identifikation, Verwaltung und Fehleranalyse.

Beispiele:
- PC-01
- ROUTER-RT1
- SERVER-DB01

---

## Zweck eines Hostnamens
- Geräte eindeutig identifizieren
- DNS kann Hostnamen auflösen
- Hilfreich für Monitoring & Logging
- Erleichtert Fehlersuche („ping pc-01“)

---

## Regeln für Hostnamen
| Regel | Erklärung |
|-------|-----------|
| Keine Leerzeichen | z. B. NICHT: "Mein PC" |
| Wenig Sonderzeichen | Bindestrich ist ok |
| Kurz & eindeutig | z. B. LAB-PC01 |
| Aussagekräftig | Router1 / Switch-Core-01 |

---

## Hostname & DNS
Hostname + Domain = **FQDN**  
Beispiel:  
Hostname: `server1`  
Domain: `schule.local`  
→ FQDN: `server1.schule.local`

---

## Beispiele für gute Benennungen
| Gerät | Hostname |
|-------|----------|
| Router | `R-CORE-01` |
| Server | `SRV-WEB01` |
| PC | `PC-Klasse3-07` |

---

## Merksatz
**Ein Hostname ist der Name, eine IP ist die Adresse.**

---

## Zusammenfassung (Spickzettel)
- Identifiziert Geräte im Netzwerk  
- Muss eindeutig sein  
- Wird oft mit DNS verwendet  
- Unterstützt Administration & Fehlersuche  
