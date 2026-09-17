# Sattmacher-Java-Plugin

Ein maßgeschneidertes Server-Plugin für Minecraft (Paper-API für Version 1.21.1 / Spigot-kompatibel), das einen interaktiven Chat-Befehl zur Sattmachung von Spielern hinzufügt.

### Funktionen
- **`/Sattmacher` Befehl:** Setzt die Saturation des ausführenden Spielers sofort auf das Maximum (20 Punkte / 10 volle Hungerkeulen).
- **Farbiger Chat-Feedback:** Sendet eine Erfolgsmeldung in etwas was braun sein sollte (`§6`) direkt an den Spieler.
- **Konsolen-Schutz:** Das Plugin prüft aktiv, ob der Befehl von einem echten Spieler oder der Server-Konsole kommt, um Abstürze zu verhindern.

### Gelernte Grundlagen & API-Konzepte
- **Schnittstellen (Interfaces):** Nutzung von `CommandExecutor` zur Registrierung eigener Befehle.
- **Event- / Lifecycle-Methoden:** Steuerung des Plugins beim Serverstart (`onEnable`) und Serverstopp (`onDisable`).
- **Vererbung & Typenprüfung:** Überprüfung des Befehls-Senders mittels `instanceof Player` und anschlegendem Typecasting.
- **Konfigurationsdateien:** Strukturierung der `plugin.yml` (YAML) zur Registrierung von Befehlen und Berechtigungen (`permissions`).
- **Build-Management:** Projekt-Konfiguration und Kompilierung in eine `.jar`-Datei mittels **Gradle**.
