# ??? Care Vita – Architektur & Tech-Stack

## Tech-Stack (geplant)

| Layer | Technologie | Status |
|-------|-------------|--------|
| **Frontend** | HTML5 / CSS3 / JavaScript | MVP |
| **Backend** | Node.js + Express.js | Planning |
| **Datenbank** | PostgreSQL oder MySQL | Planning |
| **Authentication** | JWT Token | Planning |
| **Offline** | LocalStorage / IndexedDB | Planning |
| **API** | REST | Planning |

## Frontend-Architektur

### Struktur


### Features (MVP)
- **Responsive Design:** Mobile-First, Desktop-tauglich
- **Offline-Mode:** LocalStorage für Patienten-Daten & Besuche
- **Light/Dark Mode:** Settings
- **Real-time Sync:** Wenn Internet zurückkommt

## Backend-Architektur (später)

### Geplante Struktur


## Datenbank-Schema (Überblick)

### Haupttabellen
- **users** (id, name, email, password_hash, role, created_at)
- **patients** (id, name, pid, address, phone, tags, created_at)
- **tours** (id, user_id, date, patients, status, created_at)
- **visits** (id, patient_id, tour_id, services, notes, vorfaelle, started_at, ended_at)
- **incidents** (id, visit_id, category, description, created_at)

## Security & Offline

### Authentication
- **JWT Tokens** für Session-Management
- **Password Hashing** (bcrypt)
- **Role-Based Access** (Pfleger vs. Büro)

### Offline-Handling
- **LocalStorage:** Patient-Cache, Tour-Daten
- **IndexedDB:** Größere Datasets (später)
- **Auto-Sync:** Bei Reconnect Daten zu Backend senden
- **Conflict Resolution:** Last-Write-Wins oder Merge

### Datenschutz
- **HTTPS only** (Verschlüsslung in Transit)
- **Login erforderlich** (kein Anonymous Access)
- **Audit-Logs** (Wer ändert was?)
- **Remote Wipe** (Daten von verlorenen Geräten löschen)

## Entwicklungs-Roadmap

### Phase 1 (MVP)
- [ ] Frontend-Grundgerüst (HTML/CSS)
- [ ] Login-Screen
- [ ] Besuch-Doku UI
- [ ] Offline-Caching (LocalStorage)

### Phase 2
- [ ] Backend (Node.js + Express)
- [ ] Datenbank (PostgreSQL)
- [ ] Authentication (JWT)
- [ ] API-Endpoints

### Phase 3
- [ ] Medifox-Integration
- [ ] Advanced Features (Reports, Analytics)
- [ ] Mobile App (React Native oder PWA)

**Status:** Dieses Dokument wird laufend aktualisiert.
