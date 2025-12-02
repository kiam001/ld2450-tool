# ld2450-tool

WICHTIG: Das Problem mit CORS (Cross-Origin)

Wenn du das Tool auf GitHub Pages hostest, wird Home Assistant den Zugriff standardmäßig blockieren, weil die Anfrage von einer "fremden" Webseite kommt.

Du musst Home Assistant erlauben, Anfragen von deiner GitHub-Seite anzunehmen.

Öffne deine configuration.yaml in Home Assistant.
Füge folgenden Block hinzu (oder ergänze ihn, falls http: schon existiert):

YAML:
```
http:
  cors_allowed_origins:
    - https://DEIN-GITHUB-NAME.github.io
```

Starte Home Assistant neu.


    
