# Care Vita – Projekt-Konzept

## Projekt-Überblick

**Care Vita** ist eine Dokumentations-App für ambulante Pflegedienste.

**Zweck:** Pflegekräfte dokumentieren Patientenbesuche digital vor Ort. Das Büro plant Touren und verwaltet Stammdaten.

**Hauptnutzer:**
- **Pfleger** (mobil, vor Ort): Besuche dokumentieren, Patienten-Infos abrufen
- **Büro-Personal** (Desktop): Tourenplanung, Patientenmanagement, Datenkorrektur

**Geschäftsmodell:**
- **Partner:** Medifox (Partnerprogramm)
- **Vertrieb:** App auf Medifox-Website & im Medifox-Ecosystem
- **Zielgruppe:** Ambulante Pflegedienste (bestehende Medifox-Nutzer)
- **Lizensierung:** Einzeln erwerbbar durch Pflegedienste

## MVP-Phase
- Tech-Stack wird gerade mit Claude entwickelt
- **Datenbank:** SQL-basiert (konkrete DB noch offen: PostgreSQL? MySQL?)
- Fokus: Kern-Features erste, Skalierung später
- Iterativer Ansatz mit Claude

## Feature-Prioritäten

1. **Besuch-Dokumentation** (Kern für Pfleger)
2. **Tourenplanung** (Kern für Büro)
3. **Patientenmanagement** (Büro-Funktionen)
4. **Authentifizierung & Rollen** (Pfleger vs. Büro)
5. **Offline-Sync** (Notwendig für mobile Zuverlässigkeit)
6. **Medifox-Integration** (Daten-Austausch, Single Sign-On?)

## Architektur-Richtlinien

- **Mobile-First:** Pfleger nutzen Smartphones/Tablets
- **Desktop-tauglich:** Büro braucht volle Funktionen
- **Datenintegrität:** Kritisch (medizinische Daten)
- **Rolle-basiert:** Unterschiedliche UI/Funktionen je nach User-Typ
- **Einfachheit:** Intuitive UX für schnelle Dokumentation vor Ort
- **Offline-First:** App funktioniert auch ohne Internet (Cache/Local Storage)

## Use Cases

| Nutzer | Aktion | Grund |
|--------|--------|-------|
| Pfleger | Visit dokumentieren | Nachweis der Leistung |
| Pfleger | Patient-Info abrufen | Kontext vor Besuch |
| Büro | Tour planen | Ressourcen-Optimierung |
| Büro | Patient editieren | Stammdaten aktualisieren |
| Büro | Reports ansehen | Controlling & Abrechnung |

## Medifox-Integration (WICHTIG)

**Zu klären mit Medifox:**
- Welche Daten sollen zwischen Care Vita & Medifox fließen?
- **Single Sign-On (SSO)?** (Medifox-Login für Care Vita?)
- **API-Zugang?** (Care Vita ? Medifox Daten abrufen?)
- **Embedding:** iframe? Separate App? Deep-Links?
- **Daten-Ownership:** Wem gehören die Care Vita Daten?

**Bis geklärt:** Modular bauen, damit Integration später leicht ist.
