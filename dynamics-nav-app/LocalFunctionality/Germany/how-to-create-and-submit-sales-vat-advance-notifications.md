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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1a0509e523e0c6d8e83dc288a49650b17865a33a
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-and-submit-sales-vat-advance-notifications"></a>Gewusst wie: Erstellen und Senden von Umsatzsteuervoranmeldungen
In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie die Umsatzsteuervoranmeldungsdatei elektronisch an das ELSTER-Portal übermitteln. Sie können die Umsatzsteuervoranmeldungsdatei elektronisch an das Finanzamt übertragen, nachdem Sie den errechneten Steuerbetrag und die Bemessungsgrundlage geprüft haben.  
  
### <a name="to-create-an-xml-document-for-sales-vat-advance-notification"></a>So erstellen Sie ein XML-Dokument für Umsatzsteuervoranmeldung  
  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol „Nach Seite oder Bericht suchen”") aus, und geben Sie **Umsatzsteuervoranmeldungsliste** ein. Wählen Sie dann den zugehörigen Link aus.  
  
2.  Im Fenster **Umsatzsteuervoranmeldungsliste** auf der Registerkarte **Aktionen**, wählen Sie **Neu** aus.  
  
3.  Füllen Sie im Fenster **USt.-Voranmeldungskarte** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  
  
    |Feld|Description|  
    |---
    Titel: Beschreibung der Vorgehensweise beim Erstellen und Übermitteln von Umsatzsteuervoranmeldungen: In [!INCLUDE[navnow](../../includes/navnow_md.md)] können Sie die Umsatzsteuervoranmeldungsdatei elektronisch an das ELSTER-Portal übermitteln. Sie können die Umsatzsteuervoranmeldungsdatei elektronisch an das Finanzamt übertragen, nachdem Sie den errechneten Steuerbetrag und die Bemessungsgrundlage geprüft haben.
    
    documentationcenter: '' author: SorenGP

    ms.prod: "dynamics-nav-2017" ms.topic: article ms.devlang: na ms.tgt_pltfrm: na ms.workload: na ms.search.keywords: ms.date: 07/01/2017 ms.author: sgroespe

---------------------------------|---------------------------------------|  
    |**Kontaktperson für Finanzamt**|Die Kontaktperson für das Finanzamt in Ihrer Organisation.|  
    |**Kontakt Telefonnr.**|Die Telefonnummer der Kontaktperson.|  
    |**Kontakt-E-Mail**|Die E-Mail-Adresse der Kontaktperson.|  
  
5.  Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **XML-Datei erstellen** aus.  
  
6.  Im Batchauftrag **USt.-Voranmeldung erstellen** im Inforegister **Optionen**, im Feld **XML-Datei**, wählen Sie **Erstellen** oder **Erstellen und anzeigen** aus.  
  
7.  Wählen Sie die Schaltfläche **OK** aus.  
  
### <a name="to-submit-an-xml-document-for-sales-vat-advance-notification"></a>So übermitteln Sie ein XML-Dokument für Umsatzsteuervoranmeldung  
  
1.  Im Fenster **Umsatzsteuervoranmeldungsliste** wählen Sie den Beleg aus, den Sie an ELSTER senden möchten.  
  
2.  Wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **XML-Datei übertragen** aus.  
  
     Die XML-Datei wird an ELSTER übermittelt.  
  
## <a name="see-also"></a>Siehe auch  
 [Elektronische Übermittlung der Umsatzsteuervoranmeldungen an ELSTER](electronic-submission-of-sales-vat-advance-notifications-to-elster.md)   
 [Gewusst wie: Einrichten von Umsatzsteuervoranmeldungen für ELSTER](how-to-set-up-sales-vat-advance-notifications-for-elster.md)   
 MwSt.-Abrechnung   
 USt.-Voranmeldungskarte   
 Umsatzsteuervoranmeldung   
 XML-Datei für USt.-VA erst.
