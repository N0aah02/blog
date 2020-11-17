---
title: Nameserver auf Cloudflare umstellen
date: 2020-11-12T18:08:41.279Z
published: true
tags:
  - nameserver
  - ip
cover_image: ../../static/images/uploads/nameserver.png
description: Stelle deine Nameserver auf Cloudflare um.
---
# 1. Systemsteuerung

Öffne die Systemsteuerung und klicke auf "Netzwerk und Internet" und anschliessend auf "Netzwerk- und Freugabecenter"

Alternativ einen beliebigen Ordner öffnen und "Systemsteuerung\Netzwerk und Internet\Netzwerk- und Freigabecenter" in die leiste oben eingeben und Enter drücken.

# 2. Auf das aktive Netzwerk klicken

![](../../static/images/uploads/2020-11-12_19-17-03.png)

# 3. Einstellungen verändern

Klicke anschliessend auf Eigenschaften > IPv4 > Eigenschaften > Folgende DNS-Serveradressen verwenden

Tippe schliessend in das erste Feld die folgende IP Adresse ein: 1.1.1.2

Anschliessend 1.0.0.2 in das zweite Fenster.

Klicke anschliessend bei jedem Fenster auf "OK" und die Änderungen zu bestätigen

![](../../static/images/uploads/2020-11-12_19-19-28.png)

# 4. Flush DNS

Falls die DNS Server nicht sofort übernommen wurden öffne die Konsole und tippe folgendes in die Konsole:

```
ipconfig /flushdns
```

Gib im anschluss den folgenden command ein und zu überprüfen, ob die nameserver übernommen wurden:

```
ipconfig /all
```

Falls da das folgende steht wurden die DNS Server übernommen und du kannst alle Fenster schliessen.

![](../../static/images/uploads/2020-11-12_19-28-30.png)

# Alternative nameserver:

**Standard Cloudflare Nameserver:**

1.1.1.1

1.0.0.1

**Malware blockieren:**

1.1.1.2

1.0.0.2

**Malware und erwachsenen Content blockieren:**

1.1.1.3

1.0.0.3

**Google Nameserver:**

8.8.8.8

8.8.4.4