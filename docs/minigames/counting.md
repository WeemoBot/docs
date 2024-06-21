---
title: "Counting"
description: "Benötigst du Hilfe bei der Einrichtung von Counting?"
sidebar_position: 4
---

Was ist Counting?
--------------------------
In diesem Spiel wird in einem Kanal gezählt. Es beginnt mit 1 und der nächste muss die nächste Zahl in den Kanal tippen.

Wie wird es eingerichtet?
--------------------------
Es muss ein Textkanal mit ``/count setchannel`` konfiguriert werden.

# Es startet nicht, was soll ich tun?
- Gebe ``/count settings`` ein und schaue nach, ob Weemo den Kanal aufgelistet hat.
- Überprüfe, ob Weemo die Berechtigung **Kanal sehen** und **Nachrichtenverlauf einsehen** hat.
- Falls Weemo die benötigten Berechtigungen hat, setze den Kanal erneut.

Der NoFail-Modus
--------------------------
In diesem Modus wird strikt gezählt. Tippt jemand eine falsche Zahl ein, wird der Zähler auf 1 zurückgesetzt.