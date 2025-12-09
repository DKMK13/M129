# DNS-Name

## Einführung
Das Domain Name System (**DNS**) übersetzt menschenlesbare Namen (Domains) in IP-Adressen.  
Beispiel:  
`www.google.com` → `142.250.x.x`

DNS ist das **Telefonbuch des Internets**.

---

## Aufbau eines DNS-Namens
Ein Domainname besteht aus mehreren Teilen:

| Teil | Beispiel | Bedeutung |
|------|----------|-----------|
| **TLD** | `.com`, `.ch`, `.org` | Höchste Ebene |
| **Second Level Domain** | `google`, `example` | Organisations-/Markenname |
| **Subdomain** | `www`, `api`, `mail` | Unterbereich der Domain |

Beispiel-Aufbau:  
`mail.school-example.ch`  
→ Subdomain: **mail**  
→ SLD: **school-example**  
→ TLD: **ch**

---

## Wichtige DNS-Records

| Record | Beschreibung | Beispiel |
|--------|--------------|----------|
| **A** | Domain → IPv4 | google.com → 142.250.x.x |
| **AAAA** | Domain → IPv6 | ipv6.google.com |
| **CNAME** | Alias zu einem DNS-Namen | www → server1 |
| **MX** | Mailserver | gmail-smtp-in.l.google.com |
| **TXT** | Freitext (SPF, DKIM) | SPF: erlaubt Mailserver |

---

## Ablauf einer DNS-Auflösung (vereinfacht)
1. Nutzer gibt Domain ein  
2. Browser fragt lokalen DNS-Resolver  
3. Resolver fragt Root-DNS  
4. Root gibt zuständige TLD-Server zurück  
5. TLD führt zu Authoritative DNS  
6. Der liefert IP-Adresse zurück  

---

## Merksatz
**DNS = Domain → Nummernsystem**

---

## Zusammenfassung (Spickzettel)
- Übersetzt Namen in IPs  
- Arbeitet hierarchisch (Root → TLD → Autoritativ)  
- Nutzt Records wie A, CNAME, MX  
- Ohne DNS gäbe es keine URLs, nur IPs  
