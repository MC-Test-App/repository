---

## 📄 3. FEATURE_SPEC_EXPORT.md

```markdown
# FEATURE_SPEC_EXPORT

## Ziel
Definition der Funktionen, die der Export aus der MC-Test-App unterstützen muss, um kompatible Datenformate zu erzeugen.

---

## 1. Basisfunktionen
- Auswahl der Zielplattform (Particify / arsnova.click)
- Exportformat automatisch anpassen
- Vorschau der Datenstruktur
- Validierung auf leere Felder, doppelte Antworten

---

## 2. Erweiterte Funktionen
- Automatische Konvertierung von MC-Test-Fragen in Plattformsyntax
- Optionaler Export von Metadaten (Kategorie, Zeitlimit)
- Lokaler Download (JSON oder CSV)
- API-Upload für Particify (optional)
- Logging von Exportfehlern

---

## 3. Beispielablauf
1. Nutzer wählt Fragenset in der App.
2. Klick auf „Exportieren“.
3. Zielplattform auswählen → Formatvorschau erscheint.
4. Klick auf „Datei speichern“ → Export erfolgreich.
