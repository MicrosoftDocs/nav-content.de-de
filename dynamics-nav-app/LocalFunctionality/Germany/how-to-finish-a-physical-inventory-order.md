---
title: "Gewusst wie: Einen Inventurauftrag abschließen"
description: "Nach Abschluss des Inventurauftrags können Sie die Inventurdifferenzen analysieren."
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
ms.openlocfilehash: acd7007597664c06786c18475e7c4177788880f9
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-finish-a-physical-inventory-order"></a>Gewusst wie: Einen Inventurauftrag abschließen
Nach Abschluss des Inventurauftrags können Sie die Inventurdifferenzen analysieren.  
  
 Ein Inventurauftrag kann nur abgeschlossen werden, wenn Folgendes zutrifft:  
  
-   Alle zugehörigen Inventurerfassungen müssen den **Status** "Beendet" aufweisen.  
  
-   In allen Inventurauftragszeilen wurde die erwartete Menge berechnet.  
  
     [!INCLUDE[navnow](../../includes/navnow_md.md)]Die Anwendung kennzeichnet dies durch Aktivierung des Kontrollkästchens  In Erfassungszeilen enthalten für die jeweilige Inventurauftragszeile.  
  
-   Jede Inventurauftragszeile wurde mit mindestens einer Inventurerfassungszeile gezählt.  
  
     Dies wird angegeben, indem Sie im Feld Aufzeichnungs-Zeilen das Gebiet der Inventurauftragszeile auswählen. Für eine Inventurauftragszeile können Sie eine Liste der Inventurerfassungszeilen anzeigen.  
  
### <a name="to-finish-a-physical-inventory-order"></a>So schließen Sie einen Inventurauftrag ab  
  
1.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol „Nach Seite oder Bericht suchen”"), geben Sie **Bestandsauftrag** ein, und wählen Sie dann den zugehörigen Link aus.  
  
2.  Öffnen Sie den Inventurauftrag, dessen Statistiken Sie anzeigen möchten.  
  
3.  Wählen Sie auf der Registerkarte **Start** in der Gruppe **Funktionen** die Option **Beenden** aus.  
  
     Die Anwendung setzt den Status im Inventurauftragskopf auf **Beendet**. Sie können den Inventurauftragskopf oder die Inventurauftragszeilen nun nicht mehr ändern.  
  
 Beim Abschluss des Inventurauftrags vergleicht die Anwendung die erwartete Menge und die erfassten Mengen des Inventurauftragskopfes und berechnet die Abweichungen.  
  
 Sie müssen den Status im Inventurauftragskopf erst auf "Beendet" setzen, bevor Sie Differenzen auswerten und den Inventurauftrag buchen können.  
  
## <a name="see-also"></a>Siehe auch  
 [Gewusst wie: Eingeben von Inventuraufträgen](how-to-enter-physical-inventory-orders.md)   
 [Gewusst wie: Buchen von Inventuraufträgen](how-to-post-physical-inventory-orders.md)   
 [Gewusst wie: Berechnen der verfügbaren Menge für einen Inventurauftrag](how-to-calculate-quantity-on-hand-for-a-physical-inventory-order.md)   
 [Gewusst wie: So schließen Sie eine Inventurerfassung ab](how-to-finish-a-physical-inventory-recording.md)   
 [Gewusst wie: Analysieren von Inventurdifferenzen](how-to-analyze-physical-inventory-differences.md)   
 [Inventurauftragszeilen mit Artikelverfolgungszeilen](physical-inventory-order-lines-with-item-tracking-lines.md)
