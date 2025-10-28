# TECH_SPEC_Plattformen

## Ziel
Technische Dokumentation der Schnittstellenformate für den Import von MC-Test-Daten in Particify und arsnova.click.

---

## 1. Particify – Importformat (JSON über API)
Beispielstruktur:

```json
{
  "questions": [
    {
      "type": "multiple-choice",
      "question": "Wie viele Planeten hat unser Sonnensystem?",
      "options": ["7", "8", "9", "10"],
      "correctAnswers": ["8"]
    }
  ]
}
