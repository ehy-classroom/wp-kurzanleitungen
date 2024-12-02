# WordPress Multisite einrichten

**Kurzanleitung: WordPress Multisite einrichten**
Version: 1.0

------

## Einführung

Eine WordPress-Multisite erlaubt es, mehrere Websites innerhalb einer einzigen WordPress-Installation zu verwalten. Jede Website kann eigene Inhalte, Themes und Plugins haben, während sie dieselbe Datenbank und WordPress-Core-Dateien nutzt. Dieses Setup eignet sich besonders für Netzwerke wie Unternehmensintranets, Schulnetzwerke oder Blogs.

------

## Voraussetzungen

- **WordPress Installation:** Du benötigst eine funktionierende WordPress-Installation. Dies kann lokal oder auf einem Webserver erfolgen.
- **Admin-Zugang:** Zugriff auf die WordPress-Administrationsoberfläche und die WordPress-Dateien.
- **Datenbank- und FTP-Zugang:** Zum Bearbeiten der `wp-config.php` und `htaccess`-Dateien.

------

## Schritte zur Einrichtung

### 1. Multisite aktivieren

1. Öffne die Datei `wp-config.php` im Hauptverzeichnis deiner WordPress-Installation.
2. Füge den folgenden Code direkt vor der Zeile `/* That's all, stop editing! Happy publishing. */` hinzu:

```php
define('WP_ALLOW_MULTISITE', true);
```

1. Speichere die Datei und lade sie auf deinen Server hoch, falls du per FTP arbeitest.

### 2. Multisite-Netzwerk einrichten

1. Melde dich als Administrator in deinem WordPress-Backend an.
2. Navigiere zu **Werkzeuge > Netzwerk-Einrichtung**.
3. Wähle den Netzwerktyp:
   - **Subdomains:** `site1.dein-domain.de` (erfordert Wildcard-DNS-Einstellungen).
   - **Unterverzeichnisse:** `dein-domain.de/site1`.
4. Fülle die Felder für Titel und Admin-E-Mail aus.
5. Klicke auf **Netzwerk installieren**.

### 3. Konfiguration der Dateien

Nach der Installation zeigt WordPress spezifische Code-Blöcke, die du manuell in zwei Dateien einfügen musst:

#### In `wp-config.php`:

Füge den von WordPress generierten Code **oberhalb** der Zeile `/* That's all, stop editing! Happy publishing. */` ein.

#### In `.htaccess`:

Ersetze den bisherigen Inhalt mit dem vorgeschlagenen Code. Falls `.htaccess` nicht existiert, erstelle die Datei im WordPress-Hauptverzeichnis.

### 4. Netzwerkkonfiguration überprüfen

1. Melde dich erneut im WordPress-Backend an.
2. Unter **Meine Sites > Netzwerkverwaltung > Dashboard** findest du die zentrale Steuerung für dein Netzwerk.

------

## Tipps und häufige Probleme

- **Wildcard-DNS:** Für Subdomains muss dein Server Wildcard-DNS unterstützen. Dies kann über deinen Hosting-Anbieter eingerichtet werden.
- **Speicherlimits:** Erhöhe ggf. die `upload_max_filesize` und `memory_limit` in deiner `php.ini`, um das Hochladen großer Dateien zu ermöglichen.
- **Themes und Plugins:** Diese werden auf Netzwerkebene installiert und dann für einzelne Websites freigeschaltet.

------

## Fazit

Mit WordPress Multisite kannst du mehrere Websites effizient verwalten. Die Einrichtung erfordert nur wenige Schritte, bietet aber eine flexible Basis für größere Projekte.

------

