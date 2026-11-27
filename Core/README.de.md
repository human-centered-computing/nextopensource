# Core – gemeinsame Open-Source-Grundlage

[English](README.md) · [Türkçe](README.tr.md) · [Deutsch](README.de.md) · [العربية](README.ar.md)

[NextOpenSource](../README.de.md)

Gemeinsamer Katalog und Quellort wiederverwendbarer Upstream-Komponenten. Jedes autorisierte Element hat einen stabilen Ordner `Core/<ComponentID>/`.

```text
Core/
  README.md
  README.tr.md
  <ComponentID>/                 # one directory per upstream component
    README.md                    # origin, purpose, pinned version, use
    README.tr.md                 # Turkish
    README.de.md                 # German
    README.ar.md                 # Arabic
    UPSTREAM.md                  # provenance and review record
    source/                      # authorized upstream source snapshot or Git submodule
    patches/                     # explicitly recorded HCC changes, if required
```

## Import und Wartung
- Vor Import Upstream-URL, Commit/Tag, Lizenz/Hinweise, Wartung, Abhängigkeiten, Sicherheitsprüfung, vorgesehenen Einsatz und menschliche Genehmigung dokumentieren. [Vorlage](../templates/UPSTREAM.md).
- Original-Lizenzen, Hinweise, Namensnennung und Herkunft bewahren. Geprüfte feste Revision, ggf. separates Core-Repository oder Submodule statt Duplikat. Original und HCC-Änderungen nachvollziehbar.
- Keine lokalisierten Produktdaten, vertraulichen Informationen, Präsentationsressourcen oder proprietären Quellen im Upstream; Anpassungen im Produkt, unvermeidbare Core-Patches separat geprüft.
- Updates, Kompatibilität und Sicherheit prüfen; NextSecurity-Tests verlinken. Kein Import unklarer Lizenz oder Herkunft, private Sichtbarkeit ist keine Lizenz.
- Projektbezogene Evaluation und Pläne in NextOpenSource/NextRoadmap; gemeinsame Bibliothek wiederverwenden.

## Komponenten
| Komponente | Upstream | Revision | Lizenz | Status |
|---|---|---|---|---|
| [NextID-Core](NextID-Core/README.md) | [Keycloak](https://github.com/keycloak/keycloak) | [`26.8.2`](https://github.com/keycloak/keycloak/commit/e514445f9dcdabc5bdcf67cab56c1e49655de067) | Apache-2.0 | Vollständiger unveränderter Quellstand; Sicherheits-/Build-Prüfung ausstehend |

Weitere Komponenten nach Prüfung und Autorisierung.