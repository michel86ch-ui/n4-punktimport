# N4 Punktimport

PointCheckout-Excel → Niagara 4 Import-CSV. Läuft komplett im Browser, keine Daten verlassen den Rechner.

**Tool öffnen:** https://michel86ch-ui.github.io/n4-punktimport/

## Verwendung
1. PointCheckout-Excel (.xlsx) per Drag & Drop hochladen
2. Vorschau prüfen, optional nach Anlage/Typ filtern
3. «Niagara-CSV herunterladen»
4. Niagara Workbench: File → Import → CSV → Zielordner → Finish

## Typ-Mapping
| Point Type | Niagara |
|---|---|
| Analog Input | bacnet:NumericPoint |
| Analog Output / Value | bacnet:NumericWritable |
| Binary Input | bacnet:BooleanPoint |
| Binary Output / Value | bacnet:BooleanWritable |
| MultiState Value | bacnet:EnumWritable |
| Accumulator | bacnet:NumericPoint |

CSV: UTF-8, Komma-getrennt, Punkt als Dezimalzeichen (unabhängig von CH-Regionaleinstellung).
