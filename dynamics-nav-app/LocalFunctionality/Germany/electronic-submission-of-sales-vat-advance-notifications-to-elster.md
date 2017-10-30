---
title: "Elektronische Übermittlung der Umsatzsteuervoranmeldungen an ELSTER"
description: "In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie Steuerbelege und MwSt.-Abrechnungen, wie die Umsatzsteuervoranmeldung, an das Finanzamt elektronisch übermitteln."
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ab9d7174651d5b2688da0de1a7baaebe12755414
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="electronic-submission-of-sales-vat-advance-notifications-to-elster"></a>Elektronische Übermittlung der Umsatzsteuervoranmeldungen an ELSTER
In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie Steuerbelege und MwSt.-Abrechnungen, wie die Umsatzsteuervoranmeldung, an das Finanzamt elektronisch übermitteln.  
  
## <a name="sales-vat-advance-notifications"></a>Umsatzsteuervoranmeldungen  
 [!INCLUDE[navnow](../../includes/navnow_md.md)] erstellt ein XML-Dokument, das die Steuerbeträge und Bemessungsgrundlagen zusammen mit den Firmeninformationen enthält. Sie können die Daten überprüfen, bevor Sie sie an das Finanzamt übermitteln. Sie können das XML-Dokument mithilfe des Layouts einrichten, das in der Formatvorlage der Finanzämter definiert ist. Sie können dann das XML-Dokument an die Schnittstelle des Onlineportals „Elektronische Steuererklärungen (ELSTER)” der Finanzämter übermitteln.  
  
 Zuerst müssen Sie ADD INCLUDE<!--[!INCLUDE[navnow](how-to-create-and-submit-sales-vat-advance-notifications.md) einrichten.  
  
 Der Server der Finanzämter verarbeitet das übermittelte XML-Dokument und sendet als Antwort ein XML-Dokument. Dieses Antwortdokument zeigt Codes und Beschreibungen für Fehler an, die während der Verarbeitung des übermittelten XML-Dokuments aufgetreten sind. Die XML-Dokumente sind während der Übermittlung verschlüsselt. Weitere Informationen finden Sie unter [ELSTER-Onlineportal](http://go.microsoft.com/fwlink/?LinkId=155998).  
  
## <a name="architectural-overview"></a>Architekturübersicht  
 ADD INCLUDE<!--[!INCLUDE[navnow](elster-transmission-overview.md).  
  
 Das ELSTER-Portal hat Anforderungen an Computer, die Belege übermitteln. Dies ../../umfasst ein Softwarezertifikat, das Sie für jeden Benutzer erwerben müssen, der Dokumente an ELSTER übermittelt. Sie müssen Ihre Installation anhand von Informationen überprüfen, die im [ELSTER-Onlineportal](http://go.microsoft.com/fwlink/?LinkId=155998) verfügbar sind. Im nächsten Abschnitt werden Installationsüberlegungen für Ihre [!INCLUDE[navnow](../../includes/navnow_md.md)]-Implementierung beschrieben.  
  
### <a name="installation-considerations"></a>Installationsüberlegungen  
 Die Microsoft.Dynamics.ElsterTransferHandler.dll-Assembly wird als Teil der Installation des ADD INCLUDE<!--[!INCLUDE[nav_windows](../../includes/nav_windows_md.md)]--> installiert.  
  
> [!NOTE]  
>  Zuvor installieren Sie eine neue Version von [!INCLUDE[navnow](../../includes/navnow_md.md)].  
  
 ELSTER benötigt Zertifikate, um das Unternehmen und die Person zu identifizieren, die das jeweilige Dokument übermittelt. Auf dem Computer jedes Benutzers, der eine Erklärung an ELSTER sendet, müssen Sie die folgenden Zertifikate installieren:  
  
-   Das öffentliche Zertifikat der Finanzämter.  
  
-   Ein persönliches PFX-Zertifikat für diesen Benutzer.  
  
 Sie müssen dann die Benutzer und die Anzeigenamen der Zertifikate im Fenster **Zertifikate** aufführen. Weitere Informationen darüber, wie ein Zertifikat installiert wird und wie Sie den Anzeigenamen suchen, finden Sie in der Hilfe zum Betriebssystem.  
  
 Wenn Sie einen Proxyserver verwenden, um die ELSTER-Dokumente zu senden, müssen Sie die Einstellungen im Fenster **Elektronische Umsatzsteuererklärung – Einrichtung** angeben.  
  
 Weitere Informationen finden Sie unter [Gewusst wie: Einrichten von Umsatzsteuervoranmeldungen für ELSTER](how-to-set-up-sales-vat-advance-notifications-for-elster.md).  
  
### <a name="certificates-and-style-sheets"></a>Zertifikate und Formatvorlagen  
 Ihr Unternehmen muss sich im ELSTER-Onlineportal registrieren, sodass Sie die erforderlichen Zertifikate erhalten können. Wenn Sie sich bereits registriert haben, müssen Sie sich nicht erneut registrieren.  
  
> [!IMPORTANT]  
>  Das ELSTER-Onlineportal bietet drei Methoden der Verbindung, aber [!INCLUDE[navnow](../../includes/navnow_md.md)].  
  
 Nachdem Sie sich im ELSTER-Onlineportal registriert haben, müssen Sie ein persönliches Zertifikat erwerben. Sie müssen auch das öffentliche Zertifikat der Finanzämter und die Formatvorlagen herunterladen, die für die Datenübermittlungen benötigt werden. Wenn Sie das persönliche Zertifikat auf dem Computer des Benutzers installieren, werden Sie aufgefordert, ein Kennwort anzugeben.  
  
 Das öffentliche Zertifikat der Finanzämter steht zum Download vom ELSTER-Onlineportal zur Verfügung. Der aktuelle Dateiname ist Coala2019.pem.cer.  
  
 Das persönliche PFX-Zertifikat wird benötigt, um den Benutzer deutlich zu identifizieren, der die Belege an das Finanzamt übermittelt. Das persönliche Zertifikat enthält eine digitale Signatur, die in den übermittelten XML-Dateien enthalten ist. Der Name des Benutzers, der die Dateien übermittelt hat, ist auch enthalten.  
  
 Sie müssen alle relevanten Formatvorlagen herunterladen, die die Finanzämter zur Verfügung stellen. Dazu ../../gehört die Formatvorlage ustva.xsl, die Sie im Fenster **USt.-Voranmeldungskarte** angeben müssen, aber die Finanzämter benötigen möglicherweise zusätzliche Formatvorlagen, die sich im selben Ordner, wie die Formatvorlage ustva.xsl befinden müssen.  
  
 Weitere Informationen finden Sie unter [ELSTER-Onlineportal](http://go.microsoft.com/fwlink/?LinkId=155998)  
  
### <a name="transmissions"></a>Übermittlungen  
 Im Fenster „USt.-Voranmeldungsübersicht” können Sie Umsatzsteuervoranmeldungen erstellen und senden. Wenn Sie ein Dokument erstellen, können Sie dieses in der Vorschau anzeigen, bevor Sie es an das ELSTER-Portal senden. Die Dokumente, die erstellt werden, basieren auf den XML-Formatvorlagen, die im ELSTER-Portal veröffentlicht werden, und auf dem Zertifikat und anderen Informationen, die Sie in [!INCLUDE[navnow](../../includes/navnow_md.md)] eingerichtet haben .  
  
 Nachdem Sie ein Dokument an ELSTER gesendet haben, wird ein Eintrag im Fenster **MwSt.-Übertragungsprotokollposten** vorgenommen. Wenn das ELSTER-Onlineportal das übertragene Dokument verarbeitet, können Fehler auftreten und ADD INCLUDE<!--[!INCLUDE[navnow](elster-transmission-overview.md).  
  
## <a name="see-also"></a>Siehe auch  
 [Gewusst wie: Einrichten von Umsatzsteuervoranmeldungen für ELSTER](how-to-set-up-sales-vat-advance-notifications-for-elster.md)   
 [Gewusst wie: Erstellen und Senden von Umsatzsteuervoranmeldungen](how-to-create-and-submit-sales-vat-advance-notifications.md)   
 [ELSTER-Onlineportal](http://go.microsoft.com/fwlink/?LinkId=155998)   
 USt.-Voranmeldungskarte   
 Zertifikate   
 MwSt.-Übertragungsprotokollposten
