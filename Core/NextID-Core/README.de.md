# NextID-Core

[English](README.md) · [Türkçe](README.tr.md) · [Deutsch](README.de.md) · [العربية](README.ar.md)

[Core-Bibliothek](../README.de.md)

Gemeinsame Open-Source-Identitäts- und Zugriffsgrundlage für NextID. Originalquelle [keycloak/keycloak](https://github.com/keycloak/keycloak), persönlicher Fork nur Strukturreferenz. Keine absichtliche Änderung originaler Dateien.

- Upstream-Release: [26.8.2](https://github.com/keycloak/keycloak/releases/tag/26.8.2) (2026-11-05).
- Fixierter Commit: [`e514445f9dcdabc5bdcf67cab56c1e49655de067`](https://github.com/keycloak/keycloak/commit/e514445f9dcdabc5bdcf67cab56c1e49655de067)
- Quellbaum: `6f439a9bda71c39bf725150cea5d50f149e423f6`
- Lizenz: Apache-2.0; ursprüngliche Lizenz und Namensnennungen/Hinweise in der Quelle.
- Quelle: [source/](source/), vollständiger exakter Upstream-Git-Baum als normale Dateien.

Ein normaler Clone enthält den gesamten Quellbaum ohne Submodule. NextID verwendet die fixierte Quelle zum Build; lokalisierte Daten, Themes, Erweiterungen, Dockerfile und Produktkonfiguration bleiben im eigenen Repository.

Das persönliche NextID nutzt ein Core-Containerimage plus NextLog-Listener. HCC trennt Originalquelle, geprüften Core-Build und angepasstes Produktimage. Registrierung autorisiert keinen Build oder Veröffentlichung. Exakten NextOpenSource-Commit und Imagedigest erfassen; kein schwebendes latest. Das Repository ist öffentlich; keine Zugangsdaten in Dockerfiles.

Upstream nur per geprüftem PR aktualisieren, erwarteten Baum verifizieren, Lizenz/Hinweise bewahren, NextSecurity-Prüfung, Build und Regression vor Produktion. Keine automatische Aktualisierung oder Veröffentlichung durch diese Registrierung.