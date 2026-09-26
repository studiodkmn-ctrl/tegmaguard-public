# Datenschutz kurz erklärt

Tegmaguard ist dafür gebaut, dass echte personenbezogene und geschäftskritische
Daten ein KI-Modell erst gar nicht erreichen.

## Das Grundprinzip

Bevor ein Text an ein KI-Modell geschickt wird, erkennt Tegmaguard sensible
Angaben — Namen, Adressen, IBANs, Aktenzeichen und viele weitere Kategorien —
und ersetzt sie durch stimmige, aber frei erfundene Platzhalterdaten
(„Spiegeldaten"). Erst dieser bereinigte Text verlässt das Gerät. Kommt die
Antwort zurück, werden die Platzhalter lokal wieder durch die echten Werte
ersetzt — sichtbar nur auf dem eigenen Gerät.

## Was das bedeutet

- **Kein Server von Tegmaguard.** Die Anonymisierung läuft vollständig lokal
  auf dem Gerät der nutzenden Person.
- **Keine Telemetrie.** Es werden keine Nutzungsdaten an Tegmaguard übermittelt.
- **Mit Ollama bleibt alles lokal.** Wer ein lokales Sprachmodell über Ollama
  nutzt, dessen Anfragen verlassen das Gerät gar nicht erst — der
  Ollama-Zugriff ist hart auf localhost beschränkt.
- **Cloud-Anbieter sehen nur Platzhalterdaten.** Bei Nutzung von Claude,
  ChatGPT oder Gemini erhält der jeweilige Anbieter ausschließlich den Text
  mit den erfundenen Ersatzangaben, nie die echten Werte.

## Für wen das besonders relevant ist

Berufsgruppen mit gesetzlicher Schweigepflicht — etwa Rechtsanwältinnen und
Rechtsanwälte, Steuerberatende sowie Angehörige von Gesundheitsberufen im
Sinne des § 203 StGB — dürfen echte Mandanten- oder Patientendaten nicht
ungeschützt an externe Dienste weitergeben. Tegmaguard verhindert genau diesen
Schritt, indem der echte Wert das Gerät nicht verlässt. Für andere Branchen,
etwa Banking, gelten andere rechtliche Rahmenbedingungen (z. B.
Bankgeheimnis) — auch dort bleibt das Grundprinzip (Spiegeldaten statt
Klartext) dasselbe.

## Was dieses Dokument nicht ist

Dies ist eine kurze, allgemeinverständliche Einordnung, kein
Datenschutz-Gutachten und keine vollständige DSGVO-Dokumentation. Eine
ausführlichere interne Dokumentation existiert und ist auf Anfrage für Kunden
und Auditoren einsehbar.

Rechtliche Angaben zum Anbieter: siehe [Impressum](https://tegmaguard.com/impressum.html).
