---
title: "Häufige Fragen und Probleme"
sidebar_position: 3
---

# Häufige Fragen und Probleme
Wie kann ich einen Befehl deaktivieren?
------------------------
Gehe dazu in die Servereinstellungen, klicke auf **Integrationen**, dort sollte Weemo aufgelistet sein. Du klickst auf Weemo und erhältst dort eine Übersicht ihrer Befehle.
Klicke nun den Befehl, den du deaktivieren willst, an. Wähle die Rolle **@everyone** aus, setze das :x: und klicke auf Speichern.

![Befehl deaktivieren](/img/disable_command.png)

:::note
Das versteckt den Befehl für Mitglieder, aber wird für Administratoren weiterhin sichtbar bleiben.
:::

Weemo verteilt Rollen nicht!
----------------
Kontrolliere ob Weemo die Berechtigung **Rollen verwalten** hat.
Gehe dazu in die Servereinstellungen, wähle Weemo's Rolle aus und überprüfe, ob ein Haken :white_check_mark: gesetzt wurde.

:::note
Weemo kann nur Rollen verteilen, die unter ihrer höchsten Rolle sind. Überprüfe hier, ob das Mitglied eine höhere Rolle als Weemo hat.
:::
    
Weemo reagiert langsam oder überhaupt nicht, was soll ich tun?
------------------------
### Discord's Statusseite überprüfen
Discord hat gelegentlich mal Ausfälle oder Einschränkungen, die dann meist viele Bots gleichzeitig treffen können.
Überprüfe auf der [Statusseite](https://discordstatus.com), ob derzeit im Reiter "API" eine Störung vorliegt.

### Weemo's Status überprüfen

Suche nach Weemo in der Mitglieder-Liste auf der rechten Seite.

![Weemo's Bild in der Mitgliederliste.](/img/weemo_online_status.webp)

⚪ **Falls** der Punkt neben Weemo's Profilbild grau ist:
- dann ist Weemo offline. Du musst kurz warten, bis Weemo wieder online ist.
- Sollte Weemo länger offline sein, kannst du auf dem [Weemo HQ](https://weemo.ink/discord) nachschauen,
  wann Weemo voraussichtlich neu gestartet wird.

🟢 **Falls** der Punkt neben Weemo's Profilbild grün ist:
- dann ist Weemo online

⚫ **Falls** Weemo nicht in der Liste ist:
- dann kann Weemo den Kanal nicht sehen. Ändere die Rechte, sodass Weemo den Kanal sehen kann.

:::note
*Auf größeren Servern (>1000 Mitglieder) kann es passieren, dass Mitglieder, die offline sind, nicht angezeigt werden.*
*In diesem Fall kannst du Weemo's Online-Status über die Mitgliederliste des Servers oder über andere Bots herausfinden.*
:::


### Weemo's Berechtigungen überprüfen
Gehe in die Rolleneinstellungen auf deinem Server und überprüfe Weemo's Berechtigungen.
- Weemo braucht die Rechte *Kanäle ansehen*, *Nachrichten senden* und *Links einbetten*, um Antworten zu senden. 
Für weitere Funktionen benötigt Weemo eventuell weitere Berechtigungen. In ihrem [Einladungslink](https://weemo.ink/invite) sind alle benötigten Berechtigungen, um optimal auf deinem Server funktionieren zu können, bereits ausgewählt.

In privaten Kanälen muss Weemo zusätzlich dem Kanal hinzugefügt werden, sofern sie nicht in der Mitgliederleiste auftaucht:
- Am Computer: Gehe in den Kanaleinstellungen auf *Mitglied oder Rolle hinzufügen* und füge Weemo hinzu.

- Am Handy oder über *Erweiterten Berechtigungen*:
  - Gehe in die Kanaleinstellungen.
  - Füge Weemos Rolle hinzu, sofern nicht schon getan.
  - Aktiviere *Kanal zeigen*, *Nachrichten senden* und *Links einbetten*.

### Falls das alles nicht geklappt hat...
Trete dem [Weemo HQ](https://weemo.ink/discord) bei und erstelle ein Ticket.

Was ist eine ID?
----------------

Eine ID ist eine lange Zahl, die von Discord genutzt wird, um Elemente auseinanderzuhalten.

**Zwei Gedankenspiele:**
- Stell dir vor, du schreibst eine Nachricht. Zwei Sekunden später schreibst du versehentlich die
gleiche Nachricht in den selben Kanal. Nun willst du die zweite Nachricht löschen.
Wie kannst du Discord mitteilen, dass du nur die zweite der beiden identischen Nachrichten löschen willst?

- Stell dir vor, dein Nutzername ist *Alice#1234*. Nun änderst du ihn zu *Bob#4321*.
Doch dein Server wurde von *Alice#1234* erstellt.
Wie erkennt Discord, dass der Server immer noch dir gehört, obwohl dein Name anders ist?

Darum bekommt jeder Nutzer, jeder Server, jeder Kanal, jedes Emoji, jede Nachricht und eigentlich alles auf Discord eine ID.
Diese ID ist eine 16 bis zwanzigstellige Zahl und sieht zum Beispiel so aus: ``452763583348998155``.
Einmal vergeben, kann diese ID kein zweites mal vorkommen und nicht geändert werden.
Discord arbeitet nur mit IDs, auch wenn sie meist nicht angezeigt werden.

Zwei identische Nachrichten von der gleichen Person haben zwei verschiedene IDs. So kann Discord sie unterscheiden.
Bei deinem Server ist als Owner nicht dein Name, sondern deine ID gespeichert.
Änderst du deinen Nutzernamen, ist das egal, da die ID die gleiche bleibt.

Wie bekomme ich eine ID?
------------------------

Es gibt drei Arten, eine ID herauszufinden:

-  Erwähne den Kanal, den Nutzer oder die Rolle dessen ID du bekommen möchtest.
   Schreibe dann direkt vor die Erwähnung ein Backslash (das ist dieses Zeichen: ``\``)
   Die Nummer, die Discord nach dem Senden der Nachricht anzeigt ist die ID.
   Die Klammern und Sonderzeichen um die Nummer herum sind kein Teil der ID.

   :::warning
   Die Nutzer und Rollen erhalten trotzdem einen Ping.
   :::

-  Schalte den Entwicklermodus von Discord ein.
   Gehe dazu auf *Einstellungen* > *Verhalten* und aktiviere *Entwicklermodus*.
   Wenn du nun einen Nutzer, einen Kanal oder eine Rolle mit der rechten Maustaste anklickst
   (oder auf dem Handy lange gedrückt hältst) kannst du über ``ID kopieren`` die ID kopieren.

   :::note
   Auf dem Handy musst du im Menü ggf. nach unten scrollen, um den Punkt ``ID kopieren`` zu sehen.
   :::

-  Nutze die Befehle ``roleinfo``, ``userinfo`` oder ``serverinfo``.
   Weemo wird dir auch dort die ID anzeigen.

