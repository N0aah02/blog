---
title: Discord Webhook per Zapier versenden
date: 2020-11-08T15:30:04.604Z
published: true
tags:
  - webhook
  - zapier
  - discord
cover_image: ../../static/images/uploads/component-1-.png
description: Versende einen Webhook and Discord über Zapier
---
<!--StartFragment-->

## Zapier Account erstellen

Erstelle dir einen Zapier account auf <https://zapier.com/sign-up/>

![](../../static/images/uploads/zap1.png)

## Anwendung verknüpfen

Erstelle dir hier einen neuen "Zap"<https://zapier.com/app/editor>

Wähle deine Anwendung aus die du Verbinden möchtest und Autorisiere dich damit

![](../../static/images/uploads/zap2.png)

Wähle deinen "Auslöser" und wähle anschliessend deinen Account aus

![](../../static/images/uploads/zap3.png)

Wähle im nächsten Schritt "Webhooks by Zapier" aus

![](../../static/images/uploads/zap3.png)

Wähle als Aktion "Custom Request" aus

![](../../static/images/uploads/zap4.png)

Wähle als "Methode" POST aus und füge unter URL die [Webhook](https://support.discordapp.com/hc/de/articles/228383668-Webhooks-verwenden) url ein

![](../../static/images/uploads/zap5.png)

## Embed erstellen

Erstelle dir unter [https://discohook.org/](https://discohook.org/?message=eyJtZXNzYWdlIjp7fX0) den Inhalt der Gepostet werden soll. Achte darauf, dass du Felder die sich im nachhinein ändern mit Platzhaltern versehst

Kopiere dir anschliessend die "JSON data" welche unten auf der Website generiert wird.

Füge anschliessend deine Eigenen Daten hinzu

![](../../static/images/uploads/zap6.png)

Füge unter "Headers" den folgenden Text ein:

> Content-Type application/json

![](../../static/images/uploads/zap7.png)

Drücke anschliessend auf Continue und Teste ob eine Nachricht versendet wird

![](../../static/images/uploads/zap8.png)

Drücke anschliessend auf Done und anschliessend auf "TURN ON ZAP"

<!--EndFragment-->