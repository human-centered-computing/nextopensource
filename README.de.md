# NextOpenSource

[English](README.md) · [Türkçe](README.tr.md) · [Deutsch](README.de.md) · [العربية](README.ar.md)

## Was ist NextOpenSource?

Unabhängiger Arbeitsbereich zur Bewertung und Anpassung von Open-Source-Software für NextLife und alle HCC-Projekte. Wiederverwendung, Core-Repositories und Eigenentwicklung vergleichen; Herkunft, Lizenzverträglichkeit, Wartung, Sicherheitsrisiken und Anpassungsgrenzen dokumentieren.

**Status:** Öffentliches Repository mit gemeinsamem Core-Katalog; noch kein laufender Dienst, keine eingesetzten Agenten oder automatische Freigabekontrolle.

## Rolle und Arbeitsstandards

Die Rolle **Open-Source-Spezialist** in [NextDeveloper](https://github.com/human-centered-computing/nextdeveloper) arbeitet hier als autorisierter Mensch, KI oder hybrider Akteur. Menschliche Verantwortung, unabhängige Prüfung und menschliche Genehmigung bleiben erforderlich.

- Upstream-URL, fixierten Commit/Tag, Lizenz und Hinweise, Wartung und Abhängigkeiten dokumentieren.
- Bestehende Core-Komponenten, Alternativen, Erweiterungen/Adapter und Eigenentwicklung vergleichen; Kosten und menschlichen Nutzen bewerten.
- Upstream-Herkunft, Attribution und Lizenzen erhalten; Core-Änderungen von lokalisierten Daten, Präsentation und Produktwert trennen.
- Patches, Aktualisierungsstrategie, Verträge, Lizenz- und Sicherheitsgrenzen erfassen; NextSecurity prüft unabhängig.

NextRoadmap verantwortet die genehmigte Analyse, NextOpenSource die detaillierte Quellbewertung. Die [Core-Bibliothek](Core/README.md) ist der gemeinsame Ort autorisierter Importe mit einem Verzeichnis pro Komponente. Unabhängige Core- und Produkt-Repositories bleiben für ihren angepassten Quellcode verantwortlich. Keine automatische Fork-, Release-, Lizenz- oder Integrationsgenehmigung.

## Projektarbeitsbereiche und Ablauf

- Für jede kanonische Projekt-/Modul-ID gibt es genau ein Verzeichnis auf oberster Ebene. Bei autorisierter Arbeit wird es angelegt und hier registriert; Überarbeitungen erfolgen dort. Keine doppelten oder leeren Projektordner.
- Zuerst die genehmigte Projektanalyse in [NextRoadmap](https://github.com/human-centered-computing/nextroadmap) und die HCC-Richtlinien lesen. Die [Arbeitsvorlage](templates/WORKSPACE.md) verwenden.
- Umfang, Rolle, menschliche Verantwortung, genaue Quellrevision, Nachweise, Entscheidungen, Einschränkungen, messbare Akzeptanz und menschlichen Nutzen, unabhängige Prüfung sowie erforderliche menschliche Genehmigung dokumentieren. Änderungen als überprüfbare Pull Requests einreichen.
- Keine Geheimnisse, personenbezogenen Daten oder vertraulichen Nachweise im normalen Git-Verlauf; bei Genehmigung auf geschützte Nachweise verweisen. Keine Selbstfreigabe, keine stillschweigende Ausweitung des Umfangs und keine unbewiesenen Testergebnisse.

## Core-Bibliothek

[Core](Core/README.md) enthält autorisierte wiederverwendbare Quellen und Herkunftsnachweise. Der erste registrierte Baustein [NextID-Core](Core/NextID-Core/README.md) ist eine exakt fixierte Kopie des ursprünglichen Keycloak-Quellcodes.

## Projekte

Noch keine projektspezifische Arbeit begonnen.

## Gemeinsame Richtlinien

[Engineering-Standards](https://github.com/human-centered-computing/.github/blob/main/ENGINEERING-STANDARDS.md) · [KI-Governance](https://github.com/human-centered-computing/.github/blob/main/AI-GOVERNANCE.md) · [Sicherheit](https://github.com/human-centered-computing/.github/blob/main/SECURITY.md).

Englisch ist maßgeblich. Die README-Dateien folgen dem viersprachigen Standard. Das Repository ist öffentlich; Veröffentlichung und Lizenzierung erfordern eine entsprechende Prüfung. Keine Freigabe oder Lizenzgewährung ist damit verbunden.
