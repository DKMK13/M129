# Routing

**Link**
https://www.itslot.de/2019/02/ipv4-subnetting-berechnen-schritt-fur.html

# Routing

**Link**
https://www.itslot.de/2019/02/ipv4-subnetting-berechnen-schritt-fur.html

**Übungen in Teams**
- M129 - Repetition Routing 1
- M129 - Repetition Routing 2

## Einführung
Routing bedeutet das **Weiterleiten von Datenpaketen** zwischen verschiedenen Netzwerken.  
Router entscheiden anhand ihrer Routing-Tabelle, wohin ein Paket gesendet wird.

Routing arbeitet auf **OSI-Schicht 3**.

---

## Routing-Tabelle
Eine Routing-Tabelle enthält:
- Zielnetz (z. B. 192.168.1.0/24)
- Nächster Hop (Gateway)
- Interface
- Metrik (Kosten)

Beispiel:
| Ziel | Gateway | Interface |
|------|----------|-----------|
| 192.168.2.0/24 | 192.168.1.1 | eth0 |
| 0.0.0.0/0 | 192.168.1.1 | eth0 |

Die letzte Zeile ist die **Default Route**.

---

## Routing-Arten

### **Statisches Routing**
- Manuell konfiguriert  
- Sehr zuverlässig  
- Ideal für kleine Netze

### **Dynamisches Routing**
Router tauschen Routen automatisch aus. Protokolle:
- **RIP** (einfach)
- **OSPF** (schnell, modern)
- **BGP** (Internet-Routing)

---

## Routing-Beispielablauf
1. PC sendet Paket an anderes Netz  
2. Gateway empfängt Paket  
3. Router prüft Routing-Tabelle  
4. Router wählt beste Route  
5. Paket wird weitergeleitet

---

## Merksatz
**Router verbinden Netzwerke → Switches verbinden Geräte.**

---

## Zusammenfassung (Spickzettel)
- Routing verbindet Netzwerke  
- Nutzt eine Routing-Tabelle  
- Statisch oder dynamisch  
- Default Route für „alles andere“  
