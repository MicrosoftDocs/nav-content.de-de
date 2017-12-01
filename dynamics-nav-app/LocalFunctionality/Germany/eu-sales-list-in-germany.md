---
title: Zusammenfassende Meldung in Deutschland
description: "In Deutschland wird die deutsche zusammenfassende Meldung an das „Bundeszentralamt für Steuern” (BZSt) über das BZSt-Onlineportal mithilfe der ELMA5-Schnittstelle übermittelt."
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
ms.openlocfilehash: fb18e25289f291f541672dca719c103cccbe390f
ms.contentlocale: de-de
ms.lasthandoff: 10/23/2017

---
# <a name="eu-sales-list-in-germany"></a>Zusammenfassende Meldung in Deutschland
In Deutschland wird die deutsche zusammenfassende Meldung an das „Bundeszentralamt für Steuern” (BZSt) über das BZSt-Onlineportal mithilfe der ELMA5-Schnittstelle übermittelt.  

Um die Sicherheit zu erhöhen, müssen alle Arten von Steuern und Steuererklärungen unter einer Authentifizierungsmethode übermittelt werden. Seit 1. Januar 2013 ist es obligatorisch, dass Sie Übermittlungen mit Authentifizierung vornehmen. Dazu melden Sie sich mit Ihrer BZSt-Nummer und Ihrem privaten Schlüssel an, indem Sie Ihre Passphrase im ELMA5-Kommunikationsserver verwenden. ELMA5 ist dafür ausgelegt, die Übermittlung großer Datasets von mehr als 1000 Datensätzen zu handhaben. Nach erfolgreicher Anmeldung können Sie die Datenübertragung in interaktiver Weise hochladen. Sie können die Übertragung auf automatisch einrichten.  

## <a name="implementation-in-includenavnowincludesnavnowmdmd"></a>Implementierung in [!INCLUDE[navnow](../../includes/navnow_md.md)]  
 [!INCLUDE[navnow](../../includes/navnow_md.md)] und übermitteln Sie es dann an die Verarbeitungsbehörde (ZIVIT).
 
> [!IMPORTANT]  
>  Die Möglichkeit, einen MwSt.-Bericht in einem XML-Format zu übermitteln, wird nicht unterstützt. Sie können jedoch eine Übermittlung von weniger als 1000 Datensätzen in einer CSV-Datei vornehmen. Dazu können Sie das Elster-Onlineportal verwenden und die Stapelverarbeitung „Zusammenfassende Meldung Disk”, Bericht 88, verwenden.

## <a name="see-also"></a>Siehe auch  
[BZSt-Onlineportal](http://www.bzst.de)   
[Gewusst wie: MwSt.-Berichte erstellen](how-to-create-vat-reports.md)

