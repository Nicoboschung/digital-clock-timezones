# CARE – Build a Bundle Produktseite

Mix & Match: Kund:innen wählen 3 Produkte aus allen Produkten (auch dasselbe mehrfach), inkl. Grösse/Farbe, und erhalten 15 % Rabatt.

## Dateien
| Datei | Wohin in Shopify |
|---|---|
| `sections/care-build-a-bundle.liquid` | Onlineshop → Themes → Code bearbeiten → **Sections** → „Neue Section“ `care-build-a-bundle` → Inhalt ersetzen |
| `templates/product.build-a-bundle.json` | **Templates** → „Neues Template“ → Typ *product*, Name `build-a-bundle` → Inhalt ersetzen |

## Einrichtung (5 Schritte)
1. **Rabattcode anlegen:** Rabatte → Rabatt erstellen → *Betrag von Produkten* → Code `BUNDLE15`, **15 %**,
   gilt für die Bundle-Produkte (bzw. Kollektion), Mindestanforderung **Mindestanzahl Artikel: 3**.
   Der Code wird nach „In den Warenkorb“ automatisch über `/discount/BUNDLE15` angewendet.
2. **Bundle-Produkt anlegen:** Produkt „Build a Bundle“ (Preis egal, wird nicht in den Warenkorb gelegt),
   im Vertriebskanal *Onlineshop* aktiv → rechts **Theme-Vorlage: `build-a-bundle`**.
3. **Im Theme-Editor** (Vorlage *build-a-bundle*): Titelbild + Text oben, Foto 1 + Foto 2, Beschreibung,
   optional eine Kollektion/Produktliste (leer = alle Produkte).
4. **Trust Points** als Blöcke bearbeiten (Icon wählbar oder eigenes Icon hochladen). Falls ihr eure
   bestehende Trust-Section lieber verwenden wollt: Blöcke löschen und eure Section darunter hinzufügen.
5. **Farben/Schriftgrössen** stehen unter „Design (CARE Branding)“. Schriften werden automatisch aus dem
   Theme übernommen (`--font-heading-family` / `--font-body-family`).

## Hinweis Rabatt
Shopify-Themes können Preise im Warenkorb nicht selbst ändern – deshalb der Rabattcode.
Der Code gilt für alle passenden Artikel im Warenkorb mit mind. 3 Stück. Soll der Rabatt **nur** für
Bundle-Artikel gelten, braucht es eine Bundle-App (z. B. Shopify Bundles) oder eine Shopify Function.
