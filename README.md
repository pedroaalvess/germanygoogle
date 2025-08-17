# Google Careers Deutschland - Vollständiges Projekt

## 🇩🇪 Über das Projekt

Dies ist die vollständige deutsche Version der Google Careers Website, übersetzt und angepasst für den deutschen Markt. Das Projekt umfasst:

- **Frontend**: Vollständig übersetztes React-Interface in deutscher Sprache
- **Backend**: Flask-API mit deutschen Stellenangeboten und Dokumentenverarbeitung
- **Formulare**: Angepasst für deutsche Dokumente (Personalausweis und Lebenslauf)
- **Datenbank**: Vorgefüllt mit deutschen Stellenangeboten

## 📋 Funktionen

### ✅ Frontend-Funktionen
- Vollständig responsive deutsche Benutzeroberfläche
- Interaktives Stellenkarussell mit deutschen Positionen
- Bewerbungsformular für deutsche Dokumente:
  - Personalausweis (Vorder- und Rückseite)
  - Lebenslauf
  - Steuerliche Identifikationsnummer
- Geolokalisierung für deutsche Städte
- Moderne UI mit Tailwind CSS

### ✅ Backend-Funktionen
- Flask-API mit CORS-Unterstützung
- SQLite-Datenbank mit deutschen Stellenangeboten
- Dokumenten-Upload-System
- Admin-Panel für Bewerbungsverwaltung
- Sichere Dateiverarbeitung

### ✅ Deutsche Stellenangebote
1. **Software Engineer** - München (€3.500-4.500)
2. **Product Manager** - Berlin (€4.000-5.500)
3. **UX Designer** - Hamburg (€3.200-4.200)
4. **Data Scientist** - Frankfurt (€3.800-5.000)
5. **Marketing Manager** - Köln (€3.000-4.000)
6. **Cloud Solutions Architect** - Stuttgart (€4.200-5.800)

## 🚀 Installation und Setup

### Voraussetzungen
- Python 3.8+
- Node.js 16+
- SQLite3

### Backend-Setup
```bash
cd backend
pip install -r requirements.txt
python populate_db.py  # Datenbank mit deutschen Stellenangeboten füllen
python src/main.py     # Server starten
```

### Frontend-Setup
Das Frontend ist bereits als statische Dateien im `frontend/` Ordner kompiliert.

### Vollständige Bereitstellung
1. Backend auf Port 5000 starten
2. Frontend-Dateien über einen Webserver bereitstellen
3. Sicherstellen, dass CORS korrekt konfiguriert ist

## 📁 Projektstruktur

```
google-careers-germany-complete/
├── frontend/                 # Kompilierte React-App
│   ├── index.html           # Hauptseite
│   ├── assets/              # CSS, JS, Bilder
│   └── favicon.png          # Google-Logo
├── backend/                 # Flask-API
│   ├── src/
│   │   ├── main.py         # Hauptanwendung
│   │   ├── models/         # Datenbankmodelle
│   │   └── routes/         # API-Routen
│   ├── uploads/            # Hochgeladene Dokumente
│   ├── requirements.txt    # Python-Abhängigkeiten
│   └── populate_db.py      # Datenbankinitialisierung
└── README.md               # Diese Datei
```

## 🌐 API-Endpunkte

### Öffentliche Endpunkte
- `GET /api/jobs` - Alle Stellenangebote abrufen
- `POST /api/applications` - Neue Bewerbung einreichen
- `POST /api/applications/{id}/documents` - Dokumente hochladen

### Admin-Endpunkte
- `GET /api/admin/applications` - Alle Bewerbungen anzeigen
- `GET /api/admin/applications/{id}` - Bewerbungsdetails
- `GET /api/admin/documents/{id}/download` - Dokument herunterladen

## 📝 Deutsche Anpassungen

### Formulardokumente
- **Personalausweis**: Deutscher Personalausweis (Vorder- und Rückseite)
- **Lebenslauf**: Deutscher Lebenslauf im PDF-Format
- **Steuer-ID**: Steuerliche Identifikationsnummer (optional)

### Validierungen
- Deutsche Telefonnummern: `+49` oder `0` Format
- Deutsche Postleitzahlen: 5-stellig
- Deutsche E-Mail-Adressen

### Lokalisierung
- Alle Texte in deutscher Sprache
- Deutsche Datumsformate
- Euro-Währung für Gehälter
- Deutsche Städte und Standorte

## 🔧 Konfiguration

### Umgebungsvariablen
```bash
FLASK_ENV=production
DATABASE_URL=sqlite:///google_careers_germany.db
UPLOAD_FOLDER=uploads
MAX_CONTENT_LENGTH=16777216  # 16MB
```

### CORS-Konfiguration
Das Backend ist für Cross-Origin-Requests konfiguriert, um Frontend-Backend-Kommunikation zu ermöglichen.

## 📊 Datenbank

Die SQLite-Datenbank enthält:
- **jobs**: Deutsche Stellenangebote mit Gehaltsspannen
- **applications**: Bewerberdaten mit deutschen Feldern
- **documents**: Hochgeladene Dokumente (Personalausweis, Lebenslauf)

## 🎯 Bereitstellung

### Lokale Entwicklung
1. Backend starten: `python backend/src/main.py`
2. Frontend über HTTP-Server bereitstellen
3. Auf `http://localhost:5000` zugreifen

### Produktionsbereitstellung
1. Backend auf Cloud-Plattform bereitstellen (Railway, Heroku, etc.)
2. Frontend auf CDN oder statischem Hosting bereitstellen
3. Umgebungsvariablen konfigurieren
4. HTTPS aktivieren

## 🛡️ Sicherheit

- Sichere Datei-Uploads mit Typvalidierung
- SQL-Injection-Schutz durch SQLAlchemy
- CORS-Konfiguration für sichere Cross-Origin-Requests
- Dateigröße-Limits für Uploads

## 📞 Support

Bei Fragen oder Problemen:
1. Überprüfen Sie die Logs in `backend/logs/`
2. Stellen Sie sicher, dass alle Abhängigkeiten installiert sind
3. Überprüfen Sie die Datenbankverbindung

## 🎉 Fertig!

Das Projekt ist vollständig übersetzt und bereit für die Bereitstellung im deutschen Markt. Alle Funktionen wurden getestet und funktionieren mit deutschen Dokumenten und Validierungen.

**Viel Erfolg mit Google Careers Deutschland!** 🚀

