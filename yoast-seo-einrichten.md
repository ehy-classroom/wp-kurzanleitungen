# Yoast SEO Plugin installieren und einrichten

**Kurzanleitung: Grundlegende Installation und Einrichtung des Yoast SEO Plugins**
Version: 1.0

------

## Was ist Yoast SEO?

Yoast SEO ist eines der bekanntesten WordPress-Plugins zur Suchmaschinenoptimierung. Es bietet einfache Werkzeuge, um Inhalte zu optimieren, Sitemaps zu erstellen und technische SEO-Anforderungen zu erfüllen.

------

## Voraussetzungen

- **WordPress-Installation:** Eine funktionierende WordPress-Website.
- **Administratorrechte:** Zugang zum WordPress-Dashboard mit Admin-Rechten.

------

## Schritte zur Installation

### 1. Yoast SEO Plugin installieren

1. Melde dich im **WordPress-Admin-Dashboard** an.
2. Gehe zu **Plugins > Installieren**.
3. Suche nach „Yoast SEO“ in der Suchleiste.
4. Klicke auf **Jetzt installieren**.
5. Nach der Installation klicke auf **Aktivieren**.

### 2. Yoast SEO einrichten

Nach der Aktivierung erscheint ein neuer Menüpunkt **SEO** in der linken Navigationsleiste.

------

## Grundlegende Einrichtung

### 1. Konfigurationsassistent

1. Navigiere zu **SEO > Allgemein > Konfigurationsassistent**.
2. Folge den einzelnen Schritten:
   - **Umgebung:** Wähle, ob deine Website live oder in Entwicklung ist.
   - **Website-Typ:** Gib an, ob es sich um einen Blog, eine Unternehmensseite oder eine andere Art von Website handelt.
   - **Organisation/Person:** Füge den Namen und ggf. ein Logo hinzu.
   - **Suchmaschinenindexierung:** Entscheide, ob Suchmaschinen bestimmte Inhaltstypen indexieren sollen (z. B. Beiträge und Seiten).

### 2. SEO-Titel und Metadaten anpassen

1. Gehe zu **SEO > Allgemein > Suche Erscheinungsbild**.
2. Passe Titel und Metabeschreibungen für die Startseite, Beiträge und Seiten an.
3. Nutze Variablen wie `%title%` oder `%sitename%`, um dynamische Titel zu erstellen.

Beispiel für Titel-Vorlage:
 `%title% | %sitename%`

------

## Wichtige Einstellungen

### 1. XML Sitemaps aktivieren

- Gehe zu **SEO > Allgemein > Funktionen**.
- Aktiviere die **XML Sitemap-Funktion**.
- Die Sitemap ist unter `https://deinedomain.de/sitemap_index.xml` erreichbar.

### 2. Inhaltstypen und Taxonomien

- Unter **SEO > Suche Erscheinungsbild > Inhaltstypen** kannst du festlegen, ob Beiträge, Seiten oder andere Inhalte indexiert werden sollen.
- Unter **Taxonomien** bestimmst du, ob Kategorien und Tags in Suchmaschinen sichtbar sein sollen.

### 3. Lesbarkeitsanalyse und SEO-Check

- In jedem Beitrag und jeder Seite findest du einen Yoast SEO-Bereich.
- Dieser zeigt:
  - **SEO-Bewertung:** Optimierung des Fokus-Schlüsselworts.
  - **Lesbarkeitsanalyse:** Vorschläge zur Verbesserung der Textstruktur.

------

## Tipps für die Verwendung

1. **Fokus-Schlüsselwörter setzen:** Wähle für jeden Beitrag ein Haupt-Schlüsselwort. Yoast SEO hilft dir, dieses optimal einzusetzen.
2. **Vorsicht bei Metabeschreibungen:** Schreibe individuelle Beschreibungen, die das Fokus-Schlüsselwort enthalten.
3. **Social Sharing:** Unter **SEO > Social** kannst du Open Graph-Metadaten aktivieren, um das Teilen in sozialen Netzwerken zu verbessern.

------

## Fazit

Das Yoast SEO Plugin ist eine umfassende Lösung für die Suchmaschinenoptimierung. Mit der Grundkonfiguration und den bereitgestellten Tools kannst du den SEO-Status deiner Website deutlich verbessern.