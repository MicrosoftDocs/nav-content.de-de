---
title: "Gewusst wie: Einrichten von Umsatzsteuervoranmeldungen für ELSTER"
description: "In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie die Umsatzsteuervoranmeldungsdatei-Benachrichtigung elektronisch an das ELSTER-Portal übermitteln."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: d717ccec6da7830a6ff315d595cb50869ab31c34
ms.contentlocale: de-de
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-sales-vat-advance-notifications-for-elster"></a>Gewusst wie: Einrichten von Umsatzsteuervoranmeldungen für ELSTER
In [!INCLUDE[navnow](../../includes/navnow_md.md)] müssen Sie zuerst Folgendes einrichten, damit Sie gültige Mehrwertsteuervoranmeldungen an das ELSTER-Portal übermitteln können.  

- Die Firmendaten und die Steuerinformationen.  
- Die Nummern gibt die Mehrwertsteuer-Voranmeldungsnummer an.  
- Die Benutzerauthentifizierung für die Steuerbehörden.  
- MwSt.-Abrechnung  

Sie müssen Komponenten auch vom ELSTER-Portal herunterladen. Weitere Informationen finden Sie unter [ELSTER-Onlineportal](http://go.microsoft.com/fwlink/?LinkId=155998).  

## <a name="to-set-up-company-information"></a>Um Unternehmensinformationen einzurichten:  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Symbol "Nach Seite oder Bericht suchen"") aus, geben Sie **Unternehmensdaten** ein, und wählen Sie dann den verknüpften Link aus.  
2.  Im Fenster **Firmendaten** im Inforegister **Allgemein**, im Feld **MwSt-Vertreter**, geben Sie die Kontaktperson für MwSt-bezogene Informationen ein.  
3.  Füllen Sie im Inforegister **Steuerdienst** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Description|  
    |------------------------------------|---------------------------------------|  
    |**Proxyserver verwenden**|Wählen Sie diese Option aus, um einen Proxyserver für die Kommunikation zu verwenden.|  
    |**Proxyserverauth. erforderlich**|Wählen Sie diese Option aus, um einen Proxyserver für die Authentifizierung zu verwenden.<br /><br /> Wenn Sie einen Proxyserverr und eine dedizierte Authentifizierung verwenden, müssen Sie das Benutzerkonto und das Kennwort vor der Übertragung eingeben. Wenn Sie die Windows-Authentifizierung verwenden, wählen Sie dieses Feld nicht aus.|  
    |**Proxyserver-IP-Adresse/-Port**|Die IP-Adresse und den Port, der für die Kommunikation verwendet wird, wenn Sie einen Proxyserver verwenden.|  

4.  Füllen Sie im Inforegister **HTTP-Server** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**HTTP-Server-URL 1**|Definiert einen Server der Oberfinanzdirektion (OFD), wie **http://datenannahme1.elster.de/Elster2/EMS**.|  
    |**HTTP-Server-URL 2**|Definiert einen Server der Oberfinanzdirektion (OFD), wie **http://datenannahme2.elster.de/Elster2/EMS**.|  
    |**HTTP-Server-URL 3**|Definiert einen Server der Oberfinanzdirektion (OFD), wie **http://datenannahme3.elster.de/Elster2/EMS**.|  
    |**HTTP-Server-URL 4**|Definiert einen Server der Oberfinanzdirektion (OFD), wie **http://datenannahme4.elster.de/Elster2/EMS**.|  

    Jetzt müssen Sie die Benutzer angeben, die Belege an das ELSTER-Portal übermitteln können.  

5.  Wählen Sie die **Zertifikate** Aktion aus.  

    Weitere Informationen über ELSTER-Zertifikate finden Sie unter [ELSTER-Onlineportal](http://go.microsoft.com/fwlink/?LinkId=155998).  

    1.  Im Fenster **Zertifikate** im Feld **Benutzer-ID**, geben Sie den Benutzer an, dem Sie die Berechtigung erteilen möchten, Dokumente an ELSTER zu senden.  
    2.  Wählen Sie die **Elster-Zertifikat hochladen** Aktion aus, und geben Sie die Zertifikatsdatei, z Coala2019.pem.cer an.  
    3.  Wählen Sie **PFX-Datei hochladen** und geben Sie dort die persönlichen Zertifikatsdatei für diesen Benutzer, wie test-soft-pse.pfx an.  

        > [!IMPORTANT]  
        >  Wenn Datenverschlüsselung nicht bereits ausgeführt wird, müssen Sie sie aktivieren, bevor Sie fortfahren.

    4.  Wählen Sie die Option **Kennwort für PFX-Datei festlegen** aus, und geben Sie dann das Kennwort für das persönliche Zertifikat an.  

6.  Wiederholen Sie Schritt 5 für andere Benutzer, die Dokumente an ELSTER senden.  
7.  Wählen Sie die Schaltfläche **OK** aus.  

## <a name="to-set-up-a-vat-statement-for-sales-vat-advance-notifications"></a>Um MwSt-Berichte für Umsatzsteuervoranmeldungs-Benachrichtigungen einzurichten  

1.  Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Nach Seite oder Bericht suchen") und geben die **MwSt-Bericht** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie im Fenster **MwSt-Bericht** im Feld **Name**, den Drop-Down-Pfeil.  
3.  Im Fenster **MwSt.-Abrechnungsnamen** in der Zeile für den entsprechenden MwSt.-Abrechnungsnamen wählen Sie das Feld **Verkaufs MwSt-Benachrichtigung** aus.  

    > [!NOTE]  
    >  Nur ein MwSt.-Abrechnungsname für eine Umsatzsteuervoranmeldung kann gleichzeitig ausgewählt werden. Die MwSt.-Abrechnung muss eine MwSt.-Abrechnungszeile für jede Kennzahl aufweisen, die vom Finanzamt, in der **Zeilennr.** gefordert wird Feld enthält die Kennzahl und das Feld **Betragsart** gibt an, ob es sich um eine Bemessungsgrundlage oder um einen Steuerbetrag handelt. Wenden Sie sich an Ihr Finanzamt, wenn Fragen zu den Schlüsselnummern und ihrer Definition bestehen.  

4.  Wählen Sie die Schaltfläche **OK** aus.  

## <a name="see-also"></a>Siehe auch  
 [Elektronische Übermittlung der Umsatzsteuervoranmeldungen an ELSTER](electronic-submission-of-sales-vat-advance-notifications-to-elster.md)   
 [Gewusst wie: Erstellen und Senden von Umsatzsteuervoranmeldungen](how-to-create-and-submit-sales-vat-advance-notifications.md)

