---
title: collectHighEntropyUserAgentHints
description: Verwenden Sie die Variable collectHighEntropyUserAgentHints , um zu bestimmen, ob Adobe hohe Entropy-Hinweise von Chromium-Browsern anfordert (z. B. Google Chrome und Microsoft Edge).
source-git-commit: 885a8f229fa814053e4766f3b38b6e7fb209fc00
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 4%

---


# collectHighEntropyUserAgentHints

Clienthinweise mit hoher Entropie werden von Adobe Analytics verwendet, um die Geräte- und Browseridentifizierung zu verbessern. Diese Option ist ab Version 2.23.0 von AppMeasurment.js verfügbar. Weitere Informationen zu Client-Hinweisen finden Sie in [diese Übersicht und FAQs](/help/technotes/client-hints.md) sowie [Google-Blog](https://web.dev/user-agent-client-hints/).

## Erfassen Sie mit dem Web SDK Hinweise mit hoher Entropie.

Clienthinweise mit hoher Entropie sind Teil der Kontextkategorien im Web SDK. Siehe [Konfigurieren des Platform Web SDK](https://experienceleague.adobe.com/docs/experience-platform/edge/fundamentals/configuring-the-sdk.html?lang=en) für weitere Details.

## Erfassen Sie mit der Adobe Analytics-Erweiterung Hinweise mit hoher Entropie.

**[!UICONTROL Benutzeragenten-Hinweise mit hoher Entropie sammeln]** ist ein Kontrollkästchen unter dem Akkordeon Allgemein bei der Konfiguration der Adobe Analytics-Erweiterung.

1. Anmelden bei [Adobe Experience Platform-Datenerfassung](https://experience.adobe.com/#/@adobepm/data-collection) mit Ihren Adobe ID-Anmeldeinformationen.

1. Klicken Sie auf die gewünschte [!UICONTROL Tag-Eigenschaft].

1. Navigieren Sie zu [!UICONTROL Erweiterungen] Registerkarte und klicken Sie dann auf [!UICONTROL Konfigurieren] unter Adobe Analytics.

1. Erweitern Sie die [!UICONTROL Allgemein] Akkordeon, das die [!UICONTROL Benutzeragenten-Hinweise mit hoher Entropie sammeln] aktivieren. Sie ist standardmäßig deaktiviert.

## collectHighEntropyUserAgentHints in AppMeasurement

Die `s.collectHighEntropyUserAgentHints` bestimmt, ob AppMeasurement High-Entropy-Hinweise von Chromium-Browsern anfordert (z. B. Google Chrome und Microsoft Edge). Diese Hinweise werden von Adobe Analytics zur Verbesserung der Geräte- und Browseridentifizierung verwendet.

Wenn auf TRUE gesetzt, werden alle hohen Entropy-Hinweise vom Browser angefordert.

`s.collectHighEntropyUserAgentHints = TRUE`

`s.collectHighEntropyUserAgentHints = FALSE`