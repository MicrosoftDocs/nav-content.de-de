---
title: "Vorgehensweise beim Berechnen der verfügbaren Menge für einen Inventurauftrag"
description: "Nachdem Sie den Inventurauftrag erstellt und die Inventurauftragszeilen eingegeben haben, müssen Sie vom Programm das Feld „Erwartete Menge (Basis)” für die einzelnen Inventurauftragszeilen berechnen lassen."
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
ms.openlocfilehash: bfb4ff63ea61a0b340920fd252a8e895c6ef643a
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-calculate-quantity-on-hand-for-a-physical-inventory-order"></a>Gewusst wie: Berechnen der verfügbaren Menge für einen Inventurauftrag
Nachdem Sie den Inventurauftrag erstellt und die Inventurauftragszeilen eingegeben haben, müssen Sie vom Programm das Feld „Erwartete Menge (Basis)” für die einzelnen Inventurauftragszeilen berechnen lassen.  
  
 Wenn die Erstellung dieser Inventurauftragszeilen von [!INCLUDE[navnow](../../includes/navnow_md.md)] automatisch durchgeführt wurde, konnten Sie auf der Anforderungsseite für die Stapelverarbeitung festlegen, ob die erwartete Menge berechnet werden soll. Wenn Sie die Inventurauftragszeilen manuell erstellt oder zwischenzeitlich geändert haben, müssen Sie die erwarteten Mengen manuell berechnen. Sie können Mengen auf zwei Arten berechnen, wie im folgenden Abschnitt erläutert.  
  
### <a name="to-calculate-the-expected-quantity-on-the-physical-inventory-order"></a>So wird die erwartete Menge im Inventurauftrag berechnet  
  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol „Nach Seite oder Bericht suchen”"), geben Sie **Bestandsauftrag** ein, und wählen Sie dann den zugehörigen Link aus.  
  
2.  Öffnen Sie den Inventurauftrag, für den Sie die erwartete Menge berechnen möchten.  
  
3.  Um die erwartete Menge nur einer Inventurauftragszeile zu berechnen, wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **Erwartete Menge berechnen**, und wählen Sie dann **Diese Zeile** aus.  
  
4.  Um die erwartete Menge in allen Inventurauftragszeilen zu berechnen, wählen Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktionen** die Option **Erwartete Menge berechnen**, und wählen Sie dann **Alle Zeilen** aus.  
  
     Im Dialog, der angezeigt wird, wählen Sie aus, dass die Mengen für alle Zeilen oder für die Zeilen berechnet werden, die noch nicht berechnet wurden.  
  
 Wenn [!INCLUDE[navnow](../../includes/navnow_md.md)] die erwartete Menge bereits berechnet hat, ist das Kontrollkästchen für „Berechnete erw. Menge” der Inventurauftragszeile aktiviert.  
  
> [!NOTE]  
>  Das Verfahren zur Durchführung der Inventur und zu deren Erfassung in der Inventurerfassung ist von der Berechnung der erwarteten Mengen unabhängig.  
  
 Sie müssen die erwarteten Mengen für alle Inventurauftragszeilen eines Inventurauftrags berechnen, bevor Sie das Feld „Status” auf **Beendet** setzen. Der Grund hierfür ist, dass [!INCLUDE[navnow](../../includes/navnow_md.md)] die erwarteten und die erfassten Mengen vergleicht und die Differenzen zu Buchungszwecken berechnet.  
  
## <a name="see-also"></a>Siehe auch  
 [Gewusst wie: Eingeben von Inventuraufträgen](how-to-enter-physical-inventory-orders.md)   
 [Inventurerfassung – Inventurzählung](physical-inventory-recording-counting-physical-inventory.md)   
 [Gewusst wie: Einen Inventurauftrag abschließen](how-to-finish-a-physical-inventory-order.md)   
 [Gewusst wie: So schließen Sie eine Inventurerfassung ab](how-to-finish-a-physical-inventory-recording.md)   
 [Inventurauftragszeilen mit Artikelverfolgungszeilen](physical-inventory-order-lines-with-item-tracking-lines.md)
