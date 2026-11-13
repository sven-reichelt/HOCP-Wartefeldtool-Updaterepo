# HOCP-Wartefeldtool — Programmdateien

Hier liegen ausschließlich die fertigen Programmdateien des
**HOCP-Wartefeldtools**, einer Windows-Anwendung für Kunden von
ho.Cloud Phone. Quellcode gibt es hier nicht.

Dieses Repository ist öffentlich, damit sich die installierten Anwendungen
selbst aktualisieren können, ohne ein Zugriffstoken mitzubringen.

## Für Anwender

Sie müssen hier nichts herunterladen. Die Anwendung holt sich neue Fassungen
von selbst und prüft sie dabei.

Bekommen Sie das Wartefeldtool neu, wenden Sie sich an ho.Systeme — Sie
brauchen dafür ohnehin einen Aktivierungscode.

## Was zu einer Veröffentlichung gehört

| Datei | Zweck |
|---|---|
| `HOCP-Wartefeldtool.exe` | die Anwendung |
| `HOCP-Wartefeldtool.exe.sha256` | Prüfsumme der Datei |
| `manifest.json` | Version und Prüfsummen aller Dateien |
| `manifest.json.sig` | Signatur über das Manifest |

Die Anwendung prüft beides: die Signatur des Manifests gegen einen
öffentlichen Schlüssel, den sie eingebaut mitbringt, und erst danach die
Prüfsumme der Datei gegen das Manifest. Trägt die Signatur nicht, wird nichts
installiert.

Der zugehörige private Schlüssel liegt nicht in diesem Repository und auch
nicht im Zugriff des Tokens, mit dem hier veröffentlicht wird.

---

© ho.Systeme
