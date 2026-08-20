# Startseite - MII Implementation Guide Medizinisches Forschungsvorhaben v2026.0.1

* [**Inhaltsverzeichnis**](toc.md)
* **Startseite**

## Startseite

| | |
| :--- | :--- |
| *Offizielle URL*:https://www.medizininformatik-initiative.de/fhir/modul-studie/ImplementationGuide/mii-ig-studie | *Version*:2026.0.1 |
| Active Stand: 2026-01-09 | *Maschinenlesbarer Name*:MII_IG_Medizinisches_Forschungsvorhaben |

### Einleitung

Die vorliegende Spezifikation beschreibt die FHIR-Repräsentation des Kerndatensatz-Erweiterungsmoduls **Medizinisches Forschungsvorhaben** („Studie") der Medizininformatik-Initiative (MII). Im Folgenden werden die Use-Cases des Moduls sowie die dazugehörigen FHIR-Profile und Terminologie-Ressourcen in ihrer verbindlichen Form beschrieben.

| | |
| :--- | :--- |
| Datum | 09.01.2026 |
| Version | 2026.0.1 (CalVer`JJJJ.n.n`) |
| Status | active |
| Realm | DE |

Den ersten Release finden Sie unter [2025.0.0](https://www.medizininformatik-initiative.de/Kerndatensatz/KDS_Medizinische_Forschungsvorhaben_V2025/ImplementationGuide-1.x-TechnischeImplementierung-Organization.html).

### Zielgruppe

##### Implementierende

Datenintegrationszentren (DIZ), Softwareentwickler:innen und Systemarchitekt:innen, die FHIR-basierte Lösungen umsetzen.
 → siehe [Profile](profiles.md) und [Logische Modelle](logical-models.md).

### Inhalt dieses Leitfadens

* **[Anleitung](guidance.md)** — Modulbeschreibung und Anwendungsszenarien.
* **Konformität** — die KDS-weiten Konformitätsregeln (Anforderungssprache, Must-Support, Umgang mit fehlenden Daten) pflegt zentral das [Meta-Modul](https://github.com/medizininformatik-initiative/kerndatensatz-meta/wiki/Conformance); die modul-spezifischen Aspekte zu [Sicherheit und Datenschutz](security-and-privacy.md) sind Teil dieses Leitfadens.
* **[Profile](profiles.md)** und die weiteren **[Artefakt-Seiten](artifacts.md)** — die technischen Artefakte.
* **[Beispiele](examples.md)** — Beispielinstanzen.
* **[Abhängigkeiten](ImplementationGuide-mii-ig-studie.md)** — die ImplementationGuide-Ressource mit Abhängigkeitstabelle, versionsübergreifender Analyse und Urheberrechtshinweisen.

### Verwandte Leitfäden

Dieses Modul ist Teil des MII-Kerndatensatzes; die weiteren KDS-Module und ihre Abhängigkeiten sind unter [medizininformatik-initiative.de](https://www.medizininformatik-initiative.de/de/der-kerndatensatz-der-medizininformatik-initiative) beschrieben.

### Impressum

Dieser Leitfaden ist im Rahmen der Medizininformatik-Initiative erstellt worden und unterliegt per Governance-Prozess dem Abstimmungsverfahren des Technischen Komitees von HL7 Deutschland e. V.

### Ansprechpartner

* Matthias Löbe, Inst. for Medical Informatics (IMISE), University of Leipzig
* Karoline Buckow, TMF – Technologie- und Methodenplattform für die vernetzte medizinische Forschung e. V.

Fragen zu der vorliegenden Publikation können jederzeit unter [chat.fhir.org](https://chat.fhir.org/#narrow/stream/179307-german.2Fmi-initiative) im Stream 'german/mi-initiative' gestellt werden. Anmerkungen und Kritik wird in Form von 'Issues' im [GitHub-Repository](https://github.com/medizininformatik-initiative/kerndatensatzmodul-studie/issues) gern entgegengenommen.

### Autor:innen (in alphabetischer Reihenfolge)

* Bartow, Martin
* Brix, Tobias
* Gatrio, Margaux
* Gulden, Christian
* Löbe, Matthias
* Macho, Philipp Marten
* Rinaldi, Eugenia
* Scherer, Clemens
* Strauch, Natalia
* Ulbrich, Florian
* Vella, Gustav
* Zautke, Alexander

### Urheberrecht und Lizenz

© 2019+ TMF e. V., Charlottenstraße 42, 10117 Berlin. Dieses Werk ist lizenziert unter der [Creative Commons Namensnennung 4.0 International Lizenz](https://creativecommons.org/licenses/by/4.0/).

Zu den Nutzungsrechten der zugrunde liegenden FHIR-Technologie siehe die FHIR-Basis-Spezifikation. Einige verwendete Codesysteme werden von anderen Organisationen herausgegeben und gepflegt; es gilt das Copyright der dort jeweils aufgeführten Herausgeber (Publisher).

### Haftungsausschluss

Der Inhalt dieses Dokuments ist öffentlich. Zu beachten ist, dass Teile dieses Dokuments auf FHIR Version R4 beruhen, für die das Copyright von HL7 International gilt.

Obwohl diese Publikation mit größter Sorgfalt erstellt wurde, können die Autoren keinerlei Haftung für direkten oder indirekten Schaden übernehmen, der durch den Inhalt dieser Spezifikation entstehen könnte.

