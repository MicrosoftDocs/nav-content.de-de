---
title: Vorgehensweise beim Erstellen und Senden von Umsatzsteuervoranmeldungen
description: "In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie die Umsatzsteuervoranmeldungsdatei elektronisch an das ELSTER-Portal übermitteln. Sie können die Umsatzsteuervoranmeldungsdatei elektronisch an das Finanzamt übertragen, nachdem Sie den errechneten Steuerbetrag und die Bemessungsgrundlage geprüft haben."
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
ms.openlocfilehash: e730b9e00f689cf4e42a8ff2e0a8d332ccc700d7
ms.contentlocale: de-de
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-and-submit-sales-vat-advance-notifications"></a>Gewusst wie: Erstellen und Senden von Umsatzsteuervoranmeldungen
In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie die Umsatzsteuervoranmeldungsdatei elektronisch an das ELSTER-Portal übermitteln. Sie können die Umsatzsteuervoranmeldungsdatei elektronisch an das Finanzamt übertragen, nachdem Sie den errechneten Steuerbetrag und die Bemessungsgrundlage geprüft haben.  

## <a name="to-create-an-xml-document-for-sales-vat-advance-notification"></a>So erstellen Sie ein XML-Dokument für Umsatzsteuervoranmeldung  

1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](../../media/ui-search/search_small.png "Symbol „Nach Seite oder Bericht suchen”") aus, und geben Sie **Umsatzsteuervoranmeldungsliste** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Im Fenster **Umsatzsteuervoranmeldungsliste** auf der Registerkarte Aktionen, wählen Sie **Neu** aus.  
3.  Füllen Sie im Fenster **USt.-Voranmeldungskarte** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Description|  
    |------------------------------------|---------------------------------------|  
    |**Ansprechpartner für Finanzamt**|Die Kontaktperson für das Finanzamt in Ihrer Organisation.|  
    |**Telefonnummer Kontakt**|Telefonnummer der Kontaktperson.|  
    |**Kontakt-E-Mail**|E-Mail-Adresse der Kontaktperson.|  

5.  Wählen Sie die Aktion **XML-Datei erstellen** aus.  
6.  Im Batchauftrag **MwSt.-Voranmeldung erstellen** im Inforegister **Optionen**, im Feld **XML-Datei**, wählen Sie **Erstellen** oder **Erstellen und anzeigen** aus.  
7.  Wählen Sie die Schaltfläche **OK** aus.  

## <a name="to-submit-an-xml-document-for-sales-vat-advance-notification"></a>So übermitteln Sie ein XML-Dokument für Umsatzsteuervoranmeldung  

1.  Im Fenster **Umsatzsteuervoranmeldungsliste** wählen Sie den Beleg aus, den Sie an ELSTER senden möchten.  
2.  Wählen Sie die Aktion **XML-Datei übermitteln** aus.  

Die XML-Datei wird an ELSTER übermittelt.  

## <a name="see-also"></a>Siehe auch  
 [Elektronische Übermittlung der Umsatzsteuervoranmeldungen an ELSTER](electronic-submission-of-sales-vat-advance-notifications-to-elster.md)   
 [Gewusst wie: Einrichten von Umsatzsteuervoranmeldungen für ELSTER](how-to-set-up-sales-vat-advance-notifications-for-elster.md)

