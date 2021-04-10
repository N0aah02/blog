---
title: Minecraft Server mit Domain verbinden
date: 2021-04-10T12:31:42.308Z
published: true
tags:
  - minecraft
  - server
  - domain
cover_image: ../../static/images/uploads/2021-04-10_14-31-27.png
description: Verbinde deine Minecraft Server IP mit deiner eigenen Domain
---
# 1. DNS Einstellungen

Suche die DNS Einstellungen bei deinem Domain hoster und drücke da auf "eintrag erstellen"

# 2. Server Infos heraussuchen

Suche dir die folgenden infos zu deinem Minecraft server heraus:

Server IP: z.b. 45.86.168.161

Port: z.b. 40120 (falls kein Port angegeben ist, ist es der standardport 25565)

Falls du nur eine subdomain hast z.b. pvpserver.minecraftserver.com suche dir die IP Adresse und den port [hier](https://mcsrvstat.us/) unter "show debug info" heraus

# 3. DNS Einträge erstellen

## Erstelle dir einen **A Eintrag** mit den folgenden werten:

Name: mc1

TTL: 3600

Value / Wert: **SERVER IP** (ohne port)



## Erstelle dir anschliessend einen **SRV Eintrag** mit den folgenden werten:

Service: minecraft

Protokoll: TCP

Name: **DEINE DOMAIN** (Damit kannst du dich später auf den Server verbinden, z.b. deinedomain.de oder minecraft.deinedomain.de)

TLL: 3600

Priority / Priorität: 1

Weight / Gewicht: 1

Port: **SERVER PORT**

Target / Ziel: **WERT** ( benutze den **Namen**, welchen du beim **A Eintrag** benutzt hast, z.b. mc1.deinedomain.de)

# 4. Warten

Jenachdem bei wem du die Einträge bearbeitet hast kann es bis zu 24 Stunden dauern, bis die Einträge gültig werden. Überprüfe desshalb nochmal ob alle Einträge auch wirklich stimmen.