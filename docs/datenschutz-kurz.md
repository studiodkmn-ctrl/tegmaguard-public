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

## Nicht nur Schutz — auch der Nachweis dafür

Für eine Kanzlei, Praxis oder Bank reicht die bloße Zusage "wir schützen Ihre
Daten" gegenüber einer Aufsichtsbehörde oder dem eigenen Datenschutzbeauftragten
oft nicht aus — verlangt wird ein vorzeigbares Dokument. Tegmaguard stellt dafür
zu jedem einzelnen Fall zwei Dokumente aus, jederzeit neu abrufbar, nicht nur
einmalig beim Kauf:

- **Ein DSGVO-Bericht pro Fall** (als PDF oder Word), der festhält, welche
  Datenkategorien erkannt und ersetzt wurden und welcher KI-Anbieter beteiligt
  war — mit oder ohne Klartext-Zuordnung.
- **Ein Löschzertifikat nach Art. 17 DSGVO**, ausgestellt bei jeder
  Fall-Löschung, mit einem Verifikationsscan, der die tatsächliche Löschung
  bestätigt statt sie nur zu behaupten.

Beide Dokumente lassen sich für jeden Fall erneut erzeugen, solange der Fall
existiert — nicht nur zum Zeitpunkt der Bearbeitung.

## Grenze der Erkennung, ehrlich benannt

Die Erkennung sensibler Angaben ist bestmöglich, aber nicht garantiert: ein
Wert, der weder erkannt noch bereits bekannt noch von der nutzenden Person
selbst markiert wurde, kann nicht geschützt werden. Deshalb zeigt Tegmaguard
vor jedem Versand eine Vorschau des tatsächlich zu sendenden Textes, die
aktiv bestätigt werden muss — die automatische Erkennung ist die erste,
nicht die einzige Schutzschicht.

## Was dieses Dokument nicht ist

Dies ist eine kurze, allgemeinverständliche Einordnung, kein
Datenschutz-Gutachten und keine vollständige DSGVO-Dokumentation. Eine
ausführlichere interne Dokumentation existiert und ist auf Anfrage für Kunden
und Auditoren einsehbar.

Rechtliche Angaben zum Anbieter: siehe [Impressum](https://tegmaguard.com/impressum.html).
