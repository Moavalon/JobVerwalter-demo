# JobVerwalter Demo

**Deine Bewerbungen. Dein Überblick.**

JobVerwalter hilft dir, Bewerbungen, Kontakte, Unterlagen und den Verlauf deiner
Bewerbungen lokal zu verwalten. Diese frühe Windows-Demo erlaubt insgesamt zehn
eigene Bewerbungen ohne Zeitlimit. Archivierte und gelöschte Bewerbungen zählen mit.

**[Windows-Demo herunterladen – 0.5.0-preview.3, ca. 325 MB](https://github.com/Moavalon/JobVerwalter-demo/releases/download/v0.5.0-preview.3/JobVerwalter-Demo-0.5.0-preview.3-Setup.exe)**

[Installations- und Betriebsanleitung](ANLEITUNG.md) ·
[Release und SHA-256-Prüfsumme](https://github.com/Moavalon/JobVerwalter-demo/releases/tag/v0.5.0-preview.3)

## Installation

Setup.exe herunterladen und doppelklicken. Installation und Betrieb sind für
den aktuellen Windows-Benutzer ohne angeforderte Administratorrechte vorgesehen.
Nach dem Start öffnet sich die lokale Oberfläche im Browser. Lies die
Demo-Hinweise und lege dein eigenes lokales Konto an; ein manuelles
Bootstrap-Token ist nicht erforderlich.

Die benötigten Laufzeitkomponenten werden mitgeliefert. Eine gesonderte
Installation von .NET, Node.js, PostgreSQL, Docker oder Tailscale ist nicht nötig.
Du startest mit einem leeren eigenen Bestand und richtest die Anwendung selbst ein.
Der separate Übungsbestand enthält ausschließlich fiktive Daten zum Ansehen.

## Voraussetzungen und Prüfstand

Zielsysteme sind Windows 10 22H2 oder Windows 11, jeweils x64. Installation,
Erststart, Konto, Kontingent, PDF/CSV und Deinstallation/Neuinstallation wurden
auf einer Windows-10-Pro-22H2-VM mit eingeschränktem Benutzertoken geprüft und
durch einen manuellen Installationstest ergänzt. Diese VM enthält Entwicklerwerkzeuge.
Eine vollständige Abnahme auf frischen Windows-10-/Windows-11-Systemen sowie
auf verwalteten Firmenrechnern steht noch aus. Firmenrichtlinien können Download
oder Ausführung unterbinden; die Demo umgeht diese Richtlinien nicht.

Dies ist eine frühe Demo. Noch nicht vollständig abgenommen sind insbesondere
native Backup/Restore- und Versionsupdate-Abläufe, echter SMTP-Versand mit
separaten Testzugängen sowie sämtliche Ansichts-/Tastatur-/Kernabläufe.
Bewahre bei eigenen Tests wichtige Unterlagen zusätzlich außerhalb der Demo auf.

## E-Mail und lokale Daten

Die Demo enthält keine vorgegebenen Konten, Bewerbungsdaten oder Providerzugänge.
SMTP/IMAP sind zunächst unkonfiguriert und deaktiviert. Nach bewusster Einrichtung
und Aktivierung eigener SMTP-Zugangsdaten werden **echte E-Mails** versendet.
Für Versandtests ausschließlich einen selbst kontrollierten Empfänger verwenden.
Es gibt keinen Simulationsversand im eigenen Bestand.

Die Anwendung ist über eine lokale Loopback-Adresse im Browser erreichbar.
Es gibt keinen automatischen Upload von Bewerbungsinhalten oder Fehlerberichten
an den Entwickler. Bewusst eingerichtete Providerverbindungen und geöffnete
externe Links bleiben davon unberührt.

Programmdateien: `%LOCALAPPDATA%\Programs\JobVerwalter`.
Daten, Schlüssel und Sicherungen: `%LOCALAPPDATA%\JobVerwalter`.
Normale Deinstallation erhält diese Daten und das verbrauchte Kontingent.
Updates werden später über einen neuen Setup-Installer installiert.
Zum vollständigen Beenden den Startmenü-Eintrag **JobVerwalter beenden** verwenden.

## Downloads und Rückmeldungen

Dieses unabhängige Repository enthält öffentliche Beschreibung, Anleitung und
fertige Downloads. Der Anwendungsquellcode ist hier nicht enthalten.
Der Downloadlink benötigt weder GitHub-Anmeldung noch Zugriffsschlüssel.
Die EXE ist nicht mit einem Herausgeberzertifikat signiert; Windows oder der
Browser können eine Warnung anzeigen. Die SHA-256-Prüfsumme prüft die
Dateiübereinstimmung und ersetzt keine Herausgebersignatur.

[Fehler oder Rückmeldung melden](https://github.com/Moavalon/JobVerwalter-demo/issues).
Bitte keine privaten Bewerbungsunterlagen, Zugangsdaten, Original-E-Mails oder
ungeschwärzte Screenshots veröffentlichen. GitHub-Issues sind öffentlich.

Die Lizenztexte der Anwendung und mitgelieferter Fremdkomponenten liegen im
Installationsordner unter `runtime/LICENSE.txt`
bzw. `runtime/ThirdPartyNotices`. Maßgeblich sind die jeweils mitgelieferten Texte.
