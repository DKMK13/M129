# MAC-Adresse

## Einführung
Die **MAC-Adresse** ist die physische Hardware-Adresse eines Netzwerkadapters.  
Sie ist **weltweit eindeutig** und wird vom Hersteller vergeben.

Format:  
`AA:BB:CC:DD:EE:FF`

---

## Aufbau der MAC-Adresse
| Teil | Bedeutung |
|------|-----------|
| **OUI (Organizationally Unique Identifier)** | Herstellerkennung, z. B. Intel, Cisco |
| **Geräte-ID** | Individuelle Seriennummer der Karte |

---

## Eigenschaften
- 48 Bit  
- Hexadezimal  
- Wird NICHT verändert (außer Spoofing)  
- Wird lokal im Netzwerk verwendet (Layer 2)

---

## MAC-Adresse im Netzwerk
- Switches lernen MAC-Adressen anhand eingehender Frames  
- ARP fragt IP → MAC  
- Ohne MAC keine Kommunikation im LAN

---

## Beispielablauf (ARP)
1. PC kennt IP des Ziels  
2. ARP-Broadcast: "Wer hat IP 192.168.0.10?"  
3. Ziel sendet MAC-Adresse zurück  
4. Kommunikation beginnt

---

## Merksatz
**MAC = Physische Identität. IP = Logische Identität.**

---

## Zusammenfassung (Spickzettel)
- 48-bit Hardwareadresse  
- Lokal eindeutig  
- Wird für die Kommunikation im LAN benötigt  
- Router arbeiten NICHT mit MAC-Adressen  
