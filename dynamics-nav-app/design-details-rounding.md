---
title: "Designdetails – Rundung"
description: "Rundungsreste können auftreten, wenn Sie die Kosten einer Bestandsminderung bewerten, die in einer anderen Menge als die entsprechende Bestandszunahme registriert wurde. Rundungsreste werden für alle Kostenberechnungsmethoden berechnet, wenn Sie die **Kosten anpassen - Artikeleintrag** -Stapelverarbeitung ausführen."
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2a5187811051ee2bd32ec44b22876f0a468225e2
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-rounding"></a>Designdetails: Rundung
Rundungsreste können auftreten, wenn Sie die Kosten einer Bestandsminderung bewerten, die in einer anderen Menge als die entsprechende Bestandszunahme registriert wurde. Rundungsreste werden für alle Kostenberechnungsmethoden berechnet, wenn Sie die **Kosten anpassen - Artikeleintrag**-Stapelverarbeitung ausführen.  

 Wenn Sie die Lagerabgangsmethode "Durchschnitt" verwenn, wird der Rundungsfunktionen Rückstand in einer kumulierten Posten-durch-Posten-Basis berechnet und erfasst.  

 Wenn Sie eine andere Lagerabgangsmethode als die Lagerabgangsmethode "Durchschnitt" verwenden, wird der Rundungsfunktionen Rückstand berechnet, wenn der Lagerzugang vollständig ausgeglichen wurde, d.h. wenn die Restmenge für den Lagerzugang gleich Null ist. Dann wird ein separater Posten für den ein Rundungsrest, und das Buchungsdatum dieses Rundungspostens ist das Buchungsdatum des zuletzt fakturierten Werts.  

## <a name="example"></a>Beispiel  
 Im folgenden Beispiel wird veranschaulicht, wie unterschiedliche Rundungsreste für die Durchschnittskostenbewertung und die Nicht-Durchschnittskostenbewertung behandelt werden. In beiden Fällen ist die **Kosten anpassen Artikeleingänge**-Stapelverarbeitung durchgeführt worden.  

 Die folgende Tabelle zeigt die Artikelposten, auf denen das Beispiel basiert.  

|Buchungsdatum|Menge|Lfd. Nr.|  
|------------------|--------------|---------------|  
|01-01-20|3|1|  
|02-01-20|-1|2|  
|03-01-20|-1|3|  
|04-01-20|-1|4|  

 Für einen Artikel, der die Durchschnittskostenmethode verwendet, wird die Rundungsfunktion Rückstand (1/300) mit der ersten Abgangspostennummer (Eingangsnummer 2) berechnet und auf die Postennummer 3 übertragen. Deshalb wird Postennummer 3 mit  3,34 bewertet.  

 Die folgende Tabelle zeigt die sich daraus ergebenden Wertposten.  

|Buchungsdatum|Menge|Einstandsbetrag (tatsächl.)|Artikelposten Lfd. Nr.|Lfd. Nr.|  
|------------------|--------------|----------------------------|---------------------------|---------------|  
|01-01-20|3|10|1|1|  
|02-01-20|-1|-3.33|2|2|  
|03-01-20|-1|-3.34|3|3|  
|04-01-20|-1|-3.33|4|4|  

 Für einen Artikel, der eine andere Kostenberechnungsmethode als Durchschnitt verwendet, wird der Rundungsrest (0,01) berechnet, wenn die Restmenge für die Bestandszunahme Null ist. Der Rundungsrest hat einen separaten Posten (Nummer 5).  

 Die folgende Tabelle zeigt die sich daraus ergebenden Wertposten.  

|Buchungsdatum|Menge|Einstandsbetrag (tatsächl.)|Artikelposten Lfd. Nr.|Lfd. Nr.|  
|------------------|--------------|----------------------------|---------------------------|---------------|  
|01-01-20|3|10|1|1|  
|02-01-20|-1|-3.33|2|2|  
|03-01-20|-1|-3.33|3|3|  
|04-01-20|-1|-3.33|4|4|  
|01-01-20|0|-0.01|0|5|  

## <a name="see-also"></a>Siehe auch  
 [Designdetails: Lagerkostenberechnung](design-details-inventory-costing.md)   
 [Designdetails: Kostenregulierung](design-details-cost-adjustment.md)   
 [Designdetails: Kostenmethoden](design-details-costing-methods.md) [Verwalten der Lagerregulierung](finance-manage-inventory-costs.md)  
 [Finanzen](finance.md)  
 [Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

