# ?? Care Vita MVP – Feature-Liste & Roadmap

## Priorisierung

| # | Feature | Nutzer | Priorität | Status |
|---|---------|--------|-----------|--------|
| 1 | Login / Authentifizierung | Beide | ?? Kritisch | Planning |
| 2 | Besuch-Dokumentation | Pfleger | ?? Kritisch | Planning |
| 3 | Tourenliste anzeigen | Pfleger | ?? Kritisch | Planning |
| 4 | Patienten-Details | Pfleger | ?? Kritisch | Planning |
| 5 | Leistungen dokumentieren | Pfleger | ?? Kritisch | Planning |
| 6 | Vorfälle melden | Pfleger | ?? Hoch | Planning |
| 7 | Offline-Modus | Pfleger | ?? Hoch | Planning |
| 8 | Büro-Dashboard | Büro | ?? Hoch | Planning |
| 9 | Tourenplanung | Büro | ?? Mittel | Planning |
| 10 | Patientenmanagement | Büro | ?? Mittel | Planning |
| 11 | Medifox-Integration | Integration | ?? Mittel | Planning |

## Feature Details

### 1. ?? Login / Authentifizierung
**User Story:** Als Pfleger möchte ich mich mit Benutzername & Passwort anmelden.

**Akzeptanz-Kriterien:**
- [ ] Login-Screen mit E-Mail/Passwort-Input
- [ ] Validierung (Pflichtfelder, E-Mail-Format)
- [ ] Fehlerbehandlung (Ungültige Credentials)
- [ ] Session-Speicherung (Browser-Speicher)
- [ ] Logout-Funktion

### 2. ?? Besuch-Dokumentation
**User Story:** Als Pfleger möchte ich einen Besuch dokumentieren (Zeit, Leistungen, Notizen).

**Akzeptanz-Kriterien:**
- [ ] Start-Zeit automatisch erfasst
- [ ] Leistungen auswählbar (Hygiene, Medikamente, Vitalzeichen)
- [ ] Notiz-Feld für freien Text
- [ ] End-Zeit automatisch erfasst
- [ ] Daten lokal speichern (Offline)
- [ ] Zu Server synchen (wenn Online)

### 3. ?? Tourenliste
**User Story:** Als Pfleger möchte ich meine heutige Tour sehen (Patienten, Zeiten, Adressen).

**Akzeptanz-Kriterien:**
- [ ] Patienten-Liste mit Namen, PID, Uhrzeit, km-Distanz
- [ ] Nächster Besuch hervorgehoben
- [ ] Erledigte Besuche als "? Erledigt" markiert
- [ ] Sortierung nach Uhrzeit
- [ ] Telefon-Nummer zum Anrufen

### 4. ?? Patienten-Details
**User Story:** Als Pfleger möchte ich Infos zum Patienten sehen (Adresse, Allergien, Medikamente, Risiken).

**Akzeptanz-Kriterien:**
- [ ] Name, PID, Adresse anzeigen
- [ ] Allergien & Risiken prominent zeigen (z.B. "STURZGEFAHR")
- [ ] Notizen des Büros anzeigen
- [ ] Link zum Besuch starten

### 5. ?? Leistungen dokumentieren
**User Story:** Als Pfleger möchte ich ankreuzen, welche Leistungen ich erbracht habe.

**Akzeptanz-Kriterien:**
- [ ] Checkboxen für: Hygiene, Medikamente, Vitalzeichen, Beratung
- [ ] Mehrfach-Auswahl möglich
- [ ] Auswahl speichern
- [ ] Im Büro-Report anzeigen

### 6. ?? Vorfälle melden
**User Story:** Als Pfleger möchte ich Probleme/Vorfälle melden.

**Akzeptanz-Kriterien:**
- [ ] Kategorien wählbar: Medizinisch, Organisation, Medikamente
- [ ] Freitextfeld für Beschreibung
- [ ] Spracheingabe (optional, später)
- [ ] Vorfälle im Detail-View anzeigen
- [ ] Büro sieht Vorfälle im Dashboard

### 7. ?? Offline-Modus
**User Story:** Als Pfleger möchte ich auch ohne Internet arbeiten können.

**Akzeptanz-Kriterien:**
- [ ] Patienten-Daten lokal cachern
- [ ] Besuche offline speichern
- [ ] Auto-Sync bei Verbindung
- [ ] Sync-Status anzeigen
- [ ] Konflikte auflösen (Last-Write-Wins)

### 8. ?? Büro-Dashboard
**User Story:** Als Büro-Mitarbeiter möchte ich sehen, wie viele Besuche erledigt sind & ob Vorfälle gemeldet wurden.

**Akzeptanz-Kriterien:**
- [ ] Counter: Erledigt / Offen / Vorfälle
- [ ] Liste abgeschlossener Besuche mit Leistungen
- [ ] Vorfälle prominent anzeigen
- [ ] Echtzeit-Updates (oder manuell refreshen)

## Roadmap Timeline

### Sprint 1 (Woche 1-2)
- [ ] Frontend-Grundgerüst (HTML/CSS)
- [ ] Login-Screen
- [ ] Tour-Liste & Patient-Details (UI nur)

### Sprint 2 (Woche 3-4)
- [ ] Besuch-Dokumentation UI
- [ ] Offline-Caching (LocalStorage)
- [ ] Besuche speichern & anzeigen

### Sprint 3 (Woche 5-6)
- [ ] Backend-Setup (Node.js + Express)
- [ ] Database-Schema
- [ ] API-Endpoints

**Status:** MVP v0.1 – In Planning  
**Zuletzt aktualisiert:** April 2026
