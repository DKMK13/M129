# Subnetting

**Link**
https://www.itslot.de/2019/02/ipv4-subnetting-berechnen-schritt-fur.html

**Aufgaben in Teams**
- M129 - Repetition Subnetting 1
- M129 - Subnetting Übungen


## Einführung
Subnetting teilt ein großes Netzwerk in kleinere Teilnetze (Subnetze) auf.  
Dies verbessert Struktur, Sicherheit und IP-Effizienz.

Beispiel:  
`192.168.0.0/24` → vier Subnetze /26

---

## Gründe für Subnetting
- Weniger Broadcasts  
- Bessere Netzwerksicherheit  
- Präzisere IP-Verwaltung  
- Klare Strukturierung

---

## Subnetzmaske & CIDR
| CIDR | Maske | Hosts |
|------|--------|--------|
| /24 | 255.255.255.0 | 254 |
| /25 | 255.255.255.128 | 126 |
| /26 | 255.255.255.192 | 62 |
| /30 | 255.255.255.252 | 2 (für Routerlinks) |

---

## Aufbau eines Subnetzes
Jedes Subnetz besitzt:
- Netzwerkadresse  
- Hostbereich  
- Broadcastadresse  

Beispiel: `/26`
| Subnetz | Adresse | Hostbereich | Broadcast |
|---------|----------|--------------|------------|
| 1 | 192.168.0.0 | .1–.62 | .63 |
| 2 | 192.168.0.64 | .65–.126 | .127 |
| 3 | 192.168.0.128 | .129–.190 | .191 |
| 4 | 192.168.0.192 | .193–.254 | .255 |

---

## Subnetting-Ablauf (Schritt für Schritt)
1. Wie viele Hosts benötige ich?  
2. Passende Maske wählen (z. B. /26 für 62 Hosts)  
3. Netzwerke in Schritte der Blockgröße berechnen  
4. Hostbereiche bestimmen  
5. Broadcastadresse bestimmen

---

## Merksatz
**Große Netze → kleine Netze schneiden.**

---

## Zusammenfassung (Spickzettel)
- Teilt ein Netz in kleinere Teile  
- Bietet Struktur & Sicherheit  
- Wichtigste Größe: Subnetzmaske  
- Kennt Netzwerk, Hostbereich & Broadcast  
