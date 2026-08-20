<!-- markdownlint-disable MD041 -->
<!-- Quelle: MIIIGModulStudie @1394b43 (kerndatensatzmodul-studie v2026.0.1) -->
### Kontext im Gesamtprojekt / Bezüge zu anderen Modulen

**Relation zum Modul PERSON.** Eine minimale Version des Probanden war zuvor im
Modul PERSON der MII abgebildet und wurde mit diesem Release in das Modul
Medizinisches Forschungsvorhaben verschoben.

**Relation zum Modul CONSENT.** Das Modul CONSENT beschreibt
Einwilligungserklärungen von aufgeklärten Patienten/Probanden sowie Policies
zur Durchsetzung abgestufter Nutzungsvarianten. Dabei wird dort auf
Forschungsvorhaben Bezug genommen, für welche ein solcher Consent gelten soll.

**Relation zum Modul STRUKTURDATEN.** Das in Erarbeitung befindliche Modul
STRUKTURDATEN beschreibt Organisationsstrukturen, Standorte und einzelne
Leistungsdaten von Organisationseinheiten in den Krankenhäusern der MII. Das
Modul selbst hat keinen direkten Bezug zu Forschungsvorhaben, wird jedoch von
diesem benutzt. Es sind aktuell keine modellierungstechnischen Konflikte
absehbar.

**Relation zu anderen Modulen.** In der Modulbeschreibung zur Charakterisierung
des Moduls Medizinisches Forschungsvorhaben (siehe Beschluss der AG
Interoperabilität vom 17.03.2021) werden Abhängigkeiten von/zu weiteren Modulen
erwähnt. Diese beziehen sich auf mögliche Abhängigkeiten in zukünftigen,
inhaltlich erweiterten Versionen dieses Moduls und werden gegenwärtig nicht
adressiert:

1. Das hier vorliegende Informationsmodell beschäftigt sich aktuell nicht mit
   der Abbildung einzelner klinischer Parameter, wie sie bspw. in CRF-Bögen
   erhoben werden.
2. Das hier vorliegende Informationsmodell benutzt aktuell keine erweiterten
   Metadaten zu Provenance oder Qualität.

Weitere Abhängigkeiten zu anderen Modulen sind dem Team nicht bekannt.

### Organisation (wiederverwendetes Profil)

Durch den Kerndatensatz der Medizininformatik-Initiative wird das Konzept der
„Organisation" bereits im Modul STRUKTURDATEN definiert; diese Spezifikation
wird im Rahmen dieses Moduls wiederverwendet, ist aber **noch nicht final
ballotiert**. Siehe Profil
["Profile - MI-I - Organisation - Organization"](https://simplifier.net/guide/modulstruktur-leitfaden-version1.0?version=current)
(Entwurfsstand), Canonical
`https://www.medizininformatik-initiative.de/fhir/core/modul-strukturdaten/StructureDefinition/Organization`.
Die Abbildung der Kontakt- und Standort-Elemente des Logischen Datensatzes auf
Organization ist im Abschnitt [Profile](profiles.html) beschrieben.

### Referenzen

Die vorliegende Version wurde zusammen mit Vertretern des
[Deutschen Forschungsdatenportals Gesundheit](https://forschen-fuer-gesundheit.de/)
(FDPG) diskutiert. Der vorliegende Entwurf wurde zusammen mit Vertretern der
[Nationalen Forschungsdateninfrastruktur für personenbezogene Gesundheitsdaten](https://www.nfdi4health.de/)
(NFDI4Health) diskutiert und zusammen mit Vertretern aus anderen öffentlich
geförderten Netzwerken und Industriepartnern erstellt. Es wurde auf die sich
daraus möglicherweise ergebenden Interessenkonflikte geachtet.
