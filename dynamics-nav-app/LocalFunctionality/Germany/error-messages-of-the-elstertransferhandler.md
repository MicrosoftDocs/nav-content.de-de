---
title: Fehlermeldungen des ElsterTransferHandler
description: "Wenn [!INCLUDE[navnow](../../includes/navnow_md.md)] Umsatzsteuervoranmeldungen übermittelt, können Fehler auftreten."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 434419448d45b6f82b2e9217fa61c29a6a91c151
ms.contentlocale: de-de
ms.lasthandoff: 10/23/2017

---
# <a name="error-messages-of-the-elstertransferhandler"></a>Fehlermeldungen des ElsterTransferHandler
Wenn [!INCLUDE[navnow](../../includes/navnow_md.md)] Umsatzsteuervoranmeldungen übermittelt, können Fehler auftreten.  

Wenn beispielsweise die Konfigurationsdatei für die Microsoft.Dynamics.ElsterTransferHandler.dll-Assembly nicht den richtigen Anzeigenamen des öffentlichen Zertifikats enthält, gibt das ELSTER-Portal den Fehler 3400 zurück, und [!INCLUDE[navnow](../../includes/navnow_md.md)] zeigt die entsprechende Fehlermeldung an.  

## <a name="error-messages"></a>Fehlermeldungen  
In der folgenden Tabelle sind die Fehlermeldungen aufgelistet, die das ELSTER-Portal an [!INCLUDE[navnow](../../includes/navnow_md.md)] übermittelt.  

|**Fehlernummer**|**Beschreibung**|  
|----------------------|-------------------------------------------|  
|1000|ELSTER kann den Absender nicht als [!INCLUDE[navnow](../../includes/navnow_md.md)] identifizieren. Die Microsoft.Dynamics.ElsterTransferHandler.dll-Assembly kann nur mit Microsoft Dynamics-Produkten verwendet werden.|  
|2000|Es konnte beim Übermitteln von Daten keine Verbindung zu den OFD-Servern hergestellt werden. Dies kann ein Problem mit Ihrer Netzwerkverbindung sein. Prüfen Sie Ihre Netzwerkkonfiguration, oder versuchen Sie es zu einem späteren Zeitpunkt erneut.|  
|2100|Die XML-Datei konnte nicht gesendet werden, da die Verbindung unerwartet unterbrochen wurde.|  
|2200|Es konnte beim Empfangen von Daten keine Verbindung zu den OFD-Servern hergestellt werden. Dies kann ein Problem mit Ihrer Netzwerkverbindung sein. Prüfen Sie Ihre Netzwerkkonfiguration, oder versuchen Sie es zu einem späteren Zeitpunkt erneut.|  
|2300|Das Antwortdokument konnte nicht empfangen werden, da die Verbindung unerwartet unterbrochen wurde.|  
|3000|ELSTER konnte nicht auf das benutzerspezifische Zertifikat zugreifen. Sie müssen sich vergewissern, dass das Zertifikat richtig installiert ist.|  
|3100|Sie haben ein Dokument übermittelt, haben aber keinen Zugriff auf den Zertifikatspeicher. Sie müssen sich vergewissern, dass das Zertifikat richtig installiert ist.|  
|3200|Das benutzerspezifische Zertifikat konnte nicht gefunden werden. Sie müssen sich vergewissern, dass das Zertifikat richtig installiert ist.|  
|3300|Das angegebene Zertifikat weist keinen privaten Schlüssel auf, oder das Kennwort für den privaten Schlüssel ist falsch. Sie müssen sich vergewissern, dass das Zertifikat richtig installiert ist.|  
|3400|Das öffentliche Zertifikat der OFD konnte nicht geöffnet werden. Sie müssen sich vergewissern, dass das Zertifikat richtig installiert ist.|  
|4000|Das Antwortdokument konnte nicht entschlüsselt werden, da der private Schlüssel nicht mit dem öffentlichen Schlüssel übereinstimmt, der für die Verschlüsselung verwendet wurde.|  
|4100|Das Antwortdokument konnte nicht entschlüsselt werden. Die Daten wurden während der Übermittlung möglicherweise beschädigt. Sie müssen das Dokument erneut senden.|  
|5000|Das Dokument konnte nicht komprimiert werden. Dies kann auf einen Mangel an Speicherplatz auf dem Computer zurückzuführen sein, oder dass das Betriebssystem den Komprimierungsprozess beendet hat. Sie müssen das Dokument erneut senden.|  
|5100|Das Dokument konnte nicht dekomprimiert werden. Sie müssen das Dokument erneut senden.|  
|6000|Der Proxyserver antwortet nicht. Sie müssen sicherstellen, dass die Einrichtung von Umsatzsteuervoranmeldungen in [!INCLUDE[navnow](../../includes/navnow_md.md)] korrekt ist.|  
|6100|Der Benutzer ist nicht dazu in der Lage, eine Verbindung mit dem Server herzustellen. Sie müssen sicherstellen, dass die Einrichtung von Umsatzsteuervoranmeldungen in [!INCLUDE[navnow](../../includes/navnow_md.md)] korrekt ist.|  
|6200|Der Benutzer konnte nicht auf dem Proxyserver registriert werden. Sie müssen sicherstellen, dass die Einrichtung von Umsatzsteuervoranmeldungen in [!INCLUDE[navnow](../../includes/navnow_md.md)] korrekt ist.|  
|7000|Die Daten konnten nicht signiert werden, da das konfigurierte Zertifikat nicht zum Signieren von Daten verwendet werden kann. Sie müssen sicherstellen, dass die Einrichtung von Umsatzsteuervoranmeldungen in [!INCLUDE[navnow](../../includes/navnow_md.md)] korrekt ist.|  
|7100|Das XML-Dokument konnte nicht signiert werden. Dies kann auf einen Mangel an Speicherplatz auf dem Computer zurückzuführen sein, oder dass das Betriebssystem den Komprimierungsprozess beendet hat.|  
|9000|Ein Fehler ist aufgetreten, als das ELSTER-Portal versuchte, die Konfiguration des Zertifikats zu lesen. Sie müssen den Inhalt des generierten XML-Dokuments prüfen.|  

## <a name="see-also"></a>Siehe auch  
 [ELSTER-Übermittlung – Übersicht](elster-transmission-overview.md)   
 [Gewusst wie: Einrichten von Umsatzsteuervoranmeldungen für ELSTER](how-to-set-up-sales-vat-advance-notifications-for-elster.md)

