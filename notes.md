# Gedanken und Notizen zu ToDos und möglichen Issues

## Grundlegendes

Was wollen wir mit diesem Programm denn eigentlich machen? Wollen wir ein "Host your own Goodreads?", wollen wir was anderes?

Wie gehen wir mit der Tatsache um, daß welche Bücher eine Person besitzt/liest/gutfindet bzw. wer wem welche Bücher borgt teils sehr sensible, persönliche Daten sind, die nicht *leichfertig* gesammelt oder abgreifbar sein sollten.

Warum sollten Menschen dieses Tool verwenden? Wozu?

## Notwendige Funktionalität

### User Management
Vieles hier wird vermutlich Django für uns übernehmen, sollte aber dennoch mitgedacht werden.

- Login
- Passwortmanagement
- Sessionhandling
- Angelegte User löschen
- kontaktdaten/Benachrichtigungen?

### BookCatalogue Exporte importieren
- Export parsen
- Import
- Wie mit Dublikaten umgehen?
- User Input in Import? ("Dieses Buch nicht importieren, ...")

### Bookshelves

Buchsammlungen sind sensible Daten!

- Einzelne Bücher nicht importieren/private schalten
- Evt. konfigurierbar machen das Bücher mit gew. UUIDs auch bei späteren Import nicht übernommen werden?
- Datensicherheit!
- Anzeige einzelner Datenfelder konfigurierbar machen
- Sinnvolle Defaults (Alle Bücher private? ...)

### Bookshelves anderer User ansehen

- Wie public?
- Sortierbar

### Social Stuff

- User wegen Leihwunsch kontaktieren? Wie? (Mail durch Tool? oder einfach Kontaktdaten auf user page?)
- Verleihstatus sichtbar machen?
- Wie konfigurierbar? (Nur über reimport abändern, also Konfig über BC app? Oder in dstrbooks änderbar, dadurch aber out-of-sync mit app?)

### Import/Export

- Sync?!? (Änderungen nur über App/reimport wär einfach aber unfreundlich. Andersrum ist benutzbarer, aber macht sync/mergeprobleme. Und Arbeit.)
- Export als druckbares Inventarverzeichnis? Oder statisches html für's blog?
- Wie Duplikate oder zwischenzeitliche Änderung in App-DB handhaben?

### Extras

- Statistiken? (Pro User? über alle user? Public?)
- Soziales Netzwerkfoo? ("User -- Buch", "User -- User", "Buch -- Buch", ...)
- Buchvorschlagszeugs?


