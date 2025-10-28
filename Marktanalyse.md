# MARKTANALYSE_Plattformen

## Ziel
Ziel der Analyse ist es, die beiden Zielplattformen **Particify** und **arsnova.click** im Hinblick auf den Import von Fragensets zu vergleichen und ihre Anforderungen, Möglichkeiten und Grenzen zu verstehen.

---

## 1. Particify
### Beschreibung
Particify (ars.particify.de) ist eine interaktive Lernplattform, die Umfragen, Quizzes und Q&A-Sessions ermöglicht. Sie ist datenschutzfreundlich und Open-Source.

### Stärken
- Moderne Benutzeroberfläche
- Flexible Fragetypen (Multiple Choice, Freitext, Skala, etc.)
- Echtzeit-Feedback und anonyme Teilnahme
- REST-API für automatisierten Import möglich (JSON-Struktur)

### Schwächen
- Kein direkter Bulk-Import über UI
- Formatierung erfordert JSON oder CSV über API oder manuelles Eingeben

### Importanforderungen
- Format: JSON (strukturierte Fragen, Antworten, korrekte Lösung)
- Pflichtfelder: `question`, `options`, `correctAnswers`, `type`
- Keine eingebetteten Medien per Standard-Import

---

## 2. arsnova.click
### Beschreibung
arsnova.click ist eine Quizplattform für Unterricht und Schulungen, ähnlich wie Kahoot, aber Open-Source und datenschutzkonform.

### Stärken
- Einfaches Erstellen und Teilen von Quizzen
- CSV- oder JSON-Import über „Quiz-Import“
- Unterstützt verschiedene Fragetypen
- Keine Anmeldung für Teilnehmende erforderlich

### Schwächen
- Weniger visuelle Gestaltungsmöglichkeiten
- Begrenzte API-Dokumentation

### Importanforderungen
- Format: JSON oder CSV
- Pflichtfelder: `questionText`, `answers[]`, `correctAnswer`, `timeLimit`
- UTF-8-Kodierung notwendig

---

## 3. Vergleich
| Kriterium               | Particify             | arsnova.click         |
|--------------------------|-----------------------|-----------------------|
| Open Source              | ✅                   | ✅                   |
| JSON-Import möglich      | ✅ (API-basiert)      | ✅ (Datei-basiert)    |
| CSV-Import               | ❌                   | ✅                   |
| Fragetypen-Vielfalt      | Hoch                 | Mittel                |
| API verfügbar            | ✅                   | Teilweise             |
| Geeignet für Schulen     | ✅                   | ✅                   |

---

## 4. Fazit
Beide Plattformen eignen sich für den Import von MC-Test-Fragensets.  
**arsnova.click** ist einfacher für manuelle CSV-Imports.  
**Particify** ist technisch moderner und besser für automatisierte JSON-Exporte geeignet.
